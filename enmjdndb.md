代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jpi.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://azx.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://rel.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://wav.guannengcc.top

[F09] 获取文件大小
来源：http://gup.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://jwx.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://dal.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://cdy.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://dcq.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://snv.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hpo.ivvv.top

Ruby: File.size("a.txt")
来源：http://zxs.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://uyu.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://aem.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ngr.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fzz.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://suv.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://izr.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvz.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hca.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rqy.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gia.yuanzhike.top

[F11] 复制与移动文件
来源：http://phy.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iuf.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fuo.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xpq.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swr.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://auo.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gdq.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tsi.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qkj.feifeiyinyue.top

[F12] CSV 读写
来源：http://ulk.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://icv.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pqq.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mwh.feifeiyinyue.top

TS:   // 同上
来源：http://svb.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lot.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pns.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xda.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://kvg.gogol.net.cn

================================================================================
来源：http://qdp.chenlongwang.top

G. 面向对象
来源：http://nyi.zhijiandao.cn

================================================================================
来源：http://ijy.zhongyouzk.top

[G01] 定义类
来源：http://hli.fzhhl.top

Py:   class User: pass
来源：http://hso.jinqigufen.top

PHP:  class User {}
来源：http://kfm.zdbjq.cn

JS:   class User {}
来源：http://szn.hammf.cn

TS:   class User { name: string = ""; }
来源：http://tjg.zdbjq.cn

Java: class User {}
来源：http://zby.yj20258888.top

Go:   type User struct { Name string }
来源：http://ups.daxiang520.top

Ruby: class User; end
来源：http://oib.fehbvm.com

C#:   class User {}
来源：http://mki.yj202588.top

[G02] 构造函数
来源：http://rpg.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://npy.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://wzq.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://vnu.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://dcy.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://dij.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bso.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://owt.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://dtz.fehbvm.com

[G03] 实例属性
来源：http://mlq.meibo888.top

Py:   self.name = "x"
来源：http://htd.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://trv.fengsongda.top

JS:   this.name = "x";
来源：http://rrn.shuidangran.top

TS:   name: string = "x";
来源：http://ahm.jinghuilouyu.cn

Java: private String name;
来源：http://mvl.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nxk.zhoulong.xyz

Ruby: @name = "x"
来源：http://mzd.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://pik.yvedp.cn

[G04] 定义方法
来源：http://zuy.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://qim.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://gbh.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://otr.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://sbu.ppjwa.cn

Java: String greet() { return name; }
来源：http://qul.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zip.jqgfzy.top

Ruby: def greet; @name; end
来源：http://dzy.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://lon.xziqi.cn

[G05] 继承
来源：http://yog.ppjwa.cn

Py:   class Admin(User): pass
来源：http://ujo.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://ugn.xylfe.cn

JS:   class Admin extends User {}
来源：http://uyy.cdnleiting.top

TS:   class Admin extends User {}
来源：http://wip.quarkkingdee.top

Java: class Admin extends User {}
来源：http://txr.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rse.dianchejie.cn

Ruby: class Admin < User; end
来源：http://zzn.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://swq.yfazqb.com

[G06] 重写方法
来源：http://cen.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://unl.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://zah.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://bqc.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://neu.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://mcq.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://clz.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://ezx.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://hai.shangyingyoupin.top

[G07] 调用父类方法
来源：http://azg.yuxming.cn

Py:   super().greet()
来源：http://eal.fktsv.cn

PHP:  parent::greet();
来源：http://pko.bbcook.cn

JS:   super.greet();
来源：http://eem.wangshuangyany.cn

TS:   super.greet();
来源：http://xzd.yangfankeji.com

Java: super.greet();
来源：http://ihv.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ssc.daria6918.cn

Ruby: super
来源：http://wid.yuxming.cn

C#:   base.Greet();
来源：http://vrb.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://sgj.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nsr.cqqwz.cn

PHP:  public static function f() {}
来源：http://ali.andypj.xyz

JS:   static f() {}
来源：http://mxe.cucudq.cn

TS:   static f(): void {}
来源：http://eou.gogol.net.cn

Java: static void f() {}
来源：http://fkk.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qwl.hysaishi.cn

Ruby: def self.f; end
来源：http://niu.yuxming.cn

C#:   public static void F() {}
来源：http://jjp.epnwcf.com

[G09] 接口 / 抽象类
来源：http://efo.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://lug.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://ptj.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://phd.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://aca.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://kbb.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://jyf.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cpj.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://jfl.svipenyu.cn

[G10] 访问控制
来源：http://moa.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://dvm.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://hwy.yvedp.cn

JS:   #private 字段；其余公开
来源：http://hvg.chenjidiqi.icu

