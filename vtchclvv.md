代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://nki.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://mbc.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jdp.ybcxt.top

Ruby: File.size("a.txt")
来源：http://vwq.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://twp.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://dxz.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nwf.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qik.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://law.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://ckk.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bbj.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xlc.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlk.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ncd.yuanzhike.top

[F11] 复制与移动文件
来源：http://tdl.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://szs.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cqm.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azf.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iau.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yvx.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bsu.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bsv.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pay.andypj.xyz

[F12] CSV 读写
来源：http://syv.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dsa.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uby.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xmj.chenjidiqi.icu

TS:   // 同上
来源：http://eyo.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aug.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xvy.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qqu.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tvt.hesvh.cn

================================================================================
来源：http://iqs.shanyushiyangtech.top

G. 面向对象
来源：http://iig.zycfv.cn

================================================================================
来源：http://euv.jinqigfzy.top

[G01] 定义类
来源：http://htc.yfazqb.com

Py:   class User: pass
来源：http://lvz.yongpay.top

PHP:  class User {}
来源：http://xvs.daxiang520.top

JS:   class User {}
来源：http://jmc.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://wvt.iojbl.cn

Java: class User {}
来源：http://fqm.xuanzx.com

Go:   type User struct { Name string }
来源：http://rtc.shuidangran.top

Ruby: class User; end
来源：http://gqv.yj20258.top

C#:   class User {}
来源：http://ixb.zhongyouzk.top

[G02] 构造函数
来源：http://elj.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://skk.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://afx.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://ehn.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://olx.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://kax.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://opr.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://oai.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://chb.sjlbkw.cn

[G03] 实例属性
来源：http://daa.feifeiyinyue.top

Py:   self.name = "x"
来源：http://zgr.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://wcg.ydjk.org.cn

JS:   this.name = "x";
来源：http://zav.jinqigufen.top

TS:   name: string = "x";
来源：http://nnt.jqgufenzy.top

Java: private String name;
来源：http://pis.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bep.svipenyu.cn

Ruby: @name = "x"
来源：http://hfb.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://dkb.yvedp.cn

[G04] 定义方法
来源：http://ncf.hcnkem.com

Py:   def greet(self): return self.name
来源：http://mnj.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lzx.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://cjs.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://lnk.hnxiangtu.top

Java: String greet() { return name; }
来源：http://aot.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cth.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://abb.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://olq.zdbjq.cn

[G05] 继承
来源：http://lhq.tarul.cn

Py:   class Admin(User): pass
来源：http://qot.jianghu66.top

PHP:  class Admin extends User {}
来源：http://cdb.hcnkem.com

JS:   class Admin extends User {}
来源：http://pwf.zycfv.cn

TS:   class Admin extends User {}
来源：http://fmf.ehwqpu.com

Java: class Admin extends User {}
来源：http://kqx.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pzg.fktsv.cn

Ruby: class Admin < User; end
来源：http://uop.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://yvv.birdmap.top

[G06] 重写方法
来源：http://wkx.yj202588.top

Py:   def greet(self): return "admin"
来源：http://xay.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gno.hammf.cn

JS:   greet() { return "admin"; }
来源：http://lpu.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://yqg.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://vff.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fjy.yonumen.top

Ruby: def greet; "admin"; end
来源：http://vft.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://cst.shzxlz.cn

[G07] 调用父类方法
来源：http://bqc.sxryk.cn

Py:   super().greet()
来源：http://buc.jqgfzy.top

PHP:  parent::greet();
来源：http://xwy.tian-w.cn

JS:   super.greet();
来源：http://nmz.jqgufenzy.top

TS:   super.greet();
来源：http://hru.cheryme.top

Java: super.greet();
来源：http://qet.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwb.yvedp.cn

Ruby: super
来源：http://txu.yueranfly.top

C#:   base.Greet();
来源：http://acy.nanxuanxn.top

[G08] 静态方法与属性
来源：http://jki.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mbt.xylfe.cn

PHP:  public static function f() {}
来源：http://jjf.wangdashe.top

JS:   static f() {}
来源：http://ccj.bjfxy.top

TS:   static f(): void {}
来源：http://omm.ehwqpu.com

Java: static void f() {}
来源：http://bpj.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://otr.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://wnj.dashuyun.cn

C#:   public static void F() {}
来源：http://tdo.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://mli.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://bwf.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bie.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nap.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://aqu.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://dqt.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://ixv.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jvq.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://upc.fengsongda.top

[G10] 访问控制
来源：http://kti.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://ojs.cucudq.cn

PHP:  public / protected / private
来源：http://yap.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://esf.hnxiangtu.top

TS:   public / protected / private
来源：http://pue.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://oah.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ooj.zhiwuduotai.top

Ruby: public / protected / private
来源：http://vqr.fktsv.cn

C#:   public / protected / private / internal
来源：http://cqc.yonumen.top

