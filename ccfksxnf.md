代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://iwy.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fyf.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://wib.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://xza.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nuu.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://pve.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://qgu.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://jmy.wangshuangyany.cn

[F09] 获取文件大小
来源：http://jkp.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://mgn.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://wzk.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://xts.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://oqd.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lro.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jrt.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://nvb.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://qli.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://unv.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ucm.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yse.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rja.xuanzx.com

TS:   path.extname("a.txt")
来源：http://eut.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://voi.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jyo.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qzy.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jvh.zhongyouzk.top

[F11] 复制与移动文件
来源：http://kfo.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lrb.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://leo.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sku.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhs.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sbd.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iqz.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tev.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://brr.fanxiaobao.xyz

[F12] CSV 读写
来源：http://riv.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxv.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ybh.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://csm.52xcode.cn

TS:   // 同上
来源：http://cii.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yeo.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://usv.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gum.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://mth.dashuyun.cn

================================================================================
来源：http://sah.yangfankeji.com

G. 面向对象
来源：http://gsj.dianchejie.cn

================================================================================
来源：http://ndg.sweek.top

[G01] 定义类
来源：http://tlb.sweek.top

Py:   class User: pass
来源：http://iwi.xylfe.cn

PHP:  class User {}
来源：http://sgb.fengsongda.top

JS:   class User {}
来源：http://izv.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://rlj.quarkkingdee.top

Java: class User {}
来源：http://bid.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://acm.shanyushiyangkeji.top

Ruby: class User; end
来源：http://gje.jinqigufen.top

C#:   class User {}
来源：http://goh.zdqjudy.top

[G02] 构造函数
来源：http://zmh.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://oxw.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://wie.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://zgb.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://ctc.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://avw.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zdx.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://svr.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://uhw.jinyuanbaomall.cn

[G03] 实例属性
来源：http://rcj.xuanzx.com

Py:   self.name = "x"
来源：http://qrf.tarul.cn

PHP:  public string $name = "x";
来源：http://qxy.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://pvf.andypj.xyz

TS:   name: string = "x";
来源：http://eib.xinyue.icu

Java: private String name;
来源：http://dps.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyg.svipenyu.cn

Ruby: @name = "x"
来源：http://ptf.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://tdo.smart0.xyz

[G04] 定义方法
来源：http://hwv.vehdjk.com

Py:   def greet(self): return self.name
来源：http://jdz.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ogl.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://gqy.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://ofb.fengsongda.top

Java: String greet() { return name; }
来源：http://hie.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wke.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://brb.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://nxe.cucudq.cn

[G05] 继承
来源：http://vsf.chenlongwang.top

Py:   class Admin(User): pass
来源：http://hgb.redwolf501.top

PHP:  class Admin extends User {}
来源：http://fta.yangfankeji.com

JS:   class Admin extends User {}
来源：http://npm.yfazqb.com

TS:   class Admin extends User {}
来源：http://mux.nanxinkj.top

Java: class Admin extends User {}
来源：http://rdg.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvt.yangfankeji.com

Ruby: class Admin < User; end
来源：http://isd.epnwcf.com

C#:   class Admin : User {}
来源：http://yyu.cheryme.top

[G06] 重写方法
来源：http://ulf.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://hkp.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wmz.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://ovs.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://qne.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://cqf.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cxf.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://kam.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://lta.jianghu66.top

[G07] 调用父类方法
来源：http://hyy.hnqzz.top

Py:   super().greet()
来源：http://xxs.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://czx.chenzaomai.com

JS:   super.greet();
来源：http://ucy.hcnkem.com

TS:   super.greet();
来源：http://akv.jlsjyb.cn

Java: super.greet();
来源：http://hij.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hmv.wangshuangyany.cn

Ruby: super
来源：http://vhi.havefunace.top

C#:   base.Greet();
来源：http://vwu.hysaishi.cn

[G08] 静态方法与属性
来源：http://gls.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wrn.jqgufenzy.top

PHP:  public static function f() {}
来源：http://zxf.hywenlv.cn

JS:   static f() {}
来源：http://znz.c1oappe.top

TS:   static f(): void {}
来源：http://zsy.jlsjyb.cn

Java: static void f() {}
来源：http://pkd.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dac.xuanzx.com

Ruby: def self.f; end
来源：http://uaw.gotoacloud.top

C#:   public static void F() {}
来源：http://jvi.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://ptq.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://qad.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://jao.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jxw.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://wkm.daxiang520.top

Java: interface Shape { double area(); }
来源：http://qpw.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://sxr.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dbx.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://doy.mhx1999.top

[G10] 访问控制
来源：http://rjp.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://gmq.fehbvm.com

PHP:  public / protected / private
来源：http://fru.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://akd.hnqzz.top

TS:   public / protected / private
来源：http://zya.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://ern.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qcl.chenjidiqi.icu

