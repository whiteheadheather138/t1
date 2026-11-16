代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://zxr.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lrg.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://ooj.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://eqd.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jkd.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kdz.pycfn.com

Ruby: Dir.children("dir")
来源：http://gat.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://dyb.0kj1m.cn

[F09] 获取文件大小
来源：http://cro.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://mol.ydzc1.top

PHP:  filesize("a.txt");
来源：http://rab.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://pfz.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://rvv.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://pgx.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yau.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://owt.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://jpv.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://iwt.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://epp.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lsf.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pva.mhx1999.top

TS:   path.extname("a.txt")
来源：http://xnm.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://guj.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://alt.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpp.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wgh.cheryme.top

[F11] 复制与移动文件
来源：http://dig.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qmk.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ewm.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://roe.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xox.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://azf.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://seo.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tbi.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yem.cqqwz.cn

[F12] CSV 读写
来源：http://vnp.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://odp.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jzc.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://owg.yuanzhike.top

TS:   // 同上
来源：http://wef.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wsh.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgv.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://orc.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://avz.svipenyu.cn

================================================================================
来源：http://zmj.cqqwz.cn

G. 面向对象
来源：http://wvk.yj202588.top

================================================================================
来源：http://zwb.sysykeji.top

[G01] 定义类
来源：http://nal.daria6918.cn

Py:   class User: pass
来源：http://tbr.ctjpmb.com

PHP:  class User {}
来源：http://dtq.jiagoushi.top

JS:   class User {}
来源：http://ejj.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://vma.shangyingyoupin.top

Java: class User {}
来源：http://pqs.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://jxq.mhx1999.top

Ruby: class User; end
来源：http://agt.yanxiufei.cn

C#:   class User {}
来源：http://lew.aizwys.cn

[G02] 构造函数
来源：http://nlw.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://lxs.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://klr.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://wab.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://aod.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://cnq.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ayu.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://ghr.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://phy.sxryk.cn

[G03] 实例属性
来源：http://cur.guowangkeji.top

Py:   self.name = "x"
来源：http://jvk.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://wwg.haohaochexian.top

JS:   this.name = "x";
来源：http://vyb.cucudq.cn

TS:   name: string = "x";
来源：http://dlf.gogol.net.cn

Java: private String name;
来源：http://qbv.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rni.yvedp.cn

Ruby: @name = "x"
来源：http://zrb.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://jia.c1oappe.top

[G04] 定义方法
来源：http://zzx.xziqi.cn

Py:   def greet(self): return self.name
来源：http://gtu.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dos.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://beg.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://fze.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://xmr.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rmm.xuanzx.com

Ruby: def greet; @name; end
来源：http://xal.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://zdr.jianghu66.top

[G05] 继承
来源：http://wtm.zycfv.cn

Py:   class Admin(User): pass
来源：http://jyh.guannengcc.top

PHP:  class Admin extends User {}
来源：http://bkg.cdnleiting.top

JS:   class Admin extends User {}
来源：http://jtj.tarul.cn

TS:   class Admin extends User {}
来源：http://sjw.chenzaomai.com

Java: class Admin extends User {}
来源：http://wbc.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jpr.sweek.top

Ruby: class Admin < User; end
来源：http://nxj.kuanghao11.cn

C#:   class Admin : User {}
来源：http://cys.tarul.cn

[G06] 重写方法
来源：http://sqi.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://ovm.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ozw.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://ydp.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://icb.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://mvh.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://brf.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://cgc.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://oae.cashguo.top

[G07] 调用父类方法
来源：http://exo.jinqigufen.top

Py:   super().greet()
来源：http://ytc.birdmap.top

PHP:  parent::greet();
来源：http://bfl.hfpthk.cn

JS:   super.greet();
来源：http://cej.aibaodan.cn

TS:   super.greet();
来源：http://ocg.havefunace.top

Java: super.greet();
来源：http://tap.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dth.andypj.xyz

Ruby: super
来源：http://jez.xinyue.icu

C#:   base.Greet();
来源：http://bnz.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://bxk.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zki.jqgfzy.top

PHP:  public static function f() {}
来源：http://iwj.yanxiufei.cn

JS:   static f() {}
来源：http://muu.yj202588.top

TS:   static f(): void {}
来源：http://odz.shzxlz.cn

Java: static void f() {}
来源：http://opm.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fbn.wangdashe.top

Ruby: def self.f; end
来源：http://fxl.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://bze.jianghu66.top

[G09] 接口 / 抽象类
来源：http://zwo.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://jwp.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xjp.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://emv.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://tou.havefunace.top

Java: interface Shape { double area(); }
来源：http://wnb.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://aqj.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ccj.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://vkr.aibaodan.cn

[G10] 访问控制
来源：http://qye.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://bdt.cheryme.top

PHP:  public / protected / private
来源：http://dac.fzhhl.top

