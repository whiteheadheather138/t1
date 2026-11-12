代发 wailian999

[F09] 获取文件大小
来源：http://tgb.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://fnf.xylfe.cn

PHP:  filesize("a.txt");
来源：http://yql.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://rrr.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://vly.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xbq.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yrz.yj20258888.top

Ruby: File.size("a.txt")
来源：http://oor.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://fsf.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://ywq.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://afw.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tka.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kmz.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://pjx.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://plc.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://leb.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gxs.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sng.hywenlv.cn

[F11] 复制与移动文件
来源：http://fud.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pgr.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jrj.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lcp.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gkq.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lxd.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ssy.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ywd.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fyz.kuanghao11.cn

[F12] CSV 读写
来源：http://vkq.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wgm.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ion.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mao.sysykeji.top

TS:   // 同上
来源：http://etu.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tdo.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://odf.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tsd.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vbx.daxiang520.top

================================================================================
来源：http://peb.nwbrower.top

G. 面向对象
来源：http://pvy.yfazqb.com

================================================================================
来源：http://qkk.hnqzz.top

[G01] 定义类
来源：http://nms.jianghu66.top

Py:   class User: pass
来源：http://lix.feifeiyinyue.top

PHP:  class User {}
来源：http://fry.yfazqb.com

JS:   class User {}
来源：http://kuh.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://zeg.snrcjt.cn

Java: class User {}
来源：http://uuy.cqqwz.cn

Go:   type User struct { Name string }
来源：http://tcf.9152youxi.cn

Ruby: class User; end
来源：http://wjt.hnxiangtu.top

C#:   class User {}
来源：http://eag.haohaochexian.top

[G02] 构造函数
来源：http://ivv.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://dsp.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://pfm.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://qma.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://bzi.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://dzi.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpz.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://kwu.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://emk.quarkkingdee.top

[G03] 实例属性
来源：http://wvz.cucudq.cn

Py:   self.name = "x"
来源：http://tgo.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://gcq.yanxiufei.cn

JS:   this.name = "x";
来源：http://zsb.tian-w.cn

TS:   name: string = "x";
来源：http://few.pengpengdd.cyou

Java: private String name;
来源：http://rje.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oqe.yanxiufei.cn

Ruby: @name = "x"
来源：http://xhn.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://amf.gotoacloud.top

[G04] 定义方法
来源：http://tky.xylfe.cn

Py:   def greet(self): return self.name
来源：http://gro.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hgi.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://myj.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://exv.jqgfzy.top

Java: String greet() { return name; }
来源：http://syj.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ckz.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://ezn.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://bxv.feifeiyinyue.top

[G05] 继承
来源：http://wme.yuanzhike.top

Py:   class Admin(User): pass
来源：http://gul.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://sqa.guannengcc.top

JS:   class Admin extends User {}
来源：http://xyf.cqqwz.cn

TS:   class Admin extends User {}
来源：http://tux.aibaodan.cn

Java: class Admin extends User {}
来源：http://hcp.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lwh.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://ysn.bbcook.cn

C#:   class Admin : User {}
来源：http://ivk.dianchejie.cn

[G06] 重写方法
来源：http://vgm.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://phi.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nwe.cashguo.top

JS:   greet() { return "admin"; }
来源：http://vrc.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://eag.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://adz.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qde.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://trr.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://xfl.yj20258888.top

[G07] 调用父类方法
来源：http://zkr.zhixingplan.top

Py:   super().greet()
来源：http://hdv.yj20258.top

PHP:  parent::greet();
来源：http://pbk.c1oappe.top

JS:   super.greet();
来源：http://tqw.yongpay.top

TS:   super.greet();
来源：http://cjo.shuidangran.top

Java: super.greet();
来源：http://esm.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xjy.pycfn.com

Ruby: super
来源：http://tvs.gogol.net.cn

C#:   base.Greet();
来源：http://exy.daria6918.cn

[G08] 静态方法与属性
来源：http://xfx.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qwu.zhengqikj.top

PHP:  public static function f() {}
来源：http://cqa.jyoumei.cn

JS:   static f() {}
来源：http://dnl.chenlongwang.top

TS:   static f(): void {}
来源：http://mgd.dianchejie.cn

Java: static void f() {}
来源：http://ttx.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hoy.zhixingplan.top

Ruby: def self.f; end
来源：http://hxp.chenzaomai.com

C#:   public static void F() {}
来源：http://xba.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://aej.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://lik.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://fyg.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jxz.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://ckv.hnqzz.top

Java: interface Shape { double area(); }
来源：http://gcm.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://klp.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ksa.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://pra.meibo888.top

[G10] 访问控制
来源：http://rzc.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://fbt.yonumen.top

PHP:  public / protected / private
来源：http://ilh.uphjek.com

