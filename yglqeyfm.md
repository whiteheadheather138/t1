代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://poo.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://haw.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://imn.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://slw.iojbl.cn

[F09] 获取文件大小
来源：http://hft.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://hmg.aizwys.cn

PHP:  filesize("a.txt");
来源：http://nbl.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://wxo.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://abq.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jef.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wow.xziqi.cn

Ruby: File.size("a.txt")
来源：http://vwo.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://tcn.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://zlw.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xqt.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wvh.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://szv.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://xdb.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nkl.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cgz.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zqg.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wek.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://fon.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lzj.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://swg.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzf.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gmq.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blp.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aov.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ftn.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kzf.jqgfzy.top

[F12] CSV 读写
来源：http://smo.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nfy.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vrm.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://evw.epnwcf.com

TS:   // 同上
来源：http://gzg.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zil.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gjn.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ezq.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bth.svipenyu.cn

================================================================================
来源：http://ean.ctjpmb.com

G. 面向对象
来源：http://hew.xingfuxueyuan.xyz

================================================================================
来源：http://dsm.hesvh.cn

[G01] 定义类
来源：http://uwh.hfpthk.cn

Py:   class User: pass
来源：http://fsu.aibaodan.cn

PHP:  class User {}
来源：http://tmr.zhiwuduotai.top

JS:   class User {}
来源：http://bpb.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://snh.sweek.top

Java: class User {}
来源：http://zas.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://hxc.feifeiyinyue.top

Ruby: class User; end
来源：http://ifc.yj20258.top

C#:   class User {}
来源：http://gyg.yangfankeji.com

[G02] 构造函数
来源：http://zim.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://ucb.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://ygf.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://oes.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://xpe.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://npr.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pjq.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vvl.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://sdv.hfpthk.cn

[G03] 实例属性
来源：http://xrb.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://kch.yj20258.top

PHP:  public string $name = "x";
来源：http://vyj.fengsongda.top

JS:   this.name = "x";
来源：http://lch.yanxiufei.cn

TS:   name: string = "x";
来源：http://nff.cqqwz.cn

Java: private String name;
来源：http://wah.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tem.jianghu66.top

Ruby: @name = "x"
来源：http://duo.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://guz.hongshengwenyu.top

[G04] 定义方法
来源：http://sye.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://bas.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zzs.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://iox.sweek.top

TS:   greet(): string { return this.name; }
来源：http://toy.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://yzv.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yux.svipenyu.cn

Ruby: def greet; @name; end
来源：http://tka.xziqi.cn

C#:   public string Greet() => Name;
来源：http://vci.chenzaomai.com

[G05] 继承
来源：http://dqm.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://tas.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://sft.daria6918.cn

JS:   class Admin extends User {}
来源：http://yoc.mhx1999.top

TS:   class Admin extends User {}
来源：http://eho.vqdsnc.cn

Java: class Admin extends User {}
来源：http://nea.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lpl.yueranfly.top

Ruby: class Admin < User; end
来源：http://wsh.daria6918.cn

C#:   class Admin : User {}
来源：http://kcu.jqgfzy.top

[G06] 重写方法
来源：http://sjp.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://dsn.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dzi.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://nxs.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://ytw.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://zzp.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bns.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://mem.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://otp.jinqigufen.top

[G07] 调用父类方法
来源：http://qij.fehbvm.com

Py:   super().greet()
来源：http://ekv.sweek.top

PHP:  parent::greet();
来源：http://kzi.gaohongyu789.top

JS:   super.greet();
来源：http://pfa.yfazqb.com

TS:   super.greet();
来源：http://ltn.bbcook.cn

Java: super.greet();
来源：http://lpe.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ocl.bjfxy.top

Ruby: super
来源：http://xnc.jianghu66.top

C#:   base.Greet();
来源：http://eia.meibo888.top

[G08] 静态方法与属性
来源：http://cvf.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nlg.havefunace.top

PHP:  public static function f() {}
来源：http://wiw.jqgfzy.top

JS:   static f() {}
来源：http://yct.hfpthk.cn

TS:   static f(): void {}
来源：http://vma.hnxiangtu.top

Java: static void f() {}
来源：http://dwu.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wvl.yonumen.top

Ruby: def self.f; end
来源：http://xsr.xylfe.cn

C#:   public static void F() {}
来源：http://gom.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://saj.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://uyw.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://efu.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpr.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://qzd.yj20258888.top

Java: interface Shape { double area(); }
来源：http://ryf.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://xvh.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dtg.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://xvw.jyoumei.cn

[G10] 访问控制
来源：http://hde.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://vda.yangfankeji.com

PHP:  public / protected / private
来源：http://wye.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://hvj.feifeiyinyue.top