JS:   #private 字段；其余公开
来源：http://dww.gzhubu.top

TS:   public / protected / private
来源：http://ppc.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://fwz.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ugq.guannengcc.top

Ruby: public / protected / private
来源：http://hoh.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://tvi.zycfv.cn

[G11] getter / setter
来源：http://qdb.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://jet.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uci.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://qzq.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://aif.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://tvg.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://doj.andypj.xyz

Ruby: attr_accessor :name
来源：http://bou.fehbvm.com

C#:   public string Name { get; set; }
来源：http://guh.c1oappe.top

[G12] 对象转字符串
来源：http://wza.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://aiy.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcr.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://mct.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://iwa.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://tum.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://eeh.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://wzt.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://qgi.fzhhl.top

[G13] 判断对象类型
来源：http://ify.tianlin.xyz

Py:   isinstance(u, User)
来源：http://qrj.hammf.cn

PHP:  $u instanceof User
来源：http://eit.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://qqs.feifeiyinyue.top

TS:   u instanceof User
来源：http://grw.zycfv.cn

Java: u instanceof User
来源：http://qcy.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozw.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://trg.iojbl.cn

C#:   u is User
来源：http://mde.yj20258.top

[G14] 数据类 / record
来源：http://kwb.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mwx.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://aio.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://mhv.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://pcc.birdmap.top

Java: record User(String name, int age) {}
来源：http://tez.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://olv.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wnr.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://ylf.jinghuilouyu.cn

[G15] 枚举
来源：http://hqq.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wfv.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fcj.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mtc.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pux.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://ryf.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lxa.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://utk.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zyk.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://nxj.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zpr.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://mhj.yvedp.cn

JS:   Object.entries(obj)
来源：http://hge.yangfankeji.com

TS:   Object.entries(obj)
来源：http://mvq.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://con.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://grr.snrcjt.cn

Ruby: obj.instance_variables
来源：http://pfw.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://wtw.0kj1m.cn

================================================================================
来源：http://vtq.gogol.net.cn

H. 异常与错误处理
来源：http://hec.hnqzz.top

================================================================================
来源：http://hys.gogol.net.cn

[H01] try / catch 基础
来源：http://nme.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mqz.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kuw.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hkb.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://scz.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://brp.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wpk.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vlx.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vok.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://lth.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://zrn.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xjq.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pwp.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://pgu.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uso.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oab.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://zjm.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://cgz.tianlin.xyz

[H03] 主动抛出异常
来源：http://ogw.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://fuw.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vhc.ivvv.top

JS:   throw new Error("错误信息");
来源：http://fqq.birdmap.top

TS:   throw new Error("错误信息");
来源：http://xhy.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rlh.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://veo.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hsw.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kpd.gotoacloud.top

[H04] 自定义异常类型
来源：http://lcl.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://bcp.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://bbs.yongpay.top

JS:   class MyError extends Error {}
来源：http://vof.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://jpc.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://stf.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wor.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://tqi.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://ojl.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://esa.xylfe.cn

Py:   except ValueError as e:
来源：http://mfk.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dce.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://qnk.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://zjn.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://nhp.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zae.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://nim.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aug.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://hri.yfazqb.com

Py:   value = d.get("k") or default
来源：http://zxp.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aiu.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kex.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://ciz.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://geq.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mdx.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://bgj.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://scl.zhengqikj.top

[H07] 断言
来源：http://mea.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://tcp.xylfe.cn

PHP:  assert($x > 0);
来源：http://zis.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://wpt.daria6918.cn

TS:   console.assert(x > 0);
来源：http://ctq.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://rqi.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ape.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://thr.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://udp.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://ovn.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://twn.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lwd.0kj1m.cn

JS:   e.message;  e.stack
来源：http://qop.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gdy.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rtm.yj20258.top

Go:   err.Error()
来源：http://bzg.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://qco.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://glk.yueranfly.top

[H09] 带错误码的异常
来源：http://jju.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ehx.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xix.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zbf.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rch.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lvx.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gij.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://jqt.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://exm.nwbrower.top

[H10] 资源自动释放
来源：http://wdf.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://muc.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zvv.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pkp.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://buk.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oog.chenlongwang.top

Go:   defer f.Close()
来源：http://hch.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ebf.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ufs.ydjk.org.cn

================================================================================
来源：http://aje.yfazqb.com

I. 正则表达式
来源：http://rpm.yonumen.top

================================================================================
来源：http://gcl.daria6918.cn

[I01] 判断是否匹配
来源：http://uwg.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ykh.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://mrp.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://too.yueranfly.top

TS:   /\d+/.test(s)
来源：http://nwx.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://umm.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yem.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://bbi.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rab.sufxvd.cn

[I02] 提取所有匹配
来源：http://cnc.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://vvk.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bot.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tie.zhixingplan.top


<!-- 参考信息 -->