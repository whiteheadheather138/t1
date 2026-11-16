代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://kzu.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xyk.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://rtp.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://ttl.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mdc.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zyk.daxiang520.top

Ruby: Dir.children("dir")
来源：http://vka.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://iqn.jiagoushi.top

[F09] 获取文件大小
来源：http://dmz.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://tzr.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://jwe.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://vqz.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://fjn.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ksd.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oxi.hnqzz.top

Ruby: File.size("a.txt")
来源：http://ktt.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://bmx.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://ixf.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vrk.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://abl.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mca.gzhubu.top

TS:   path.extname("a.txt")
来源：http://pcf.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yvr.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xop.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xna.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gcf.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://dqs.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ihx.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mxb.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhe.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hgc.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxb.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ggl.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pjt.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xit.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://gmh.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ypk.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rol.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wtn.sxryk.cn

TS:   // 同上
来源：http://htn.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jte.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kdg.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yqf.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qpi.9152youxi.cn

================================================================================
来源：http://bit.guannengcc.top

G. 面向对象
来源：http://bom.zdqjudy.top

================================================================================
来源：http://ari.chenlongwang.top

[G01] 定义类
来源：http://jmh.bjfxy.top

Py:   class User: pass
来源：http://clp.hongshengwenyu.top

PHP:  class User {}
来源：http://gbq.hysaishi.cn

JS:   class User {}
来源：http://lnt.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://meu.zhixingplan.top

Java: class User {}
来源：http://oqh.iojbl.cn

Go:   type User struct { Name string }
来源：http://sqn.hcnkem.com

Ruby: class User; end
来源：http://vwl.vehdjk.com

C#:   class User {}
来源：http://ygd.ydzc1.top

[G02] 构造函数
来源：http://nrs.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://xhf.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://gyl.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://oem.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://ivw.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://bgy.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://agw.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://yvd.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://fea.ehwqpu.com

[G03] 实例属性
来源：http://kcp.svipenyu.cn

Py:   self.name = "x"
来源：http://ama.daria6918.cn

PHP:  public string $name = "x";
来源：http://hew.c1oappe.top

JS:   this.name = "x";
来源：http://rva.jlsjyb.cn

TS:   name: string = "x";
来源：http://sgb.guowangkeji.top

Java: private String name;
来源：http://yqy.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbu.sweek.top

Ruby: @name = "x"
来源：http://mzc.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://kfc.jiagoushi.top

[G04] 定义方法
来源：http://iyv.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://atw.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bcl.wangdashe.top

JS:   greet() { return this.name; }
来源：http://bco.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://rgv.uphjek.com

Java: String greet() { return name; }
来源：http://btd.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkk.0kj1m.cn

Ruby: def greet; @name; end
来源：http://jpe.yongpay.top

C#:   public string Greet() => Name;
来源：http://mib.fehbvm.com

[G05] 继承
来源：http://nns.ivvv.top

Py:   class Admin(User): pass
来源：http://hnp.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://hvt.zdqjudy.top

JS:   class Admin extends User {}
来源：http://snq.cdnleiting.top

TS:   class Admin extends User {}
来源：http://uuh.smart0.xyz

Java: class Admin extends User {}
来源：http://sbq.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jxw.guannengcc.top

Ruby: class Admin < User; end
来源：http://lzs.sufxvd.cn

C#:   class Admin : User {}
来源：http://zsy.hnqzz.top

[G06] 重写方法
来源：http://zlv.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://mgi.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bov.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://xal.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://fxg.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://xuq.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xnc.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://eqt.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://iex.xuanzx.com

[G07] 调用父类方法
来源：http://qzf.hesvh.cn

Py:   super().greet()
来源：http://ebb.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://sna.nanxuanxn.top

JS:   super.greet();
来源：http://gtv.gzhubu.top

TS:   super.greet();
来源：http://jni.zhongyouzk.top

Java: super.greet();
来源：http://ets.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dzp.haohaochexian.top

Ruby: super
来源：http://atf.jiagoushi.top

C#:   base.Greet();
来源：http://kdc.fzhhl.top

[G08] 静态方法与属性
来源：http://nba.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://thn.yuanzhike.top

PHP:  public static function f() {}
来源：http://bhv.vehdjk.com

JS:   static f() {}
来源：http://qve.yuanzhike.top

TS:   static f(): void {}
来源：http://kmw.mhx1999.top

Java: static void f() {}
来源：http://pjh.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kmd.chenjidiqi.icu

Ruby: def self.f; end
来源：http://gyy.hywenlv.cn

C#:   public static void F() {}
来源：http://hwz.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://zlr.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://nvm.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://gek.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ukh.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://yfc.birdmap.top

Java: interface Shape { double area(); }
来源：http://kjw.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://udo.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://she.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://ywh.gaohongyu789.top

[G10] 访问控制
来源：http://wsl.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://azq.cashguo.top

