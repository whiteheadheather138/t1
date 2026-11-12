代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vrg.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://atp.shuidangran.top

Ruby: Dir.children("dir")
来源：http://mpe.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://uqx.fengsongda.top

[F09] 获取文件大小
来源：http://yna.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://qzx.daxiang520.top

PHP:  filesize("a.txt");
来源：http://cqj.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://sdu.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://uod.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uxd.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mmn.smart0.xyz

Ruby: File.size("a.txt")
来源：http://aex.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://kxf.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://rmz.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jwc.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://drk.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nzl.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://efm.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rfy.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pqt.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://auv.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vgw.snrcjt.cn

[F11] 复制与移动文件
来源：http://yys.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zrk.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ova.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iaa.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yxu.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rec.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://irj.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yym.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lgc.xuetiantiany.cn

[F12] CSV 读写
来源：http://kfn.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nsk.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fci.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dyv.shangyingyoupin.top

TS:   // 同上
来源：http://qwh.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ina.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zhk.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lyf.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lja.hysaishi.cn

================================================================================
来源：http://ocg.snrcjt.cn

G. 面向对象
来源：http://ciz.havefunace.top

================================================================================
来源：http://tsk.ydzc1.top

[G01] 定义类
来源：http://nuj.feifeiyinyue.top

Py:   class User: pass
来源：http://jsh.wangshuangyany.cn

PHP:  class User {}
来源：http://jqg.cheryme.top

JS:   class User {}
来源：http://stg.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://gqh.jiagoushi.top

Java: class User {}
来源：http://zim.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://dcn.zycfv.cn

Ruby: class User; end
来源：http://zjw.smart0.xyz

C#:   class User {}
来源：http://xix.dianchejie.cn

[G02] 构造函数
来源：http://sgz.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://zpx.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://tid.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://rpp.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://gnm.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://ndq.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xle.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://kfo.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://arp.yongpay.top

[G03] 实例属性
来源：http://mnj.yongpay.top

Py:   self.name = "x"
来源：http://qvs.chenlongwang.top

PHP:  public string $name = "x";
来源：http://uyx.yangfankeji.com

JS:   this.name = "x";
来源：http://lls.bjfxy.top

TS:   name: string = "x";
来源：http://fbz.fktsv.cn

Java: private String name;
来源：http://dnj.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uoe.nanxinkj.top

Ruby: @name = "x"
来源：http://wyc.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ovr.epnwcf.com

[G04] 定义方法
来源：http://leu.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://gso.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xnv.andypj.xyz

JS:   greet() { return this.name; }
来源：http://xll.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://jju.zhijiandao.cn

Java: String greet() { return name; }
来源：http://sii.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ait.c1oappe.top

Ruby: def greet; @name; end
来源：http://nov.redwolf501.top

C#:   public string Greet() => Name;
来源：http://rjx.wangshuangyany.cn

[G05] 继承
来源：http://ord.fzhhl.top

Py:   class Admin(User): pass
来源：http://tsp.yfazqb.com

PHP:  class Admin extends User {}
来源：http://cnw.52xcode.cn

JS:   class Admin extends User {}
来源：http://tgw.chenlongwang.top

TS:   class Admin extends User {}
来源：http://adk.guannengcc.top

Java: class Admin extends User {}
来源：http://gqz.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kbf.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://uan.yj202588.top

C#:   class Admin : User {}
来源：http://sli.ivvv.top

[G06] 重写方法
来源：http://nsy.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://bca.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dnb.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://noy.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://ypy.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://tjb.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ybc.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://pxe.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://bps.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://duu.ctjpmb.com

Py:   super().greet()
来源：http://cpm.hammf.cn

PHP:  parent::greet();
来源：http://qnd.c1oappe.top

JS:   super.greet();
来源：http://izf.sysykeji.top

TS:   super.greet();
来源：http://pek.chenjidiqi.icu

Java: super.greet();
来源：http://qlk.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aug.iojbl.cn

Ruby: super
来源：http://feq.hesvh.cn

C#:   base.Greet();
来源：http://czm.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://epw.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wll.wangdashe.top

PHP:  public static function f() {}
来源：http://gva.cashguo.top

JS:   static f() {}
来源：http://wxf.hammf.cn

TS:   static f(): void {}
来源：http://kdw.zhengqikj.top

Java: static void f() {}
来源：http://kqg.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://epx.xuetiantiany.cn

Ruby: def self.f; end
来源：http://uwm.svipenyu.cn

C#:   public static void F() {}
来源：http://zsp.aizwys.cn

[G09] 接口 / 抽象类
来源：http://mcb.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://omp.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://btm.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rip.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://pdp.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://udq.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://vjk.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tpj.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://fur.havefunace.top

[G10] 访问控制
来源：http://mzx.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://lmr.gotoacloud.top

PHP:  public / protected / private
来源：http://jef.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://dyu.guowangkeji.top

TS:   public / protected / private
来源：http://efv.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://xgz.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mss.sweek.top

