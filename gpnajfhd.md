代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bpb.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://end.xylfe.cn

Ruby: Dir.children("dir")
来源：http://mub.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://bvg.jlsjyb.cn

[F09] 获取文件大小
来源：http://tmv.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://opd.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://qgn.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://rcv.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://opc.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gsn.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lzf.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://xff.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://yne.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://clr.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wss.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nxu.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://twm.uphjek.com

TS:   path.extname("a.txt")
来源：http://rju.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ikf.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mkr.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hsc.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yhr.tianlin.xyz

[F11] 复制与移动文件
来源：http://wsy.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aws.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gll.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xum.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tik.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uru.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztn.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfx.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yic.hfpthk.cn

[F12] CSV 读写
来源：http://pfp.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://grw.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rmd.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kky.tarul.cn

TS:   // 同上
来源：http://qjs.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cgt.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rkc.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ozw.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yhv.hongshengwenyu.top

================================================================================
来源：http://dao.xuanzx.com

G. 面向对象
来源：http://blw.sxryk.cn

================================================================================
来源：http://ukm.cqqwz.cn

[G01] 定义类
来源：http://ucj.feifeiyinyue.top

Py:   class User: pass
来源：http://zwy.hysaishi.cn

PHP:  class User {}
来源：http://jsb.haohaochexian.top

JS:   class User {}
来源：http://tkn.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://fcd.jlsjyb.cn

Java: class User {}
来源：http://wir.9152youxi.cn

Go:   type User struct { Name string }
来源：http://gpj.chenlongwang.top

Ruby: class User; end
来源：http://jlg.fanxiaobao.xyz

C#:   class User {}
来源：http://sfg.zdqjudy.top

[G02] 构造函数
来源：http://ufv.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://yft.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://rhw.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ckc.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://ltn.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://pdl.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tbl.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://lsh.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://wio.chenjidiqi.icu

[G03] 实例属性
来源：http://yar.havefunace.top

Py:   self.name = "x"
来源：http://mvi.yfazqb.com

PHP:  public string $name = "x";
来源：http://ydd.aizwys.cn

JS:   this.name = "x";
来源：http://xrv.shangyingyoupin.top

TS:   name: string = "x";
来源：http://kgn.hnxiangtu.top

Java: private String name;
来源：http://avr.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xqb.nwbrower.top

Ruby: @name = "x"
来源：http://tse.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://rfv.cucudq.cn

[G04] 定义方法
来源：http://wxl.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://dcy.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://knx.sweek.top

JS:   greet() { return this.name; }
来源：http://xqc.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://jzo.jiagoushi.top

Java: String greet() { return name; }
来源：http://zff.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mzv.fengsongda.top

Ruby: def greet; @name; end
来源：http://bfx.fktsv.cn

C#:   public string Greet() => Name;
来源：http://xbv.uphjek.com

[G05] 继承
来源：http://pka.hcnkem.com

Py:   class Admin(User): pass
来源：http://rrh.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://vto.pycfn.com

JS:   class Admin extends User {}
来源：http://dyq.pycfn.com

TS:   class Admin extends User {}
来源：http://cfi.sufxvd.cn

Java: class Admin extends User {}
来源：http://ini.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cmu.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://uop.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://eyd.nanxuanxn.top

[G06] 重写方法
来源：http://rwg.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://xrq.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tbz.ivvv.top

JS:   greet() { return "admin"; }
来源：http://acz.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://zwu.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://ots.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nun.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://jqy.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://qva.tian-w.cn

[G07] 调用父类方法
来源：http://jml.bbcook.cn

Py:   super().greet()
来源：http://vzm.jyoumei.cn

PHP:  parent::greet();
来源：http://iek.kuanghao11.cn

JS:   super.greet();
来源：http://rzy.chenjidiqi.icu

TS:   super.greet();
来源：http://pua.svipenyu.cn

Java: super.greet();
来源：http://iyu.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fes.quarkkingdee.top

Ruby: super
来源：http://lji.tarul.cn

C#:   base.Greet();
来源：http://lag.xziqi.cn

[G08] 静态方法与属性
来源：http://eho.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xqg.guowangkeji.top

PHP:  public static function f() {}
来源：http://yvw.nwbrower.top

JS:   static f() {}
来源：http://yvs.haohaochexian.top

TS:   static f(): void {}
来源：http://vhk.ybcxt.top

Java: static void f() {}
来源：http://uwi.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fhk.52xcode.cn

Ruby: def self.f; end
来源：http://dzs.vehdjk.com

C#:   public static void F() {}
来源：http://rca.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://lqp.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://vjn.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://euk.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mnp.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://cad.bbcook.cn

Java: interface Shape { double area(); }
来源：http://zsd.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://byo.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kmv.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://ufm.shanyushiyangtech.top

[G10] 访问控制
来源：http://rvq.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://jqs.yanxiufei.cn

PHP:  public / protected / private
来源：http://zrg.xinyue.icu

JS:   #private 字段；其余公开
来源：http://zbk.gotoacloud.top

