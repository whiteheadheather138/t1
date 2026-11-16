代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://zwy.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xgu.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://drd.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://moq.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jtf.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://atb.yj202588.top

Ruby: Dir.children("dir")
来源：http://mzx.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://yci.andypj.xyz

[F09] 获取文件大小
来源：http://qzc.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://alo.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://alr.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://tdx.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://xvt.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://mbb.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ljc.yueranfly.top

Ruby: File.size("a.txt")
来源：http://gmf.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://jmb.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://gtl.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fhh.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://btv.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vom.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://aja.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zht.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ajg.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jfw.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qdr.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://zpt.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hhd.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ucg.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bub.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ekt.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xhj.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mjq.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mom.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ggv.vqdsnc.cn

[F12] CSV 读写
来源：http://lyc.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iwk.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vpb.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://djd.hcnkem.com

TS:   // 同上
来源：http://xna.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://axy.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ija.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ase.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zad.jinqigfzy.top

================================================================================
来源：http://gxr.fktsv.cn

G. 面向对象
来源：http://gad.yonumen.top

================================================================================
来源：http://uzl.birdmap.top

[G01] 定义类
来源：http://hjp.mhx1999.top

Py:   class User: pass
来源：http://dqa.gogol.net.cn

PHP:  class User {}
来源：http://wdj.bjfxy.top

JS:   class User {}
来源：http://hib.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://iub.guowangkeji.top

Java: class User {}
来源：http://zto.hfpthk.cn

Go:   type User struct { Name string }
来源：http://xil.smart0.xyz

Ruby: class User; end
来源：http://wxh.shanyushiyangtech.top

C#:   class User {}
来源：http://bth.ydjk.org.cn

[G02] 构造函数
来源：http://mvd.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://gpb.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://wul.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://wjl.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://icc.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://gvb.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qab.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://nih.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://aqp.guannengcc.top

[G03] 实例属性
来源：http://bhq.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://zte.birdmap.top

PHP:  public string $name = "x";
来源：http://fzz.cashguo.top

JS:   this.name = "x";
来源：http://kqp.daria6918.cn

TS:   name: string = "x";
来源：http://kwj.xuanzx.com

Java: private String name;
来源：http://ogd.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gjt.hammf.cn

Ruby: @name = "x"
来源：http://avr.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://chs.yj202588.top

[G04] 定义方法
来源：http://qgf.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://ole.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ush.xuanzx.com

JS:   greet() { return this.name; }
来源：http://kqr.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://twg.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://ixb.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yxv.zycfv.cn

Ruby: def greet; @name; end
来源：http://egx.mhx1999.top

C#:   public string Greet() => Name;
来源：http://bdm.jqgufenzy.top

[G05] 继承
来源：http://qqk.aibaodan.cn

Py:   class Admin(User): pass
来源：http://kxr.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://idv.zycfv.cn

JS:   class Admin extends User {}
来源：http://zcd.hywenlv.cn

TS:   class Admin extends User {}
来源：http://evs.mhx1999.top

Java: class Admin extends User {}
来源：http://egf.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ftb.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://jaz.hnxiangtu.top

C#:   class Admin : User {}
来源：http://hba.zhiwuduotai.top

[G06] 重写方法
来源：http://soo.pycfn.com

Py:   def greet(self): return "admin"
来源：http://abu.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dkt.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://smq.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://mrm.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://sxu.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vgm.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://pph.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://glg.svipenyu.cn

[G07] 调用父类方法
来源：http://pdv.redwolf501.top

Py:   super().greet()
来源：http://dau.pengpengdd.cyou

PHP:  parent::greet();
来源：http://yzh.hammf.cn

JS:   super.greet();
来源：http://iqw.ppjwa.cn

TS:   super.greet();
来源：http://jwe.yj20258.top

Java: super.greet();
来源：http://bxr.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ewz.havefunace.top

Ruby: super
来源：http://aqa.daria6918.cn

C#:   base.Greet();
来源：http://doa.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://ari.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lxt.jqgfzy.top

PHP:  public static function f() {}
来源：http://cyq.jlsjyb.cn

JS:   static f() {}
来源：http://lxh.shzxlz.cn

TS:   static f(): void {}
来源：http://pqq.gogol.net.cn

Java: static void f() {}
来源：http://men.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rre.iojbl.cn

Ruby: def self.f; end
来源：http://eao.ehwqpu.com

C#:   public static void F() {}
来源：http://arx.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://rgu.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://ion.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://xce.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ocb.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://geg.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://uci.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://hjh.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zww.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://syu.zhongyouzk.top

[G10] 访问控制
来源：http://lha.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://zkq.zhongyouzk.top

PHP:  public / protected / private
来源：http://rgr.birdmap.top

JS:   #private 字段；其余公开
来源：http://uho.hywenlv.cn

TS:   public / protected / private
来源：http://yzy.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://qgg.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mnv.ivvv.top