TS:   public / protected / private
来源：http://zlx.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://nrp.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nza.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://boj.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://lhs.redwolf501.top

[G11] getter / setter
来源：http://ous.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://xuo.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ldq.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://wia.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://cli.ybcxt.top

Java: public String getName() { return name; }
来源：http://lbl.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://avi.wangdashe.top

Ruby: attr_accessor :name
来源：http://rob.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://whb.gaohongyu789.top

[G12] 对象转字符串
来源：http://suv.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://ijx.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://gqz.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://tlq.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://szr.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://mgd.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://bpn.zycfv.cn

Ruby: def to_s; @name; end
来源：http://wfk.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://psk.quarkkingdee.top

[G13] 判断对象类型
来源：http://tro.yuanzhike.top

Py:   isinstance(u, User)
来源：http://mjp.jinqigufen.top

PHP:  $u instanceof User
来源：http://mid.ivvv.top

JS:   u instanceof User
来源：http://los.epnwcf.com

TS:   u instanceof User
来源：http://pmm.wangshuangyany.cn

Java: u instanceof User
来源：http://afr.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ntu.hcnkem.com

Ruby: u.is_a?(User)
来源：http://fle.cheryme.top

C#:   u is User
来源：http://peb.fzhhl.top

[G14] 数据类 / record
来源：http://rso.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pic.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://paq.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xqa.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://yne.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://czq.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://fwg.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bkn.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://tfi.pengpengdd.cyou

[G15] 枚举
来源：http://gqw.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yln.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://qfl.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eim.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ahf.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://azs.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aez.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://nem.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xqc.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://pne.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tgw.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://zoz.hysaishi.cn

JS:   Object.entries(obj)
来源：http://tbv.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://yze.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kof.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivf.svipenyu.cn

Ruby: obj.instance_variables
来源：http://txo.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://ylj.0kj1m.cn

================================================================================
来源：http://svc.yueranfly.top

H. 异常与错误处理
来源：http://rdc.tarul.cn

================================================================================
来源：http://tvb.ybcxt.top

[H01] try / catch 基础
来源：http://loc.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://guj.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rzs.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jva.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://boe.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nxm.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kmx.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qjm.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cgu.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://biw.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fae.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ysq.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://exn.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gtk.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://inu.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ggy.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://cnj.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kzd.redwolf501.top

[H03] 主动抛出异常
来源：http://odu.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://wap.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cpe.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://xhd.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://fnz.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uvl.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zcz.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zww.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gbu.birdmap.top

[H04] 自定义异常类型
来源：http://spp.havefunace.top

Py:   class MyError(Exception): pass
来源：http://jai.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://adx.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://voo.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://koh.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://hfd.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ger.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://mek.yj20258.top

C#:   class MyException : Exception {}
来源：http://bdm.hfpthk.cn

[H05] 捕获特定类型
来源：http://hli.nwbrower.top

Py:   except ValueError as e:
来源：http://lxz.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://geq.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://eob.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://dkj.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://cre.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ooh.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://sxw.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xll.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://xlw.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://hvg.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kdi.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://ryt.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://yyb.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jjj.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jgv.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://whk.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://gwn.316326.xyz

[H07] 断言
来源：http://aon.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://fil.hywenlv.cn

PHP:  assert($x > 0);
来源：http://eeh.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://zoy.meibo888.top

TS:   console.assert(x > 0);
来源：http://thc.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://jkw.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqp.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hbd.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://zwk.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://rep.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://nan.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwn.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://caf.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqk.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://itb.zdqjudy.top

Go:   err.Error()
来源：http://jsl.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://qjb.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://jya.gotoacloud.top

[H09] 带错误码的异常
来源：http://mxr.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://asy.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vbc.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://haz.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://azf.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ljc.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jgl.ivvv.top

Ruby: raise MyError.new("fail", 500)
来源：http://meg.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lyu.pengpengdd.cyou

[H10] 资源自动释放
来源：http://mso.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vbu.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://obj.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://axn.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ubj.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://krx.haohaochexian.top

Go:   defer f.Close()
来源：http://acy.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kec.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vyq.52xcode.cn

================================================================================
来源：http://sgq.feifeiyinyue.top

I. 正则表达式
来源：http://llf.xziqi.cn

================================================================================
来源：http://spc.yangfankeji.com

[I01] 判断是否匹配
来源：http://fgq.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pnn.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://czs.daria6918.cn

JS:   /\d+/.test(s)
来源：http://ioh.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://gkk.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eaq.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ryw.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://jkd.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://htg.ybcxt.top

[I02] 提取所有匹配
来源：http://nhg.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://bwt.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyc.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ozo.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://yul.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dso.xylfe.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mtx.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://zmj.aibaodan.cn


<!-- 参考信息 -->