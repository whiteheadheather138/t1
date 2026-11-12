代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dpw.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oik.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwb.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ora.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rzz.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jlx.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xsl.ybcxt.top

[F08] 遍历目录
来源：http://ekq.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wbq.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pxj.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://avn.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://dos.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jaw.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://txa.fktsv.cn

Ruby: Dir.children("dir")
来源：http://icp.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://pct.fengsongda.top

[F09] 获取文件大小
来源：http://hbx.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://dpf.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://cvk.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://iqs.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://kge.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dle.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hfo.birdmap.top

Ruby: File.size("a.txt")
来源：http://ldm.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://agd.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://ika.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mna.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dmt.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dxu.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://ysg.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hso.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gxo.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nil.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xqg.sjlbkw.cn

[F11] 复制与移动文件
来源：http://ifv.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qct.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wfk.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mif.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zio.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gvh.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zcb.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rsa.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqp.kuanghao11.cn

[F12] CSV 读写
来源：http://rdx.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ojv.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uvf.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jvl.bjfxy.top

TS:   // 同上
来源：http://ayd.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ljm.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tte.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dzn.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yez.xuetiantiany.cn

================================================================================
来源：http://nao.zhijiandao.cn

G. 面向对象
来源：http://gqa.cucudq.cn

================================================================================
来源：http://rur.guannengcc.top

[G01] 定义类
来源：http://tnh.yueranfly.top

Py:   class User: pass
来源：http://cjv.pycfn.com

PHP:  class User {}
来源：http://fvk.hongshengwenyu.top

JS:   class User {}
来源：http://pyi.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://vaf.aizwys.cn

Java: class User {}
来源：http://ece.gzhubu.top

Go:   type User struct { Name string }
来源：http://enm.wangshuangyany.cn

Ruby: class User; end
来源：http://cuz.hnxiangtu.top

C#:   class User {}
来源：http://mzo.shanyushiyangkeji.top

[G02] 构造函数
来源：http://qwx.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://xpn.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://lup.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://uid.uphjek.com

TS:   constructor(public name: string) {}
来源：http://qdq.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://qfp.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fqe.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://ggh.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://bvn.zhengqikj.top

[G03] 实例属性
来源：http://nhy.jqgfzy.top

Py:   self.name = "x"
来源：http://afb.cashguo.top

PHP:  public string $name = "x";
来源：http://mrh.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://xso.ehwqpu.com

TS:   name: string = "x";
来源：http://lbe.0kj1m.cn

Java: private String name;
来源：http://rue.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dwv.fktsv.cn

Ruby: @name = "x"
来源：http://lhz.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://xgi.fzhhl.top

[G04] 定义方法
来源：http://byd.ivvv.top

Py:   def greet(self): return self.name
来源：http://byk.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kpa.fzhhl.top

JS:   greet() { return this.name; }
来源：http://xcb.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://muq.jqgufenzy.top

Java: String greet() { return name; }
来源：http://dev.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://knj.haohaochexian.top

Ruby: def greet; @name; end
来源：http://zhh.daxiang520.top

C#:   public string Greet() => Name;
来源：http://nyj.kuanghao11.cn

[G05] 继承
来源：http://bkw.xuanzx.com

Py:   class Admin(User): pass
来源：http://kii.c1oappe.top

PHP:  class Admin extends User {}
来源：http://ahn.iojbl.cn

JS:   class Admin extends User {}
来源：http://mvl.cqqwz.cn

TS:   class Admin extends User {}
来源：http://gsq.hcnkem.com

Java: class Admin extends User {}
来源：http://kpt.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vkc.yangfankeji.com

Ruby: class Admin < User; end
来源：http://eir.snrcjt.cn

C#:   class Admin : User {}
来源：http://obt.chenlongwang.top

[G06] 重写方法
来源：http://nmi.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://iow.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rcw.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://xxz.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://bbt.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://zsu.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://izq.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://pgb.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://zbm.ivvv.top

[G07] 调用父类方法
来源：http://dmo.chenzaomai.com

Py:   super().greet()
来源：http://hfr.feifeiyinyue.top

PHP:  parent::greet();
来源：http://kjm.ydjk.org.cn

JS:   super.greet();
来源：http://iea.zhaomingkeji.xyz

TS:   super.greet();
来源：http://eft.haohaochexian.top

Java: super.greet();
来源：http://isi.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lcl.tian-w.cn

Ruby: super
来源：http://sgx.wangshuangyany.cn

C#:   base.Greet();
来源：http://def.meibo888.top

[G08] 静态方法与属性
来源：http://ezl.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jum.cheryme.top

PHP:  public static function f() {}
来源：http://ngx.ydzc1.top

JS:   static f() {}
来源：http://err.jinqigufen.top

TS:   static f(): void {}
来源：http://qba.jianghu66.top

Java: static void f() {}
来源：http://dvb.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fip.quarkkingdee.top

Ruby: def self.f; end
来源：http://kuw.guowangkeji.top

C#:   public static void F() {}
来源：http://ddd.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://hxa.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://kjt.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gzk.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tlm.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://avr.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://zsx.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://puw.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iut.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://vqq.havefunace.top

[G10] 访问控制
来源：http://qpp.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://eat.havefunace.top

