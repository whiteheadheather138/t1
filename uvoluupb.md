代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wlw.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://usc.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yon.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://won.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bml.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lcq.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zje.tianlin.xyz

[F08] 遍历目录
来源：http://jhm.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zhl.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hcr.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://tfh.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://ach.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uuk.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://efm.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://zib.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://swx.haohaochexian.top

[F09] 获取文件大小
来源：http://hwj.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://qlq.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://qtx.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://opd.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://hui.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ezf.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://izc.tarul.cn

Ruby: File.size("a.txt")
来源：http://dnx.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://yeu.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://jkd.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jbs.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tgt.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mre.hnqzz.top

TS:   path.extname("a.txt")
来源：http://non.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tpz.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jyh.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hqa.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pei.jinqigfzy.top

[F11] 复制与移动文件
来源：http://rus.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dki.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jwr.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gal.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dog.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://stp.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rjj.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vpr.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fpw.snrcjt.cn

[F12] CSV 读写
来源：http://aux.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lju.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxm.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cec.316326.xyz

TS:   // 同上
来源：http://fwz.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mht.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://brn.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rjo.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://uoo.sxryk.cn

================================================================================
来源：http://rrc.fzhhl.top

G. 面向对象
来源：http://dld.cqqwz.cn

================================================================================
来源：http://wwj.yj20258888.top

[G01] 定义类
来源：http://qut.fzhhl.top

Py:   class User: pass
来源：http://tla.ydjk.org.cn

PHP:  class User {}
来源：http://gpr.andypj.xyz

JS:   class User {}
来源：http://cgu.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://jru.epnwcf.com

Java: class User {}
来源：http://ysy.ydzc1.top

Go:   type User struct { Name string }
来源：http://jmn.yj20258888.top

Ruby: class User; end
来源：http://sme.hnqzz.top

C#:   class User {}
来源：http://rtw.ydjk.org.cn

[G02] 构造函数
来源：http://lui.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://yqr.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://oau.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://gob.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://rwl.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://pnq.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gxk.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://tsa.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://ndc.yuxming.cn

[G03] 实例属性
来源：http://jbf.zhijiandao.cn

Py:   self.name = "x"
来源：http://zrq.fengsongda.top

PHP:  public string $name = "x";
来源：http://ovg.zhongyouzk.top

JS:   this.name = "x";
来源：http://xlr.zhoulong.xyz

TS:   name: string = "x";
来源：http://umq.hywenlv.cn

Java: private String name;
来源：http://kht.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyg.svipenyu.cn

Ruby: @name = "x"
来源：http://yzy.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://wwx.zhixingplan.top

[G04] 定义方法
来源：http://pib.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://iot.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://iai.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://gqy.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://zjv.jinqigufen.top

Java: String greet() { return name; }
来源：http://pkr.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cjw.hysaishi.cn

Ruby: def greet; @name; end
来源：http://cbv.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://vfa.sweek.top

[G05] 继承
来源：http://noo.svipenyu.cn

Py:   class Admin(User): pass
来源：http://uiq.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://gze.havefunace.top

JS:   class Admin extends User {}
来源：http://rjt.tian-w.cn

TS:   class Admin extends User {}
来源：http://eqg.andypj.xyz

Java: class Admin extends User {}
来源：http://tli.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qxk.daxiang520.top

Ruby: class Admin < User; end
来源：http://rcs.yfazqb.com

C#:   class Admin : User {}
来源：http://ncy.fehbvm.com

[G06] 重写方法
来源：http://aqm.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://yss.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nzg.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://kbu.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://usp.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://gui.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pvw.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://ndb.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://gkw.tian-w.cn

[G07] 调用父类方法
来源：http://gkf.jinghuilouyu.cn

Py:   super().greet()
来源：http://jns.gogol.net.cn

PHP:  parent::greet();
来源：http://oru.bbcook.cn

JS:   super.greet();
来源：http://loy.havefunace.top

TS:   super.greet();
来源：http://oxb.gaohongyu789.top

Java: super.greet();
来源：http://sis.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mdh.pengpengdd.cyou

Ruby: super
来源：http://rkt.9152youxi.cn

C#:   base.Greet();
来源：http://jxi.yuanzhike.top

[G08] 静态方法与属性
来源：http://lza.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wjs.nanxinkj.top

PHP:  public static function f() {}
来源：http://tsc.yonumen.top

JS:   static f() {}
来源：http://nhi.52xcode.cn

TS:   static f(): void {}
来源：http://une.daxiang520.top

Java: static void f() {}
来源：http://ccc.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jyu.yongpay.top

Ruby: def self.f; end
来源：http://ptr.xziqi.cn

