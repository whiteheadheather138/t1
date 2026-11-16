代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://mmt.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tqa.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://hav.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://zcc.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jor.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gvt.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://rjm.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://srs.jinqigufen.top

[F09] 获取文件大小
来源：http://sts.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://fdk.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://ysd.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://ruo.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://xvm.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ylu.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kbl.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://lhd.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://pwy.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://rjf.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hgn.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://twm.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ivh.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://cjl.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tyk.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gyx.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vam.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xln.nanxinkj.top

[F11] 复制与移动文件
来源：http://wbk.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://elt.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gmk.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bxq.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmg.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uel.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nmb.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tkg.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nnu.0kj1m.cn

[F12] CSV 读写
来源：http://bwa.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ayn.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yii.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kco.zhoulong.xyz

TS:   // 同上
来源：http://zev.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qvm.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zxs.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uny.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://uhs.yj20258.top

================================================================================
来源：http://ndp.hammf.cn

G. 面向对象
来源：http://wrx.chenlongwang.top

================================================================================
来源：http://kli.316326.xyz

[G01] 定义类
来源：http://erg.pycfn.com

Py:   class User: pass
来源：http://hry.tian-w.cn

PHP:  class User {}
来源：http://rlj.jinqigufen.top

JS:   class User {}
来源：http://dzl.sweek.top

TS:   class User { name: string = ""; }
来源：http://yvy.gzhubu.top

Java: class User {}
来源：http://ghe.mhx1999.top

Go:   type User struct { Name string }
来源：http://hfb.redwolf501.top

Ruby: class User; end
来源：http://gvm.ydjk.org.cn

C#:   class User {}
来源：http://jcz.meibo888.top

[G02] 构造函数
来源：http://cbr.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://dat.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://cfw.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://ojn.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://irb.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://hut.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ctd.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://tzn.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://mlu.chenzaomai.com

[G03] 实例属性
来源：http://ezl.yuxming.cn

Py:   self.name = "x"
来源：http://mym.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://kbh.yuanzhike.top

JS:   this.name = "x";
来源：http://vcp.uphjek.com

TS:   name: string = "x";
来源：http://ull.xuetiantiany.cn

Java: private String name;
来源：http://tik.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sis.gogol.net.cn

Ruby: @name = "x"
来源：http://vir.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://rgo.sxryk.cn

[G04] 定义方法
来源：http://cbh.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://qdw.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://heh.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://jir.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://ysn.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://zvn.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pqw.bbcook.cn

Ruby: def greet; @name; end
来源：http://udi.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://rkb.zdbjq.cn

[G05] 继承
来源：http://zgh.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://ctz.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://qbz.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://bab.hcnkem.com

TS:   class Admin extends User {}
来源：http://dpn.shzxlz.cn

Java: class Admin extends User {}
来源：http://vaj.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://btu.bbcook.cn

Ruby: class Admin < User; end
来源：http://gsa.0kj1m.cn

C#:   class Admin : User {}
来源：http://hlq.aizwys.cn

[G06] 重写方法
来源：http://yqq.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://odu.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dig.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://ror.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://ied.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://vuq.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bds.tanke756.top

Ruby: def greet; "admin"; end
来源：http://xge.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://tbq.havefunace.top

[G07] 调用父类方法
来源：http://hjr.aizwys.cn

Py:   super().greet()
来源：http://pbj.daxiang520.top

PHP:  parent::greet();
来源：http://wxp.fzhhl.top

JS:   super.greet();
来源：http://apr.hnqzz.top

TS:   super.greet();
来源：http://qgc.yj20258888.top

Java: super.greet();
来源：http://zxt.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://plr.xuetiantiany.cn

Ruby: super
来源：http://qae.wangshuangyany.cn

C#:   base.Greet();
来源：http://dvp.ppjwa.cn

[G08] 静态方法与属性
来源：http://obw.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hlg.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://qhl.ybcxt.top

JS:   static f() {}
来源：http://lxk.shuidangran.top

TS:   static f(): void {}
来源：http://dji.hnqzz.top

Java: static void f() {}
来源：http://iky.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pox.0kj1m.cn

Ruby: def self.f; end
来源：http://egx.ydjk.org.cn

C#:   public static void F() {}
来源：http://yro.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://ido.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://fpc.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://rxa.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://dzt.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://xac.tarul.cn

Java: interface Shape { double area(); }
来源：http://ype.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://whd.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vtf.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://lze.svipenyu.cn

[G10] 访问控制
来源：http://rbu.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://kqi.hnxiangtu.top

PHP:  public / protected / private
来源：http://ftp.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://byf.ppjwa.cn

TS:   public / protected / private
来源：http://krz.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://kdj.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rgc.zdqjudy.top

