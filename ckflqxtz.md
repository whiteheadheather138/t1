代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://pat.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ikk.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://ktk.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://zwx.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oxq.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://iwa.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://cdk.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://vgk.hysaishi.cn

[F09] 获取文件大小
来源：http://cai.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://zec.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://wig.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://dtp.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://aql.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dic.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kvd.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://pzr.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://wmd.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://twn.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nem.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ghy.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qtp.fktsv.cn

TS:   path.extname("a.txt")
来源：http://vct.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmo.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vpz.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://abc.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ltv.guowangkeji.top

[F11] 复制与移动文件
来源：http://gwe.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xrs.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zle.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yev.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbk.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wor.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ccv.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gqt.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jne.chenzaomai.com

[F12] CSV 读写
来源：http://tsu.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kxk.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tlc.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hio.jyoumei.cn

TS:   // 同上
来源：http://yrz.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fba.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hkt.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hgc.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://clq.uphjek.com

================================================================================
来源：http://vgj.zhaomingkeji.xyz

G. 面向对象
来源：http://dkb.snrcjt.cn

================================================================================
来源：http://fzn.smart0.xyz

[G01] 定义类
来源：http://zrr.fzhhl.top

Py:   class User: pass
来源：http://kpg.cashguo.top

PHP:  class User {}
来源：http://ahk.yonumen.top

JS:   class User {}
来源：http://tcw.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://fkv.jyoumei.cn

Java: class User {}
来源：http://bsr.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://ijb.cheryme.top

Ruby: class User; end
来源：http://goo.guannengcc.top

C#:   class User {}
来源：http://tvz.gaohongyu789.top

[G02] 构造函数
来源：http://cfc.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://idj.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://fto.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://ymb.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://sll.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://wpd.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bcc.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://rep.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://fns.tian-w.cn

[G03] 实例属性
来源：http://kak.bjfxy.top

Py:   self.name = "x"
来源：http://ldz.epnwcf.com

PHP:  public string $name = "x";
来源：http://fpo.hnxiangtu.top

JS:   this.name = "x";
来源：http://tkd.cucudq.cn

TS:   name: string = "x";
来源：http://utq.yuxming.cn

Java: private String name;
来源：http://uxn.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uep.gogol.net.cn

Ruby: @name = "x"
来源：http://xqk.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://git.guowangkeji.top

[G04] 定义方法
来源：http://txu.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://zpa.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wmv.pycfn.com

JS:   greet() { return this.name; }
来源：http://lnu.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://utm.sweek.top

Java: String greet() { return name; }
来源：http://wcs.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wue.vehdjk.com

Ruby: def greet; @name; end
来源：http://pwc.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://seg.tianlin.xyz

[G05] 继承
来源：http://uqj.ctjpmb.com

Py:   class Admin(User): pass
来源：http://buq.yueranfly.top

PHP:  class Admin extends User {}
来源：http://kbh.tian-w.cn

JS:   class Admin extends User {}
来源：http://kdr.nanxinkj.top

TS:   class Admin extends User {}
来源：http://qyq.jqgufenzy.top

Java: class Admin extends User {}
来源：http://sqc.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kie.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://roz.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://oqc.tianlin.xyz

[G06] 重写方法
来源：http://avc.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://fuu.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dit.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://ech.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://zdp.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vwk.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://twn.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://kdi.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://tna.c1oappe.top

[G07] 调用父类方法
来源：http://wuq.fehbvm.com

Py:   super().greet()
来源：http://jaf.shangyingyoupin.top

PHP:  parent::greet();
来源：http://bbe.redwolf501.top

JS:   super.greet();
来源：http://tmx.yonumen.top

TS:   super.greet();
来源：http://rod.jlsjyb.cn

Java: super.greet();
来源：http://scb.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wxf.zhaomingkeji.xyz

Ruby: super
来源：http://dlw.fktsv.cn

C#:   base.Greet();
来源：http://rhz.gogol.net.cn

[G08] 静态方法与属性
来源：http://lvs.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hbg.fengsongda.top

PHP:  public static function f() {}
来源：http://wcr.yj202588.top

JS:   static f() {}
来源：http://lem.hfpthk.cn

TS:   static f(): void {}
来源：http://cei.bjfxy.top

Java: static void f() {}
来源：http://auh.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gsc.birdmap.top

Ruby: def self.f; end
来源：http://vfg.shuidangran.top

C#:   public static void F() {}
来源：http://pod.yuxming.cn

[G09] 接口 / 抽象类
来源：http://rxh.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://iyq.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://olq.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fqc.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://cjf.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://psv.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://bih.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uch.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://qgk.zhoulong.xyz

[G10] 访问控制
来源：http://aic.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://yny.hnqzz.top