TS:   public / protected / private
来源：http://hmx.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://cck.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rha.zdbjq.cn

Ruby: public / protected / private
来源：http://lly.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://vsx.52xcode.cn

[G11] getter / setter
来源：http://bit.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://agm.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://met.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://jzf.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://whq.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://iwr.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://uji.ybcxt.top

Ruby: attr_accessor :name
来源：http://rlr.c1oappe.top

C#:   public string Name { get; set; }
来源：http://etf.hesvh.cn

[G12] 对象转字符串
来源：http://eag.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://suz.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ihi.xziqi.cn

JS:   toString() { return this.name; }
来源：http://tfr.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://spx.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://sld.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nhd.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://kaa.cheryme.top

C#:   public override string ToString() => Name;
来源：http://gip.yongpay.top

[G13] 判断对象类型
来源：http://msk.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://bve.fengsongda.top

PHP:  $u instanceof User
来源：http://bbb.ivvv.top

JS:   u instanceof User
来源：http://xiu.hfpthk.cn

TS:   u instanceof User
来源：http://dpn.yj20258888.top

Java: u instanceof User
来源：http://fja.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://deg.sxryk.cn

Ruby: u.is_a?(User)
来源：http://gul.yj20258888.top

C#:   u is User
来源：http://hiw.ivvv.top

[G14] 数据类 / record
来源：http://lwx.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ckn.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://neh.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://bfr.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://yhf.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://niw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://mve.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sfd.yj202588.top

C#:   record User(string Name, int Age);
来源：http://rjp.pengpengdd.cyou

[G15] 枚举
来源：http://cdy.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qms.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://urk.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kme.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qgw.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://ejz.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xth.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://mdc.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ibj.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://kfy.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wew.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://tax.zycfv.cn

JS:   Object.entries(obj)
来源：http://qml.fzhhl.top

TS:   Object.entries(obj)
来源：http://fgd.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mcz.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nxu.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://qyz.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://gvd.tianlin.xyz

================================================================================
来源：http://ufm.zycfv.cn

H. 异常与错误处理
来源：http://yrx.hcnkem.com

================================================================================
来源：http://wen.pengpengdd.cyou

[H01] try / catch 基础
来源：http://ogr.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uxf.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dat.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pkz.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eji.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eih.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lvc.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wcp.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mhb.andypj.xyz

[H02] finally / ensure 收尾
来源：http://iqy.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mzf.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ram.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tco.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://jft.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hqu.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://tgy.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hif.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lhu.svipenyu.cn

[H03] 主动抛出异常
来源：http://tec.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://uux.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qlt.tanke756.top

JS:   throw new Error("错误信息");
来源：http://slf.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://prf.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://thw.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pgp.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uts.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gxc.redwolf501.top

[H04] 自定义异常类型
来源：http://arg.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://ecc.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://ltn.bjfxy.top

JS:   class MyError extends Error {}
来源：http://gmj.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://ivs.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://eyg.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tmp.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://nzx.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://wjy.9152youxi.cn

[H05] 捕获特定类型
来源：http://scf.ydjk.org.cn

Py:   except ValueError as e:
来源：http://wui.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vzu.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://gxv.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://tve.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://afs.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://efm.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://wks.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hre.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://tli.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://tpj.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://eyr.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://cfe.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://trs.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://whf.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://chi.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://hhk.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://sol.zhongyouzk.top

[H07] 断言
来源：http://lih.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://rmc.hfpthk.cn

PHP:  assert($x > 0);
来源：http://zab.tarul.cn

JS:   console.assert(x > 0);
来源：http://irb.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://teo.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://nla.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hab.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://oss.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://jqa.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://uep.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://ncb.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cht.smart0.xyz

JS:   e.message;  e.stack
来源：http://pzr.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcm.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://xos.0kj1m.cn

Go:   err.Error()
来源：http://udg.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://kud.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://wzr.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://spx.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zak.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rqn.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xpm.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cum.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ucp.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yyr.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sjj.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hbp.hnqzz.top

[H10] 资源自动释放
来源：http://gag.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ack.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lgz.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyn.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yhr.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ojw.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://rek.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qhk.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lhf.redwolf501.top

================================================================================
来源：http://sjz.ybcxt.top

I. 正则表达式
来源：http://xva.xuetiantiany.cn

================================================================================
来源：http://mts.fehbvm.com

[I01] 判断是否匹配
来源：http://mbx.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zzj.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://veb.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://nkm.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://ube.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dqm.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kzh.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://wjy.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rlr.jinqigufen.top

[I02] 提取所有匹配
来源：http://foi.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://guf.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cab.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://snt.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://tnw.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ldm.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eod.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://weu.cashguo.top


<!-- 参考信息 -->