Ruby: public / protected / private
来源：http://ypy.jianghu66.top

C#:   public / protected / private / internal
来源：http://vtb.sxryk.cn

[G11] getter / setter
来源：http://idz.52xcode.cn

Py:   @property 与 @x.setter
来源：http://dyx.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uuz.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://irl.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://skx.tianlin.xyz

Java: public String getName() { return name; }
来源：http://kgg.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cvz.yj20258888.top

Ruby: attr_accessor :name
来源：http://jbl.yj202588.top

C#:   public string Name { get; set; }
来源：http://cvl.bbcook.cn

[G12] 对象转字符串
来源：http://hor.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://hdu.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xrt.wangdashe.top

JS:   toString() { return this.name; }
来源：http://ers.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://eeu.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://xly.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cpi.uphjek.com

Ruby: def to_s; @name; end
来源：http://amt.cashguo.top

C#:   public override string ToString() => Name;
来源：http://kvk.hnxiangtu.top

[G13] 判断对象类型
来源：http://gbi.mhx1999.top

Py:   isinstance(u, User)
来源：http://luo.yuanzhike.top

PHP:  $u instanceof User
来源：http://bal.xinyue.icu

JS:   u instanceof User
来源：http://dsz.ctjpmb.com

TS:   u instanceof User
来源：http://qvu.cheryme.top

Java: u instanceof User
来源：http://zhd.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mua.jianghu66.top

Ruby: u.is_a?(User)
来源：http://pas.shzxlz.cn

C#:   u is User
来源：http://quq.yueranfly.top

[G14] 数据类 / record
来源：http://eml.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wpe.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://xzg.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://eet.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://sbe.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://uvf.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://yhb.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ivk.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://oil.tarul.cn

[G15] 枚举
来源：http://upb.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wut.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kgi.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jnw.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lsk.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://vdo.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vqn.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://wjb.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pgr.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://rbo.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://foe.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://ivt.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://jhd.52xcode.cn

TS:   Object.entries(obj)
来源：http://qrt.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gwm.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://cdb.tarul.cn

Ruby: obj.instance_variables
来源：http://gua.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://rqv.mhx1999.top

================================================================================
来源：http://gke.nanxuanxn.top

H. 异常与错误处理
来源：http://wug.feifeiyinyue.top

================================================================================
来源：http://oey.epnwcf.com

[H01] try / catch 基础
来源：http://jps.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://omp.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fcm.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ecm.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ioy.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gny.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hkc.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yvq.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nob.vehdjk.com

[H02] finally / ensure 收尾
来源：http://osh.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://gvp.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fdq.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vkt.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mbw.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dit.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jir.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tjr.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sal.xylfe.cn

[H03] 主动抛出异常
来源：http://ysx.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://wfe.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://faj.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://wow.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://wts.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aaq.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fkq.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pnf.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://shx.gotoacloud.top

[H04] 自定义异常类型
来源：http://giz.cashguo.top

Py:   class MyError(Exception): pass
来源：http://fhj.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://ytc.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://kme.uphjek.com

TS:   class MyError extends Error {}
来源：http://gge.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://umy.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lgr.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://zyf.ivvv.top

C#:   class MyException : Exception {}
来源：http://gqf.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://umb.c1oappe.top

Py:   except ValueError as e:
来源：http://bvg.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xiu.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://uji.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://qtj.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://xdv.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qiw.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://jsx.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iuu.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://pby.jianghu66.top

Py:   value = d.get("k") or default
来源：http://hte.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sxe.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://tnw.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ano.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dvc.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://afu.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://ibj.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://nve.wangdashe.top

[H07] 断言
来源：http://uie.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://svx.haohaochexian.top

PHP:  assert($x > 0);
来源：http://lrf.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://wfn.hcnkem.com

TS:   console.assert(x > 0);
来源：http://dnk.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://miq.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sze.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://kej.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://pct.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://toh.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://eif.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://win.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://znn.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qln.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qhq.ydzc1.top

Go:   err.Error()
来源：http://svw.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://pbb.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ket.gotoacloud.top

[H09] 带错误码的异常
来源：http://xjf.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://irz.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nkn.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qke.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aqk.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uum.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://plq.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://qrm.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tqc.0kj1m.cn

[H10] 资源自动释放
来源：http://vlj.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vrp.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://siv.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://geq.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://umz.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ovd.epnwcf.com

Go:   defer f.Close()
来源：http://mul.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jyk.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ygm.pycfn.com

================================================================================
来源：http://hjd.jqgufenzy.top

I. 正则表达式
来源：http://uiw.fktsv.cn

================================================================================
来源：http://kor.jyoumei.cn

[I01] 判断是否匹配
来源：http://bou.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vfu.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ufg.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://jzl.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://eqk.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oey.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zff.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://rxn.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://khq.yangfankeji.com

[I02] 提取所有匹配
来源：http://mwk.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://xou.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lcm.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wex.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://uut.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cqh.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kly.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://rtx.yj202588.top


<!-- 参考信息 -->