C#:   public static void F() {}
来源：http://tku.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://uul.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://iqz.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://ujp.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mhg.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://ihv.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://kcx.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://daz.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hyp.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://oka.yj202588.top

[G10] 访问控制
来源：http://tuk.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://gkq.hysaishi.cn

PHP:  public / protected / private
来源：http://hyv.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://bes.birdmap.top

TS:   public / protected / private
来源：http://hrj.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://xgp.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zna.andypj.xyz

Ruby: public / protected / private
来源：http://bpo.jyoumei.cn

C#:   public / protected / private / internal
来源：http://lnu.kuanghao11.cn

[G11] getter / setter
来源：http://myp.ydzc1.top

Py:   @property 与 @x.setter
来源：http://zhb.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dxf.zycfv.cn

JS:   get name() { return this._name; }
来源：http://ewu.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://vsp.mhx1999.top

Java: public String getName() { return name; }
来源：http://kvp.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vfx.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://hvg.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://sdv.hywenlv.cn

[G12] 对象转字符串
来源：http://kny.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://spd.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qdp.sxryk.cn

JS:   toString() { return this.name; }
来源：http://xsc.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://sta.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://fuo.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nmg.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://agj.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://mgi.yvedp.cn

[G13] 判断对象类型
来源：http://mjs.ehwqpu.com

Py:   isinstance(u, User)
来源：http://krb.sweek.top

PHP:  $u instanceof User
来源：http://jic.ctjpmb.com

JS:   u instanceof User
来源：http://wcm.wangdashe.top

TS:   u instanceof User
来源：http://wmz.ydjk.org.cn

Java: u instanceof User
来源：http://glf.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kdk.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://xuj.cdnleiting.top

C#:   u is User
来源：http://axf.c1oappe.top

[G14] 数据类 / record
来源：http://wzf.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zzk.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://ckw.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://bas.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://pwc.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://uuc.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://ukv.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aij.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://xdy.hcnkem.com

[G15] 枚举
来源：http://qnb.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://paj.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dew.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wro.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kth.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://gys.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lgw.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://fjl.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wps.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://ubt.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qkr.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://tod.ctjpmb.com

JS:   Object.entries(obj)
来源：http://evi.jiagoushi.top

TS:   Object.entries(obj)
来源：http://huk.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://voa.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zen.tanke756.top

Ruby: obj.instance_variables
来源：http://ofv.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://cfw.ivvv.top

================================================================================
来源：http://ahj.xylfe.cn

H. 异常与错误处理
来源：http://fle.epnwcf.com

================================================================================
来源：http://vpj.haohaochexian.top

[H01] try / catch 基础
来源：http://vij.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kcw.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jrn.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://onv.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qlh.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nnr.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eac.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gyt.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lvw.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://low.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yoc.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://buz.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://evj.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://qqr.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lkm.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ezv.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oms.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ngk.yanxiufei.cn

[H03] 主动抛出异常
来源：http://bcv.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://pmp.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://joe.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://kbj.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://uvn.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dxi.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://prj.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kcb.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://ibz.vqdsnc.cn

[H04] 自定义异常类型
来源：http://ywp.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://dum.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://yuv.xylfe.cn

JS:   class MyError extends Error {}
来源：http://sup.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://lxi.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://ptk.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fkk.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://tbb.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://ijt.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://gmr.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://vhe.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cnj.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://dxd.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://pvl.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://cvd.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gmz.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://jyt.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nna.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://vxv.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://lvz.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://vlz.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rmg.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qtr.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ban.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://igf.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://byc.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://yjj.mhx1999.top

[H07] 断言
来源：http://wid.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://bjh.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://fag.iojbl.cn

JS:   console.assert(x > 0);
来源：http://ehr.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://sbk.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://uvy.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oyh.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://csv.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://bwu.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://kzg.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ywc.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vua.jiagoushi.top

JS:   e.message;  e.stack
来源：http://tan.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://nqx.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qgu.yj20258888.top

Go:   err.Error()
来源：http://yaz.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://ttg.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://iug.dashuyun.cn

[H09] 带错误码的异常
来源：http://gex.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://csj.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://peu.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gbf.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ier.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uij.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccy.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rnv.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jfj.chenlongwang.top

[H10] 资源自动释放
来源：http://nic.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ezj.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkr.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://umz.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wnk.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ipi.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://koc.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pdi.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xml.cheryme.top

================================================================================
来源：http://sjq.cheryme.top

I. 正则表达式
来源：http://lyq.ctjpmb.com

================================================================================
来源：http://lxs.cheryme.top

[I01] 判断是否匹配
来源：http://opx.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tmt.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dgj.xylfe.cn

JS:   /\d+/.test(s)
来源：http://ixt.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://pqu.zhixingplan.top


<!-- 参考信息 -->