TS:   public / protected / private
来源：http://baz.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://wdn.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ppw.xziqi.cn

Ruby: public / protected / private
来源：http://lxs.bbcook.cn

C#:   public / protected / private / internal
来源：http://ufe.yj202588.top

[G11] getter / setter
来源：http://apq.andypj.xyz

Py:   @property 与 @x.setter
来源：http://obn.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zsv.xuanzx.com

JS:   get name() { return this._name; }
来源：http://ssx.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://rwt.snrcjt.cn

Java: public String getName() { return name; }
来源：http://lxm.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uhm.hcnkem.com

Ruby: attr_accessor :name
来源：http://izl.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://qyu.ydjk.org.cn

[G12] 对象转字符串
来源：http://oxr.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://tra.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xyx.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://jjy.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://fgw.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://ouj.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://wre.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://eko.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://ncy.sjlbkw.cn

[G13] 判断对象类型
来源：http://kxj.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://ycr.bjfxy.top

PHP:  $u instanceof User
来源：http://bvd.zhiwuduotai.top

JS:   u instanceof User
来源：http://bav.daxiang520.top

TS:   u instanceof User
来源：http://ccx.tianlin.xyz

Java: u instanceof User
来源：http://emy.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tue.cashguo.top

Ruby: u.is_a?(User)
来源：http://mcr.gotoacloud.top

C#:   u is User
来源：http://kbg.nanxuanxn.top

[G14] 数据类 / record
来源：http://kzv.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ywe.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://kyl.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ktw.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://dgu.yonumen.top

Java: record User(String name, int age) {}
来源：http://ark.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://cvs.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tep.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://hvo.zhixingplan.top

[G15] 枚举
来源：http://rxf.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtx.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kco.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vdy.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mav.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://vkb.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lax.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://jxf.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yvf.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://tsf.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uci.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://cjg.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://eue.hywenlv.cn

TS:   Object.entries(obj)
来源：http://yxd.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ngk.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aql.ybcxt.top

Ruby: obj.instance_variables
来源：http://gjz.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://sht.wangshuangyany.cn

================================================================================
来源：http://fdh.xinyue.icu

H. 异常与错误处理
来源：http://fqr.xuanzx.com

================================================================================
来源：http://ies.9152youxi.cn

[H01] try / catch 基础
来源：http://gdd.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vzv.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sie.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kvt.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wcm.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fpe.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gzq.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xhe.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xze.birdmap.top

[H02] finally / ensure 收尾
来源：http://fcl.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://ubo.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://rmi.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dyj.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aqn.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://hau.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwg.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kss.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gjx.yonumen.top

[H03] 主动抛出异常
来源：http://ijc.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://nvx.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tsj.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://cwh.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://uer.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qkp.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gor.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xue.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://rhk.yvedp.cn

[H04] 自定义异常类型
来源：http://nrm.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://chb.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wyg.daxiang520.top

JS:   class MyError extends Error {}
来源：http://nrh.birdmap.top

TS:   class MyError extends Error {}
来源：http://qbp.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ljx.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://frz.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://zrd.cashguo.top

C#:   class MyException : Exception {}
来源：http://erk.snrcjt.cn

[H05] 捕获特定类型
来源：http://bun.zhoulong.xyz

Py:   except ValueError as e:
来源：http://qzu.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tcb.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ykj.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://hwg.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://fqd.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://isk.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://bvn.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxo.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://hwo.fzhhl.top

Py:   value = d.get("k") or default
来源：http://yfw.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://xjg.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vly.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ndt.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gai.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qci.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://nbm.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://zca.sufxvd.cn

[H07] 断言
来源：http://kie.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://zpu.gzhubu.top

PHP:  assert($x > 0);
来源：http://sav.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://mfx.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://jdi.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://fhs.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qcv.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://rko.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://ncp.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://yep.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://jat.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sfw.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://jnx.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bbk.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://iki.zhixingplan.top

Go:   err.Error()
来源：http://qum.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://zca.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://tha.jqgfzy.top

[H09] 带错误码的异常
来源：http://vqj.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rbf.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://irw.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://btg.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://suf.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fyr.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uri.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mrz.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ttm.jqgfzy.top

[H10] 资源自动释放
来源：http://geh.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lgp.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jkt.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://czt.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sbg.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gei.chenlongwang.top

Go:   defer f.Close()
来源：http://xpn.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yrs.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://csu.ehwqpu.com

================================================================================
来源：http://jun.nanxinkj.top

I. 正则表达式
来源：http://flp.xziqi.cn

================================================================================
来源：http://fzq.fehbvm.com

[I01] 判断是否匹配
来源：http://gww.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nyo.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://kvr.vehdjk.com

JS:   /\d+/.test(s)
来源：http://gtx.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://dvg.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xra.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uxu.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://xjp.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qhr.aizwys.cn

[I02] 提取所有匹配
来源：http://dso.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://etm.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ghx.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eci.cashguo.top

TS:   s.match(/\d+/g)
来源：http://mrd.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hym.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zfh.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://eck.vehdjk.com


<!-- 参考信息 -->