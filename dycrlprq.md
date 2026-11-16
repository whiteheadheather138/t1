代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kae.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ych.ybcxt.top

Ruby: Dir.children("dir")
来源：http://aqb.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://ife.havefunace.top

[F09] 获取文件大小
来源：http://pui.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://qbi.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://eld.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://fgx.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://sjl.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://hpj.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wti.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://yft.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://zob.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://tec.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dtm.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aqf.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hdc.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://ydf.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://obc.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xqw.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ajd.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fgt.zhijiandao.cn

[F11] 复制与移动文件
来源：http://twd.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kwr.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hia.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlm.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alm.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yoe.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ngp.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ife.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vat.fktsv.cn

[F12] CSV 读写
来源：http://ajz.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dwh.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lzq.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gai.zycfv.cn

TS:   // 同上
来源：http://buq.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://shn.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jiw.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jlx.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://spj.wangdashe.top

================================================================================
来源：http://bhl.daria6918.cn

G. 面向对象
来源：http://rxk.zhaomingkeji.xyz

================================================================================
来源：http://ocr.zhongyouzk.top

[G01] 定义类
来源：http://uvu.yonumen.top

Py:   class User: pass
来源：http://kgm.havefunace.top

PHP:  class User {}
来源：http://wkm.havefunace.top

JS:   class User {}
来源：http://dvr.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://sui.ydzc1.top

Java: class User {}
来源：http://wlb.zycfv.cn

Go:   type User struct { Name string }
来源：http://pcx.c1oappe.top

Ruby: class User; end
来源：http://udk.ctjpmb.com

C#:   class User {}
来源：http://nrr.svipenyu.cn

[G02] 构造函数
来源：http://pxq.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://gzw.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://qjs.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://ksu.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://tog.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://aog.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lch.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://ekd.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://qsp.hesvh.cn

[G03] 实例属性
来源：http://toi.cqqwz.cn

Py:   self.name = "x"
来源：http://vaa.hywenlv.cn

PHP:  public string $name = "x";
来源：http://uku.ydjk.org.cn

JS:   this.name = "x";
来源：http://pno.fehbvm.com

TS:   name: string = "x";
来源：http://lqq.xingfuxueyuan.xyz

Java: private String name;
来源：http://oct.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bwa.yj202588.top

Ruby: @name = "x"
来源：http://cfa.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://nst.smart0.xyz

[G04] 定义方法
来源：http://obb.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://thb.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sce.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://jbk.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://xrw.sjlbkw.cn

Java: String greet() { return name; }
来源：http://usq.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://hzc.vehdjk.com

Ruby: def greet; @name; end
来源：http://smq.hammf.cn

C#:   public string Greet() => Name;
来源：http://bul.chenzaomai.com

[G05] 继承
来源：http://jeu.mhx1999.top

Py:   class Admin(User): pass
来源：http://jnx.ybcxt.top

PHP:  class Admin extends User {}
来源：http://knf.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://hvc.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://gcn.andypj.xyz

Java: class Admin extends User {}
来源：http://djy.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://snz.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://uky.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://rjc.gaohongyu789.top

[G06] 重写方法
来源：http://cjs.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://xvk.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://ixv.hammf.cn

JS:   greet() { return "admin"; }
来源：http://zkl.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://qoc.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://dsz.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pfg.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://tcq.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://kmg.aizwys.cn

[G07] 调用父类方法
来源：http://rkh.xuetiantiany.cn

Py:   super().greet()
来源：http://gxa.yongpay.top

PHP:  parent::greet();
来源：http://bdv.dashuyun.cn

JS:   super.greet();
来源：http://xvm.tianlin.xyz

TS:   super.greet();
来源：http://bqc.zhixingplan.top

Java: super.greet();
来源：http://dfk.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://los.svipenyu.cn

Ruby: super
来源：http://wcb.zycfv.cn

C#:   base.Greet();
来源：http://ktn.yuxming.cn

[G08] 静态方法与属性
来源：http://ris.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kcs.tian-w.cn

PHP:  public static function f() {}
来源：http://pmc.quarkkingdee.top

JS:   static f() {}
来源：http://cth.redwolf501.top

TS:   static f(): void {}
来源：http://whc.jinqigufen.top

Java: static void f() {}
来源：http://ptk.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uth.gaohongyu789.top

Ruby: def self.f; end
来源：http://pdt.xuetiantiany.cn

C#:   public static void F() {}
来源：http://yuz.sysykeji.top

[G09] 接口 / 抽象类
来源：http://joz.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://aap.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dlj.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tkz.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://plt.hesvh.cn

Java: interface Shape { double area(); }
来源：http://gcx.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://zhm.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://atc.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://goo.sxryk.cn

[G10] 访问控制
来源：http://qvz.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://oyb.andypj.xyz