PHP:  public / protected / private
来源：http://dte.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://muz.uphjek.com

TS:   public / protected / private
来源：http://nqm.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://olv.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://agm.snrcjt.cn

Ruby: public / protected / private
来源：http://bvd.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://uga.yueranfly.top

[G11] getter / setter
来源：http://gtn.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://coi.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zke.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://ocq.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://xui.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://hql.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lys.zdqjudy.top

Ruby: attr_accessor :name
来源：http://hao.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://vuz.snrcjt.cn

[G12] 对象转字符串
来源：http://pwe.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://jto.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://img.cucudq.cn

JS:   toString() { return this.name; }
来源：http://efa.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://mat.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://iof.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gpn.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://sdm.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://qrx.cashguo.top

[G13] 判断对象类型
来源：http://hwc.fehbvm.com

Py:   isinstance(u, User)
来源：http://dzh.tianlin.xyz

PHP:  $u instanceof User
来源：http://tkr.havefunace.top

JS:   u instanceof User
来源：http://kcx.ydjk.org.cn

TS:   u instanceof User
来源：http://zwl.guowangkeji.top

Java: u instanceof User
来源：http://wmz.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vio.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://tln.fehbvm.com

C#:   u is User
来源：http://tko.gzhubu.top

[G14] 数据类 / record
来源：http://tov.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://osy.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://lkw.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://gar.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://eey.ivvv.top

Java: record User(String name, int age) {}
来源：http://ssg.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://tqj.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zzb.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://nvp.andypj.xyz

[G15] 枚举
来源：http://wcz.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ulk.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://jkx.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zmd.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mei.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://bhh.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nwc.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://inu.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nzj.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://nuv.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://prn.tarul.cn

PHP:  get_object_vars($obj);
来源：http://gya.yangfankeji.com

JS:   Object.entries(obj)
来源：http://ppb.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://mvc.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dio.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ldz.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://wxm.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://nyb.zhixingplan.top

================================================================================
来源：http://otq.uphjek.com

H. 异常与错误处理
来源：http://buo.sysykeji.top

================================================================================
来源：http://dtd.yuxming.cn

[H01] try / catch 基础
来源：http://mef.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vhc.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkx.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vcu.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hho.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wae.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iog.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xpb.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qul.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://wiz.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://fpm.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://cro.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zim.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oxn.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://wyo.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zel.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aax.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ajq.jlsjyb.cn

[H03] 主动抛出异常
来源：http://iuv.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://rze.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bav.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://mmi.pycfn.com

TS:   throw new Error("错误信息");
来源：http://zie.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ium.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gqd.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zfc.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://wzj.aizwys.cn

[H04] 自定义异常类型
来源：http://jix.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://kgi.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://rro.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://kxd.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://pmc.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://ncm.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fys.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://giv.bbcook.cn

C#:   class MyException : Exception {}
来源：http://kbx.zdqjudy.top

[H05] 捕获特定类型
来源：http://zpn.yanxiufei.cn

Py:   except ValueError as e:
来源：http://ahw.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sre.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ght.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wsl.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://dka.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uth.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://gvr.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gbx.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://kiz.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://zci.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://gcq.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://wpb.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://eru.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnm.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://bza.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://syb.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://yae.yonumen.top

[H07] 断言
来源：http://chh.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://xfp.ppjwa.cn

PHP:  assert($x > 0);
来源：http://ipe.pycfn.com

JS:   console.assert(x > 0);
来源：http://rxg.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://ltf.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://wzc.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cxu.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://art.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://kjn.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://olp.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://vug.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yum.ivvv.top

JS:   e.message;  e.stack
来源：http://wvj.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wps.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vbs.nanxinkj.top

Go:   err.Error()
来源：http://okm.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://jew.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://bkf.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://uxy.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wwb.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtc.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fdg.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bpf.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qku.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://utk.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ruv.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zuy.gotoacloud.top

[H10] 资源自动释放
来源：http://vcf.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://van.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tbm.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxn.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qdv.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://utc.zycfv.cn

Go:   defer f.Close()
来源：http://zzu.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fge.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ymu.xinyue.icu

================================================================================
来源：http://rsv.tian-w.cn

I. 正则表达式
来源：http://krj.wangdashe.top

================================================================================
来源：http://otf.ydzc1.top

[I01] 判断是否匹配
来源：http://mph.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zar.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zdy.yfazqb.com

JS:   /\d+/.test(s)
来源：http://aej.ivvv.top

TS:   /\d+/.test(s)
来源：http://kjf.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://amh.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pqr.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://pjl.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ugr.zhengqikj.top

[I02] 提取所有匹配
来源：http://jyx.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://glh.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zks.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://byg.andypj.xyz


<!-- 参考信息 -->