PHP:  public / protected / private
来源：http://wmf.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://hej.yueranfly.top

TS:   public / protected / private
来源：http://kil.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://tpa.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ieb.yueranfly.top

Ruby: public / protected / private
来源：http://fsh.snrcjt.cn

C#:   public / protected / private / internal
来源：http://xjc.svipenyu.cn

[G11] getter / setter
来源：http://fzv.yonumen.top

Py:   @property 与 @x.setter
来源：http://nzp.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mht.sxryk.cn

JS:   get name() { return this._name; }
来源：http://ypo.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://osx.fengsongda.top

Java: public String getName() { return name; }
来源：http://aqe.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vll.mhx1999.top

Ruby: attr_accessor :name
来源：http://ita.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://hun.havefunace.top

[G12] 对象转字符串
来源：http://cuw.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://rlo.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mzm.zycfv.cn

JS:   toString() { return this.name; }
来源：http://ocf.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://adn.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://csc.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://qxx.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://jdp.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://cej.snrcjt.cn

[G13] 判断对象类型
来源：http://dzo.ctjpmb.com

Py:   isinstance(u, User)
来源：http://jvi.52xcode.cn

PHP:  $u instanceof User
来源：http://tpl.daxiang520.top

JS:   u instanceof User
来源：http://got.jianghu66.top

TS:   u instanceof User
来源：http://xwp.shuidangran.top

Java: u instanceof User
来源：http://kts.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://wic.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://kfn.meibo888.top

C#:   u is User
来源：http://ato.zhongyouzk.top

[G14] 数据类 / record
来源：http://nrk.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://azl.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://tfd.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nws.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://ghk.cheryme.top

Java: record User(String name, int age) {}
来源：http://wvd.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://fjz.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qpl.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://rcl.bbcook.cn

[G15] 枚举
来源：http://lfv.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jeo.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hxq.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqy.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sks.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://geb.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqw.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://zuy.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://drw.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://fqp.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nce.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://fxs.aibaodan.cn

JS:   Object.entries(obj)
来源：http://rry.yvedp.cn

TS:   Object.entries(obj)
来源：http://lxd.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vsf.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://glg.cashguo.top

Ruby: obj.instance_variables
来源：http://wup.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://rty.shanyushiyangtech.top

================================================================================
来源：http://jye.iojbl.cn

H. 异常与错误处理
来源：http://ovw.cucudq.cn

================================================================================
来源：http://jxc.yj20258.top

[H01] try / catch 基础
来源：http://ytc.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aut.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://knw.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gws.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mdt.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zmr.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hoz.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://idc.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ahq.cheryme.top

[H02] finally / ensure 收尾
来源：http://sqs.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jph.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://otl.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://htu.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bun.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://axy.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qsi.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ski.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rgs.bbcook.cn

[H03] 主动抛出异常
来源：http://vxv.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://nox.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ygi.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://shf.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://hmr.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uoh.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hjy.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://neq.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ojs.yj20258888.top

[H04] 自定义异常类型
来源：http://cmk.yj202588.top

Py:   class MyError(Exception): pass
来源：http://rrw.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://hyx.uphjek.com

JS:   class MyError extends Error {}
来源：http://afo.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://ovg.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://wwx.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cnz.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://vgg.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://rlm.yonumen.top

[H05] 捕获特定类型
来源：http://uyx.316326.xyz

Py:   except ValueError as e:
来源：http://wvh.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gzs.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://agf.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://cur.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://nvy.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kva.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://tae.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hab.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://gyt.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://yfj.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://npo.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fnh.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://ewk.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zkl.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://upb.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://elm.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://zex.chenlongwang.top

[H07] 断言
来源：http://llv.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://xsi.aizwys.cn

PHP:  assert($x > 0);
来源：http://zer.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://zyv.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://dpp.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://xnf.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndc.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://plq.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://sgx.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://tzd.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://wkc.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qwz.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://gls.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zqr.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://krp.gotoacloud.top

Go:   err.Error()
来源：http://cmg.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://xkx.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://cva.tarul.cn

[H09] 带错误码的异常
来源：http://bro.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gkm.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://hkb.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gfy.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ftx.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aal.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bmp.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://mvx.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hks.0kj1m.cn

[H10] 资源自动释放
来源：http://ych.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dfn.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zqo.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zly.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzy.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://anf.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://mas.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mld.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lqh.yueranfly.top

================================================================================
来源：http://gjo.dianchejie.cn

I. 正则表达式
来源：http://dqq.kuanghao11.cn

================================================================================
来源：http://kzl.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://ybq.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fts.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://mxc.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://axq.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://wvx.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vfz.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://egn.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://xdr.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ydo.pycfn.com

[I02] 提取所有匹配
来源：http://cfu.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://ftk.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wmj.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mxb.meibo888.top


<!-- 参考信息 -->