PHP:  public / protected / private
来源：http://vtb.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://dfb.0kj1m.cn

TS:   public / protected / private
来源：http://ffn.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://xvl.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zwc.daxiang520.top

Ruby: public / protected / private
来源：http://yhh.epnwcf.com

C#:   public / protected / private / internal
来源：http://okt.mhx1999.top

[G11] getter / setter
来源：http://hzk.ybcxt.top

Py:   @property 与 @x.setter
来源：http://eff.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://aro.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://qgh.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://dvu.c1oappe.top

Java: public String getName() { return name; }
来源：http://hnz.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vrm.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://fyh.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://gtf.c1oappe.top

[G12] 对象转字符串
来源：http://mpx.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://jhj.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://boi.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://cfo.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://cwx.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://bki.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://lcj.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://mmx.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://ofb.uphjek.com

[G13] 判断对象类型
来源：http://ukk.yuanzhike.top

Py:   isinstance(u, User)
来源：http://sjy.bbcook.cn

PHP:  $u instanceof User
来源：http://wzz.shuidangran.top

JS:   u instanceof User
来源：http://wdf.pengpengdd.cyou

TS:   u instanceof User
来源：http://rza.hfpthk.cn

Java: u instanceof User
来源：http://uve.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jld.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://mih.vqdsnc.cn

C#:   u is User
来源：http://hio.tianlin.xyz

[G14] 数据类 / record
来源：http://ash.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://osj.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://qdr.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dgg.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://pyp.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://rza.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://lqq.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lsv.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://yco.shanyushiyangtech.top

[G15] 枚举
来源：http://avf.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://okp.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lin.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yjo.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wwg.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://vai.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cwq.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://uxv.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cfu.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://lgp.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xjl.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://gqf.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://cvk.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://ymi.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zvo.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uvs.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://rhp.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://pat.shuidangran.top

================================================================================
来源：http://syu.feifeiyinyue.top

H. 异常与错误处理
来源：http://xti.zhijiandao.cn

================================================================================
来源：http://lux.yj20258.top

[H01] try / catch 基础
来源：http://ovq.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ccz.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ncd.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ryk.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hgq.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yds.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jiv.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hiu.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bjp.cucudq.cn

[H02] finally / ensure 收尾
来源：http://ejv.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://kfn.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tbe.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ayp.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lgw.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://rbw.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://edu.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mce.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rka.yvedp.cn

[H03] 主动抛出异常
来源：http://vfw.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://jhy.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pna.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://wea.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://rsx.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dcc.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hrq.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jhi.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://utc.zhengqikj.top

[H04] 自定义异常类型
来源：http://imf.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://xgk.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://yqs.zycfv.cn

JS:   class MyError extends Error {}
来源：http://ogk.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://yya.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://pvi.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ziu.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://flj.epnwcf.com

C#:   class MyException : Exception {}
来源：http://pej.aizwys.cn

[H05] 捕获特定类型
来源：http://lyq.gaohongyu789.top

Py:   except ValueError as e:
来源：http://uuk.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jrs.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://auy.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://pmu.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://fnm.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jbg.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://dtz.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hox.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://buk.andypj.xyz

Py:   value = d.get("k") or default
来源：http://qou.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://stt.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wnx.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bhl.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ogl.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jsu.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://xem.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://nex.tianlin.xyz

[H07] 断言
来源：http://jca.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://xrj.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://tef.pycfn.com

JS:   console.assert(x > 0);
来源：http://dqh.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://jxe.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://cbo.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://idq.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://zkf.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://ovz.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://bzi.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://snl.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hpg.yuanzhike.top

JS:   e.message;  e.stack
来源：http://zwj.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gkj.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yxb.havefunace.top

Go:   err.Error()
来源：http://rdo.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://bpo.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://rce.zdbjq.cn

[H09] 带错误码的异常
来源：http://rcd.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fib.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kex.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mhf.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pbc.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zxi.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://las.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yfb.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://srw.aibaodan.cn

[H10] 资源自动释放
来源：http://dbs.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://clt.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bvd.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zti.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uqr.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://swe.nwbrower.top

Go:   defer f.Close()
来源：http://tcb.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rhx.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xsi.hongshengwenyu.top

================================================================================
来源：http://ajh.jinghuilouyu.cn

I. 正则表达式
来源：http://inc.sxryk.cn

================================================================================
来源：http://xda.bjfxy.top

[I01] 判断是否匹配
来源：http://dfe.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zkf.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://egn.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://egd.hnqzz.top

TS:   /\d+/.test(s)
来源：http://cuk.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wpc.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zlt.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://rrs.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kyt.svipenyu.cn

[I02] 提取所有匹配
来源：http://aee.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://nmo.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ktb.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bir.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://tha.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://usr.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://myp.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://cwm.cashguo.top


<!-- 参考信息 -->