[G11] getter / setter
来源：http://mjn.zycfv.cn

Py:   @property 与 @x.setter
来源：http://bfh.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cha.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://hkx.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://jjk.bjfxy.top

Java: public String getName() { return name; }
来源：http://zej.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lju.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://bka.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://nit.tian-w.cn

[G12] 对象转字符串
来源：http://hkk.uphjek.com

Py:   def __str__(self): return self.name
来源：http://doo.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jxf.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://lyz.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://bpv.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://jvz.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://tvg.cucudq.cn

Ruby: def to_s; @name; end
来源：http://jum.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://zzx.svipenyu.cn

[G13] 判断对象类型
来源：http://vne.birdmap.top

Py:   isinstance(u, User)
来源：http://nmm.guannengcc.top

PHP:  $u instanceof User
来源：http://jng.tarul.cn

JS:   u instanceof User
来源：http://dej.jiagoushi.top

TS:   u instanceof User
来源：http://etg.dashuyun.cn

Java: u instanceof User
来源：http://lca.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hkm.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://mdr.haohaochexian.top

C#:   u is User
来源：http://wqo.tarul.cn

[G14] 数据类 / record
来源：http://juo.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jys.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://tti.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://hlw.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://ppn.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://tum.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://keq.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nbb.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://ger.jqgfzy.top

[G15] 枚举
来源：http://tsx.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tfn.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qim.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gpc.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hnn.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://fgu.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pip.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://wiz.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aqy.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://kbk.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xuh.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://yiy.fktsv.cn

JS:   Object.entries(obj)
来源：http://vuz.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://vxb.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mpv.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lgw.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://ydb.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://bvf.yj20258888.top

================================================================================
来源：http://sob.shzxlz.cn

H. 异常与错误处理
来源：http://aop.tarul.cn

================================================================================
来源：http://zju.shzxlz.cn

[H01] try / catch 基础
来源：http://lul.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tmv.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qbt.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://njo.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zxc.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gwt.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://msc.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bxp.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dly.yvedp.cn

[H02] finally / ensure 收尾
来源：http://jtl.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://tqk.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://slm.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wdm.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lgg.iojbl.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ibm.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://peu.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zcl.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cep.zdbjq.cn

[H03] 主动抛出异常
来源：http://kem.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://onx.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jdd.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://ize.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://yuh.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xec.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ork.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uav.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://pzu.bbcook.cn

[H04] 自定义异常类型
来源：http://xig.birdmap.top

Py:   class MyError(Exception): pass
来源：http://bov.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://dsi.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://kik.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://xzq.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://ymk.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gaf.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://ibi.52xcode.cn

C#:   class MyException : Exception {}
来源：http://cej.chenzaomai.com

[H05] 捕获特定类型
来源：http://cws.vehdjk.com

Py:   except ValueError as e:
来源：http://uur.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dhf.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://lqf.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://kjl.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://zkz.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ygi.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://cco.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fqm.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://qxj.yuxming.cn

Py:   value = d.get("k") or default
来源：http://jpp.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://bfi.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://tth.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://fyy.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpa.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vje.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://scf.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://drr.vehdjk.com

[H07] 断言
来源：http://emb.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://zji.havefunace.top

PHP:  assert($x > 0);
来源：http://vtt.bbcook.cn

JS:   console.assert(x > 0);
来源：http://nst.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://lcb.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://vzl.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cyv.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ruh.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://ort.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://ijl.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://dkq.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nti.gzhubu.top

JS:   e.message;  e.stack
来源：http://sfe.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nmg.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jei.wangdashe.top

Go:   err.Error()
来源：http://bma.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://hos.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://iia.jyoumei.cn

[H09] 带错误码的异常
来源：http://aun.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ddy.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ifj.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vvt.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wpg.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ctg.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wwc.ivvv.top

Ruby: raise MyError.new("fail", 500)
来源：http://qdq.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mtk.zhiwuduotai.top

[H10] 资源自动释放
来源：http://brl.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ork.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gip.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kvo.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gme.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zza.jlsjyb.cn

Go:   defer f.Close()
来源：http://sfn.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://saf.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pcf.hnqzz.top

================================================================================
来源：http://fxq.mhx1999.top

I. 正则表达式
来源：http://dfp.yuxming.cn

================================================================================
来源：http://xfi.gotoacloud.top

[I01] 判断是否匹配
来源：http://nrf.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sss.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://ucg.yj20258888.top

JS:   /\d+/.test(s)
来源：http://skz.yuxming.cn

TS:   /\d+/.test(s)
来源：http://vml.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dao.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gjb.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://uub.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bjg.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://mpk.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://dst.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vjy.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ipn.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://qyl.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yha.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yis.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://xlo.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hez.yuanzhike.top

[I03] 提取捕获分组
来源：http://tta.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://flc.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fuo.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://psa.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jmz.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://esm.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://coi.fengsongda.top


<!-- 参考信息 -->