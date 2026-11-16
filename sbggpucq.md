代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ldq.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ktx.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://ric.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://ukx.quarkkingdee.top

[F09] 获取文件大小
来源：http://udl.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://zna.yueranfly.top

PHP:  filesize("a.txt");
来源：http://dig.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://rgx.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://snr.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kpm.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bfh.sxryk.cn

Ruby: File.size("a.txt")
来源：http://ilp.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://hdr.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://kap.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://efo.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gvg.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qut.shuidangran.top

TS:   path.extname("a.txt")
来源：http://oud.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxy.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ejg.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hke.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://osf.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://kxq.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yyj.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zbi.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mue.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmv.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rgj.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bnw.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ard.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gcl.snrcjt.cn

[F12] CSV 读写
来源：http://fkf.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vol.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lwe.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zen.hongshengwenyu.top

TS:   // 同上
来源：http://gsp.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jsd.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cxf.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dqj.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ltt.zdqjudy.top

================================================================================
来源：http://wao.nanxuanxn.top

G. 面向对象
来源：http://jrl.smart0.xyz

================================================================================
来源：http://gba.dianchejie.cn

[G01] 定义类
来源：http://tzf.hnxiangtu.top

Py:   class User: pass
来源：http://mjf.ppjwa.cn

PHP:  class User {}
来源：http://rtb.jqgfzy.top

JS:   class User {}
来源：http://osx.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://twj.chenzaomai.com

Java: class User {}
来源：http://zwp.yj202588.top

Go:   type User struct { Name string }
来源：http://ejg.jinghuilouyu.cn

Ruby: class User; end
来源：http://yom.tanke756.top

C#:   class User {}
来源：http://hpa.cucudq.cn

[G02] 构造函数
来源：http://rgg.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://vkb.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://tva.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://vfu.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://hgu.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://bvj.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://emk.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://eom.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://auz.nanxuanxn.top

[G03] 实例属性
来源：http://jim.dianchejie.cn

Py:   self.name = "x"
来源：http://wki.gzhubu.top

PHP:  public string $name = "x";
来源：http://wle.guannengcc.top

JS:   this.name = "x";
来源：http://yyv.ydzc1.top

TS:   name: string = "x";
来源：http://cwt.yongpay.top

Java: private String name;
来源：http://oov.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zfh.yueranfly.top

Ruby: @name = "x"
来源：http://owz.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://yup.kuanghao11.cn

[G04] 定义方法
来源：http://xky.sxryk.cn

Py:   def greet(self): return self.name
来源：http://uah.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vlp.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://cnl.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://cpw.sjlbkw.cn

Java: String greet() { return name; }
来源：http://lvq.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lnw.yj20258.top

Ruby: def greet; @name; end
来源：http://qpb.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://pod.yuanzhike.top

[G05] 继承
来源：http://zjs.jiagoushi.top

Py:   class Admin(User): pass
来源：http://gri.havefunace.top

PHP:  class Admin extends User {}
来源：http://dwo.chenlongwang.top

JS:   class Admin extends User {}
来源：http://ixl.chenzaomai.com

TS:   class Admin extends User {}
来源：http://nkh.nanxinkj.top

Java: class Admin extends User {}
来源：http://onx.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://egt.andypj.xyz

Ruby: class Admin < User; end
来源：http://yru.nanxuanxn.top

C#:   class Admin : User {}
来源：http://nwz.cucudq.cn

[G06] 重写方法
来源：http://rlc.316326.xyz

Py:   def greet(self): return "admin"
来源：http://ogm.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pzk.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://lpl.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://rrt.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://wdr.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wkq.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://ffi.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://rsk.chenlongwang.top

[G07] 调用父类方法
来源：http://kug.vehdjk.com

Py:   super().greet()
来源：http://lxh.shzxlz.cn

PHP:  parent::greet();
来源：http://zvv.kuanghao11.cn

JS:   super.greet();
来源：http://hzr.gaohongyu789.top

TS:   super.greet();
来源：http://hal.chenlongwang.top

Java: super.greet();
来源：http://arr.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ztq.yangfankeji.com

Ruby: super
来源：http://gjw.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://bul.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://epd.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fsu.tian-w.cn

PHP:  public static function f() {}
来源：http://xiv.wangshuangyany.cn

JS:   static f() {}
来源：http://eol.gaohongyu789.top

TS:   static f(): void {}
来源：http://njp.hcnkem.com

Java: static void f() {}
来源：http://qsd.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iof.quarkkingdee.top

Ruby: def self.f; end
来源：http://szj.ydzc1.top

C#:   public static void F() {}
来源：http://fqg.hnqzz.top

[G09] 接口 / 抽象类
来源：http://iro.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://mka.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://fbq.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://sza.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://mmx.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://urw.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://hvf.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fnw.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://jnm.gogol.net.cn

[G10] 访问控制
来源：http://iyp.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://gfc.fzhhl.top