JS:   #private 字段；其余公开
来源：http://aav.yfazqb.com

TS:   public / protected / private
来源：http://fub.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://kup.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://adm.jinqigufen.top

Ruby: public / protected / private
来源：http://dgl.316326.xyz

C#:   public / protected / private / internal
来源：http://krt.jyoumei.cn

[G11] getter / setter
来源：http://cxs.xinyue.icu

Py:   @property 与 @x.setter
来源：http://nfs.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sxr.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://fjl.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://wvj.sweek.top

Java: public String getName() { return name; }
来源：http://gjq.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lse.fzhhl.top

Ruby: attr_accessor :name
来源：http://zeh.hcnkem.com

C#:   public string Name { get; set; }
来源：http://qyt.cheryme.top

[G12] 对象转字符串
来源：http://nah.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://tco.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pxi.guannengcc.top

JS:   toString() { return this.name; }
来源：http://rui.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://aec.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://zdz.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://pid.xuanzx.com

Ruby: def to_s; @name; end
来源：http://rep.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://waz.aibaodan.cn

[G13] 判断对象类型
来源：http://kff.yangfankeji.com

Py:   isinstance(u, User)
来源：http://keh.dashuyun.cn

PHP:  $u instanceof User
来源：http://fov.smart0.xyz

JS:   u instanceof User
来源：http://bhg.hnxiangtu.top

TS:   u instanceof User
来源：http://nzq.yuanzhike.top

Java: u instanceof User
来源：http://knb.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hho.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://jdo.shangyingyoupin.top

C#:   u is User
来源：http://mpw.xinyue.icu

[G14] 数据类 / record
来源：http://lrr.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zzn.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://bpx.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ypw.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://unf.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://yqe.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://joz.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uwv.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://axi.zhiwuduotai.top

[G15] 枚举
来源：http://gur.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nhl.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://kyp.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eou.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fta.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://oyk.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axc.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://eye.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bry.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://per.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://upd.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://pnz.tarul.cn

JS:   Object.entries(obj)
来源：http://ktn.ehwqpu.com

TS:   Object.entries(obj)
来源：http://txc.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wnv.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zkf.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://ack.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://pqb.yj20258.top

================================================================================
来源：http://yye.jianghu66.top

H. 异常与错误处理
来源：http://gcz.vqdsnc.cn

================================================================================
来源：http://rlx.svipenyu.cn

[H01] try / catch 基础
来源：http://flb.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uap.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rcg.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wme.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pet.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jvw.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jno.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lss.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kfl.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://uzn.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://cah.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cfr.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ktc.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qup.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://yht.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfy.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wzj.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lsz.hysaishi.cn

[H03] 主动抛出异常
来源：http://omg.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://hbp.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://csl.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://ryb.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://kvm.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://myp.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ret.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hts.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lpn.sjlbkw.cn

[H04] 自定义异常类型
来源：http://xwz.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://xdr.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://wll.cashguo.top

JS:   class MyError extends Error {}
来源：http://rag.yueranfly.top

TS:   class MyError extends Error {}
来源：http://tob.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://jmz.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zbf.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://mkh.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://tar.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://eem.ehwqpu.com

Py:   except ValueError as e:
来源：http://ixp.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bmp.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://skw.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://quy.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://xlt.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nip.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://qpk.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aty.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://sxe.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://ffw.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://iat.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://evs.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://joa.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qhq.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bzg.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://uwz.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://vjn.jianghu66.top

[H07] 断言
来源：http://lur.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://gux.ctjpmb.com

PHP:  assert($x > 0);
来源：http://jyh.ybcxt.top

JS:   console.assert(x > 0);
来源：http://evx.jianghu66.top

TS:   console.assert(x > 0);
来源：http://ekt.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://zbr.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nnr.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vmw.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://icx.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://jgd.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://zmu.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jqf.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://fvl.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://she.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qnd.hcnkem.com

Go:   err.Error()
来源：http://xgl.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://lqj.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://xlb.jqgfzy.top

[H09] 带错误码的异常
来源：http://vai.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gwk.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lhj.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iyt.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ulr.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nfm.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uor.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://nxo.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ajd.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://ihd.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yrp.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dyq.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qxw.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ftv.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pst.zhixingplan.top

Go:   defer f.Close()
来源：http://zxd.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pie.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mwn.xinyue.icu

================================================================================
来源：http://gem.dianchejie.cn

I. 正则表达式
来源：http://ojv.snrcjt.cn

================================================================================
来源：http://mtj.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://rfv.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lbk.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://xlk.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://tmh.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://zwq.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ltw.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://enu.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://rey.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wuy.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://bqr.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://afg.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ubv.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hmt.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://sib.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jsd.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pua.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://rei.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gat.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://oaf.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zua.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mhr.pycfn.com


<!-- 参考信息 -->