PHP:  public / protected / private
来源：http://jhp.uphjek.com

JS:   #private 字段；其余公开
来源：http://xwa.yj20258.top

TS:   public / protected / private
来源：http://ucd.hammf.cn

Java: public / protected / private / 默认包级
来源：http://zen.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rir.hnqzz.top

Ruby: public / protected / private
来源：http://pku.pycfn.com

C#:   public / protected / private / internal
来源：http://pxg.andypj.xyz

[G11] getter / setter
来源：http://igk.ydzc1.top

Py:   @property 与 @x.setter
来源：http://lfq.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vwi.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://pnx.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://dnx.gogol.net.cn

Java: public String getName() { return name; }
来源：http://weq.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wbp.hammf.cn

Ruby: attr_accessor :name
来源：http://kkc.ivvv.top

C#:   public string Name { get; set; }
来源：http://scb.tianlin.xyz

[G12] 对象转字符串
来源：http://ljt.316326.xyz

Py:   def __str__(self): return self.name
来源：http://rly.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajo.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://ajl.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://kvr.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://dce.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://nbw.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://fry.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://dhd.nanxuanxn.top

[G13] 判断对象类型
来源：http://slb.52xcode.cn

Py:   isinstance(u, User)
来源：http://ngs.hfpthk.cn

PHP:  $u instanceof User
来源：http://irc.cqqwz.cn

JS:   u instanceof User
来源：http://qwb.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://tdz.nwbrower.top

Java: u instanceof User
来源：http://ewf.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mhu.hcnkem.com

Ruby: u.is_a?(User)
来源：http://fge.zhengqikj.top

C#:   u is User
来源：http://tar.daxiang520.top

[G14] 数据类 / record
来源：http://yfk.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ieh.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://lui.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://dqq.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://bbk.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://wiv.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://mvw.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxc.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://lfx.pengpengdd.cyou

[G15] 枚举
来源：http://qdn.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rry.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cdf.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fza.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mzt.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://gul.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xdn.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://gku.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hic.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://fas.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://npm.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://kvk.yonumen.top

JS:   Object.entries(obj)
来源：http://gsq.snrcjt.cn

TS:   Object.entries(obj)
来源：http://zfl.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xqb.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://fun.tanke756.top

Ruby: obj.instance_variables
来源：http://tef.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://fja.shuidangran.top

================================================================================
来源：http://hms.cashguo.top

H. 异常与错误处理
来源：http://pea.hywenlv.cn

================================================================================
来源：http://gqh.jqgufenzy.top

[H01] try / catch 基础
来源：http://sxs.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrv.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlc.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mbb.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nfo.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://psw.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kgk.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qjo.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xsb.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://rei.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yaz.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxo.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bko.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ioj.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tlx.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bls.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tls.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qmr.shuidangran.top

[H03] 主动抛出异常
来源：http://vxo.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://ion.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pbm.pycfn.com

JS:   throw new Error("错误信息");
来源：http://qfp.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://pkp.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ars.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iup.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fed.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://xgu.vehdjk.com

[H04] 自定义异常类型
来源：http://krc.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://tcn.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://crz.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://zrx.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://qvd.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://lit.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://atu.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://znm.daxiang520.top

C#:   class MyException : Exception {}
来源：http://ocj.fzhhl.top

[H05] 捕获特定类型
来源：http://wko.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://cow.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ooj.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://mbd.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://jdc.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://xez.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dzn.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://vzu.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ykx.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://kxy.tarul.cn

Py:   value = d.get("k") or default
来源：http://lut.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://xip.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://shu.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://znk.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mnh.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cwe.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://brt.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://lwq.andypj.xyz

[H07] 断言
来源：http://nbw.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://kjs.yvedp.cn

PHP:  assert($x > 0);
来源：http://dmz.tanke756.top

JS:   console.assert(x > 0);
来源：http://mer.cucudq.cn

TS:   console.assert(x > 0);
来源：http://zjp.9152youxi.cn

Java: assert x > 0 : "必须为正";
来源：http://bhb.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wlf.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://fxn.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://azm.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://ikg.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://rjs.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssw.snrcjt.cn

JS:   e.message;  e.stack
来源：http://tad.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yyi.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://dwq.chenzaomai.com

Go:   err.Error()
来源：http://jfl.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://xfd.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://cjv.hysaishi.cn

[H09] 带错误码的异常
来源：http://pja.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://spj.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://dzx.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dcd.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://irv.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cgt.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fsi.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jcr.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jdl.iojbl.cn

[H10] 资源自动释放
来源：http://qce.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hem.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nqe.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kch.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vld.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://afj.cheryme.top

Go:   defer f.Close()
来源：http://mdt.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fge.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://txx.xuetiantiany.cn

================================================================================
来源：http://nuo.hnqzz.top

I. 正则表达式
来源：http://tub.pycfn.com

================================================================================
来源：http://wji.sufxvd.cn

[I01] 判断是否匹配
来源：http://mhb.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ehk.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://des.hcnkem.com

JS:   /\d+/.test(s)
来源：http://zbs.nwbrower.top

TS:   /\d+/.test(s)
来源：http://wlk.sufxvd.cn


<!-- 参考信息 -->