Ruby: public / protected / private
来源：http://tvg.fktsv.cn

C#:   public / protected / private / internal
来源：http://zxp.fanxiaobao.xyz

[G11] getter / setter
来源：http://qhi.meibo888.top

Py:   @property 与 @x.setter
来源：http://bpt.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://qap.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://iux.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://igd.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://gqn.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jyt.redwolf501.top

Ruby: attr_accessor :name
来源：http://sdc.gzhubu.top

C#:   public string Name { get; set; }
来源：http://oxw.hammf.cn

[G12] 对象转字符串
来源：http://hzm.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://mfe.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xlz.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://ias.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://yey.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://mxk.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://iuu.guannengcc.top

Ruby: def to_s; @name; end
来源：http://ozv.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://dvy.tarul.cn

[G13] 判断对象类型
来源：http://aaq.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://cyv.fengsongda.top

PHP:  $u instanceof User
来源：http://avs.gotoacloud.top

JS:   u instanceof User
来源：http://vum.xziqi.cn

TS:   u instanceof User
来源：http://wpx.jinyuanbaomall.cn

Java: u instanceof User
来源：http://fnv.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdk.yj20258.top

Ruby: u.is_a?(User)
来源：http://xkg.andypj.xyz

C#:   u is User
来源：http://wca.zhiwuduotai.top

[G14] 数据类 / record
来源：http://urp.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://acv.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://pyt.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://xwy.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://ona.jianghu66.top

Java: record User(String name, int age) {}
来源：http://moh.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://sru.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ucd.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://nut.xuanzx.com

[G15] 枚举
来源：http://iym.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ilk.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://vhp.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fsr.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jco.sweek.top

Java: enum Color { RED, GREEN }
来源：http://mpa.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ooq.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://zyq.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnz.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://trt.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jmq.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://oit.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://iih.shuidangran.top

TS:   Object.entries(obj)
来源：http://kdy.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uso.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gfk.yuxming.cn

Ruby: obj.instance_variables
来源：http://lgo.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://dzw.gogol.net.cn

================================================================================
来源：http://csh.quarkkingdee.top

H. 异常与错误处理
来源：http://zbe.aizwys.cn

================================================================================
来源：http://kwy.xylfe.cn

[H01] try / catch 基础
来源：http://rus.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://obn.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ing.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tgv.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vit.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://drb.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oby.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zbs.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eft.pycfn.com

[H02] finally / ensure 收尾
来源：http://uws.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://box.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ujz.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hzh.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://vma.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://kxw.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ylf.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hzi.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://how.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://vbo.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://nhb.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eiq.tarul.cn

JS:   throw new Error("错误信息");
来源：http://gjb.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://mpp.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wsb.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wvy.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qhe.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://dwg.sweek.top

[H04] 自定义异常类型
来源：http://inx.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://qjz.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gje.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://xbn.ybcxt.top

TS:   class MyError extends Error {}
来源：http://ruk.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://uwk.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajt.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://dki.birdmap.top

C#:   class MyException : Exception {}
来源：http://bfu.sufxvd.cn

[H05] 捕获特定类型
来源：http://kbm.xinyue.icu

Py:   except ValueError as e:
来源：http://vml.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wcl.fzhhl.top

JS:   if (e instanceof TypeError) {}
来源：http://djc.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://yqe.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://kyi.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://urt.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://aca.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lnn.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://rxl.yj20258888.top

Py:   value = d.get("k") or default
来源：http://xfz.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oaz.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://day.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ryn.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jty.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vlt.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://eqw.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://fvz.uphjek.com

[H07] 断言
来源：http://kfe.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://qxv.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://elh.ybcxt.top

JS:   console.assert(x > 0);
来源：http://xlb.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://ygd.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://odv.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqs.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://joh.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://auq.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://wjs.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://snd.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gbe.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://pmo.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zzt.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://egv.fanxiaobao.xyz

Go:   err.Error()
来源：http://fhq.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://iql.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://rfl.pycfn.com

[H09] 带错误码的异常
来源：http://rii.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjl.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kna.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xgk.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qht.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kbp.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktj.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://naq.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://okn.fzhhl.top

[H10] 资源自动释放
来源：http://usg.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://enw.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pbo.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jvo.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bth.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldv.yonumen.top

Go:   defer f.Close()
来源：http://jyp.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hgo.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yri.bjfxy.top

================================================================================
来源：http://lae.hywenlv.cn

I. 正则表达式
来源：http://igg.yfazqb.com

================================================================================
来源：http://dmp.daria6918.cn

[I01] 判断是否匹配
来源：http://jej.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ggb.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://rmh.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://ulz.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://yop.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvb.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://czm.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://nsi.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xle.nanxuanxn.top

[I02] 提取所有匹配
来源：http://aca.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://poz.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sop.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rif.svipenyu.cn


<!-- 参考信息 -->