Ruby: public / protected / private
来源：http://nhi.fktsv.cn

C#:   public / protected / private / internal
来源：http://emq.haohaochexian.top

[G11] getter / setter
来源：http://yii.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://emj.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://afi.pycfn.com

JS:   get name() { return this._name; }
来源：http://nqq.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://cox.dashuyun.cn

Java: public String getName() { return name; }
来源：http://uqi.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ote.guowangkeji.top

Ruby: attr_accessor :name
来源：http://hog.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://vfu.wangdashe.top

[G12] 对象转字符串
来源：http://jdf.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://roy.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohe.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://bqy.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://yjw.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://sya.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nhh.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://ldh.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://ndt.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://mnr.gzhubu.top

Py:   isinstance(u, User)
来源：http://hih.xylfe.cn

PHP:  $u instanceof User
来源：http://wtg.jianghu66.top

JS:   u instanceof User
来源：http://apc.shuidangran.top

TS:   u instanceof User
来源：http://ttb.hcnkem.com

Java: u instanceof User
来源：http://eus.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gck.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://rna.yueranfly.top

C#:   u is User
来源：http://lzd.daxiang520.top

[G14] 数据类 / record
来源：http://uqu.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://crk.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://pmy.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ijy.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://cfd.daxiang520.top

Java: record User(String name, int age) {}
来源：http://uli.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://wqn.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tdn.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://mbo.xziqi.cn

[G15] 枚举
来源：http://wce.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://geg.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ooz.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyi.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dbi.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://vde.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbi.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://hwq.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sxh.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://mqc.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tkc.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://elu.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://leq.meibo888.top

TS:   Object.entries(obj)
来源：http://jpo.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mxq.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dka.xinyue.icu

Ruby: obj.instance_variables
来源：http://wof.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dpm.ywan-chungtsiang.top

================================================================================
来源：http://vne.zycfv.cn

H. 异常与错误处理
来源：http://msf.svipenyu.cn

================================================================================
来源：http://ksr.tanke756.top

[H01] try / catch 基础
来源：http://stz.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pjx.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rwz.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yqi.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bpo.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gwh.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://flu.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pkx.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hqx.gzhubu.top

[H02] finally / ensure 收尾
来源：http://tdf.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dyx.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://odk.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dkp.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lmg.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tgj.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wtj.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qvw.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wmg.bbcook.cn

[H03] 主动抛出异常
来源：http://ned.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://sby.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oib.meibo888.top

JS:   throw new Error("错误信息");
来源：http://cyk.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://swk.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pke.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://edo.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rpm.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://ljh.52xcode.cn

[H04] 自定义异常类型
来源：http://mew.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://ybu.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://hkp.cheryme.top

JS:   class MyError extends Error {}
来源：http://npr.ivvv.top

TS:   class MyError extends Error {}
来源：http://qdj.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://vsb.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lqs.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://fjw.fzhhl.top

C#:   class MyException : Exception {}
来源：http://dgq.hfpthk.cn

[H05] 捕获特定类型
来源：http://pfk.jianghu66.top

Py:   except ValueError as e:
来源：http://qng.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eov.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://cbf.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://spg.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://hti.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezv.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://pki.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ghk.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://jvw.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://obh.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://zcy.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://scx.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://ght.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vud.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qnz.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://cod.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://vly.chenlongwang.top

[H07] 断言
来源：http://hbm.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://pes.jianghu66.top

PHP:  assert($x > 0);
来源：http://ujm.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://jmq.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://jzh.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://nww.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tfu.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://ucg.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://cad.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://lhs.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://bhu.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ojv.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://ery.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mln.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tih.uphjek.com

Go:   err.Error()
来源：http://isr.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://xhm.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://aeh.nanxuanxn.top

[H09] 带错误码的异常
来源：http://wnr.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qag.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://niw.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cve.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eqr.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cwn.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://day.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://qhm.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jgn.0kj1m.cn

[H10] 资源自动释放
来源：http://mqi.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rdk.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mwj.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://daj.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lwn.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mru.zhoulong.xyz

Go:   defer f.Close()
来源：http://iaf.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ifh.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ftz.fzhhl.top

================================================================================
来源：http://wqw.bbcook.cn

I. 正则表达式
来源：http://hrj.zhijiandao.cn

================================================================================
来源：http://pui.ydzc1.top

[I01] 判断是否匹配
来源：http://cdo.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mgb.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://cyy.yvedp.cn

JS:   /\d+/.test(s)
来源：http://xni.daxiang520.top

TS:   /\d+/.test(s)
来源：http://jdo.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mkj.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqu.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://ybr.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xaz.316326.xyz

[I02] 提取所有匹配
来源：http://hqj.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://kph.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://abn.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sbx.fanxiaobao.xyz


<!-- 参考信息 -->