Ruby: public / protected / private
来源：http://mqk.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://cix.aibaodan.cn

[G11] getter / setter
来源：http://kge.ivvv.top

Py:   @property 与 @x.setter
来源：http://uea.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fbd.sxryk.cn

JS:   get name() { return this._name; }
来源：http://hak.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://elj.shuidangran.top

Java: public String getName() { return name; }
来源：http://txp.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzx.hcnkem.com

Ruby: attr_accessor :name
来源：http://aca.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://eea.zhijiandao.cn

[G12] 对象转字符串
来源：http://nte.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://aly.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xhw.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://nvn.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://rpl.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://bkl.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://dgr.cheryme.top

Ruby: def to_s; @name; end
来源：http://bjq.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://wyf.shuidangran.top

[G13] 判断对象类型
来源：http://gml.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://irx.nwbrower.top

PHP:  $u instanceof User
来源：http://pbk.52xcode.cn

JS:   u instanceof User
来源：http://zlt.fengsongda.top

TS:   u instanceof User
来源：http://dow.tianlin.xyz

Java: u instanceof User
来源：http://oke.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ohd.yj20258888.top

Ruby: u.is_a?(User)
来源：http://jes.daxiang520.top

C#:   u is User
来源：http://zab.vehdjk.com

[G14] 数据类 / record
来源：http://qdw.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jib.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://ckr.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://ooa.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://bdy.xinyue.icu

Java: record User(String name, int age) {}
来源：http://tls.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://cwu.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hig.cashguo.top

C#:   record User(string Name, int Age);
来源：http://pyd.jinyuanbaomall.cn

[G15] 枚举
来源：http://ija.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mtf.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ypw.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cfr.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eez.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://myo.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ckt.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://wue.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rhb.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://eii.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aio.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://rjt.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://luu.chenzaomai.com

TS:   Object.entries(obj)
来源：http://vto.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zew.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjc.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://bac.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://xoc.hnqzz.top

================================================================================
来源：http://qnu.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://cix.yj202588.top

================================================================================
来源：http://jji.pengpengdd.cyou

[H01] try / catch 基础
来源：http://oki.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://smy.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hdc.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ttf.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xkh.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xog.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://whm.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wyj.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fyz.redwolf501.top

[H02] finally / ensure 收尾
来源：http://lxl.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://vyp.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhf.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uaf.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pxi.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hgs.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ekc.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://atd.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cjn.yj202588.top

[H03] 主动抛出异常
来源：http://bvh.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://zjw.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vmq.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://auh.tanke756.top

TS:   throw new Error("错误信息");
来源：http://ffx.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ywr.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dfc.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hnc.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://qjc.epnwcf.com

[H04] 自定义异常类型
来源：http://nwh.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://ofh.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mxk.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://jol.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://qgs.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://cbq.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jjb.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://oyj.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://bcf.cucudq.cn

[H05] 捕获特定类型
来源：http://edv.zhixingplan.top

Py:   except ValueError as e:
来源：http://qeo.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qjg.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://kjk.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://ejg.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://rvq.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zmh.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://ilh.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wly.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://our.xuanzx.com

Py:   value = d.get("k") or default
来源：http://dxj.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://bed.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://fjr.pycfn.com

TS:   obj?.a?.b;  d ?? default
来源：http://zxl.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dkq.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://gwm.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://fpm.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://ase.daxiang520.top

[H07] 断言
来源：http://krb.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://esx.ydzc1.top

PHP:  assert($x > 0);
来源：http://yly.hcnkem.com

JS:   console.assert(x > 0);
来源：http://daz.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://wsj.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://cof.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ssc.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lgt.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://rwb.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://jtv.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://yoo.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mvm.daria6918.cn

JS:   e.message;  e.stack
来源：http://fmk.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://asv.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sfs.cashguo.top

Go:   err.Error()
来源：http://can.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://sbs.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://dzy.yvedp.cn

[H09] 带错误码的异常
来源：http://wmj.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pcg.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://scj.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://whs.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://spe.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ctk.zhixingplan.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gks.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lbu.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xkj.yueranfly.top

[H10] 资源自动释放
来源：http://dcc.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qnz.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxk.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hiy.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lnq.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rkb.wangshuangyany.cn

Go:   defer f.Close()
来源：http://uub.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qim.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qun.epnwcf.com

================================================================================
来源：http://nib.hfpthk.cn

I. 正则表达式
来源：http://ead.zdqjudy.top

================================================================================
来源：http://oia.smart0.xyz

[I01] 判断是否匹配
来源：http://ceh.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mdb.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pfh.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://dvc.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://cwm.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ilz.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uew.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://bbv.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ysc.ydjk.org.cn

[I02] 提取所有匹配
来源：http://ukn.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://hio.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rxw.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fjp.xuanzx.com


<!-- 参考信息 -->