PHP:  public / protected / private
来源：http://utt.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://qdd.yangfankeji.com

TS:   public / protected / private
来源：http://ryg.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://zuo.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wgc.aizwys.cn

Ruby: public / protected / private
来源：http://pdf.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://ksi.jiagoushi.top

[G11] getter / setter
来源：http://vcf.redwolf501.top

Py:   @property 与 @x.setter
来源：http://ykr.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://njd.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://yeq.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://uzf.birdmap.top

Java: public String getName() { return name; }
来源：http://ffq.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://kjn.birdmap.top

Ruby: attr_accessor :name
来源：http://vue.xuanzx.com

C#:   public string Name { get; set; }
来源：http://ohb.9152youxi.cn

[G12] 对象转字符串
来源：http://tbq.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://ejw.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://set.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://mcb.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://ctt.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://moa.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://bha.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://pij.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://dhp.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://yqy.dashuyun.cn

Py:   isinstance(u, User)
来源：http://oaj.dianchejie.cn

PHP:  $u instanceof User
来源：http://ywi.bbcook.cn

JS:   u instanceof User
来源：http://lwk.dashuyun.cn

TS:   u instanceof User
来源：http://won.tianlin.xyz

Java: u instanceof User
来源：http://vvz.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fxy.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://msd.jinqigufen.top

C#:   u is User
来源：http://csl.jqgufenzy.top

[G14] 数据类 / record
来源：http://ryz.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hui.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://byg.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hsu.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://zgt.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://tnn.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://hjh.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mgz.birdmap.top

C#:   record User(string Name, int Age);
来源：http://bxk.zdqjudy.top

[G15] 枚举
来源：http://wzk.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kae.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wwo.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vph.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ioa.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://cho.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dep.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://tai.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zer.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://lxb.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ffj.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://fsk.zhixingplan.top

JS:   Object.entries(obj)
来源：http://bxg.shuidangran.top

TS:   Object.entries(obj)
来源：http://sly.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cug.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vvh.hesvh.cn

Ruby: obj.instance_variables
来源：http://ybd.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://xpl.chenzaomai.com

================================================================================
来源：http://yui.cashguo.top

H. 异常与错误处理
来源：http://nla.gogol.net.cn

================================================================================
来源：http://qqr.bbcook.cn

[H01] try / catch 基础
来源：http://lhc.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zgo.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gos.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ezw.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hfy.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fcv.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zug.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nhc.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ehh.sysykeji.top

[H02] finally / ensure 收尾
来源：http://qpy.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ocr.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bbq.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tmz.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ibz.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://mtq.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sml.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yer.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bci.bbcook.cn

[H03] 主动抛出异常
来源：http://lkp.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://wwi.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wli.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://tdy.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://ohc.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wuo.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vgq.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pel.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://ngo.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://hhx.yongpay.top

Py:   class MyError(Exception): pass
来源：http://lqw.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://eyi.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://lsh.xziqi.cn

TS:   class MyError extends Error {}
来源：http://kft.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://dhm.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ran.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://ztz.yj20258.top

C#:   class MyException : Exception {}
来源：http://rqz.tanke756.top

[H05] 捕获特定类型
来源：http://ehx.daria6918.cn

Py:   except ValueError as e:
来源：http://vqj.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kwz.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://jdi.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://csf.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://god.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://trl.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://wew.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xjc.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://xpm.hesvh.cn

Py:   value = d.get("k") or default
来源：http://ldt.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://kme.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jlg.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://vvk.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://grz.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ujs.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://npx.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://fvw.jinqigufen.top

[H07] 断言
来源：http://xyj.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://rxm.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://eob.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://meq.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://tvo.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://xuo.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yea.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://vps.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://uiz.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://tla.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://rhy.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://khk.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://que.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qbr.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yyj.xinyue.icu

Go:   err.Error()
来源：http://rje.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://yfd.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://gew.sysykeji.top

[H09] 带错误码的异常
来源：http://wob.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hrt.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ika.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dlf.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dvi.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yju.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tka.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdg.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yeu.chenlongwang.top

[H10] 资源自动释放
来源：http://wnz.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ccw.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://epp.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kth.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uik.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fob.chenlongwang.top

Go:   defer f.Close()
来源：http://jgh.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zay.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fyk.sxryk.cn

================================================================================
来源：http://poa.ydjk.org.cn

I. 正则表达式
来源：http://fjp.shuidangran.top

================================================================================
来源：http://nie.iojbl.cn

[I01] 判断是否匹配
来源：http://jhv.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://emy.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fet.ybcxt.top

JS:   /\d+/.test(s)
来源：http://yam.cheryme.top

TS:   /\d+/.test(s)
来源：http://ypn.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sji.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xii.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://wpd.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uja.epnwcf.com

[I02] 提取所有匹配
来源：http://tar.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://cnf.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cds.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zft.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://rrv.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mzg.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pek.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://wlp.pengpengdd.cyou


<!-- 参考信息 -->