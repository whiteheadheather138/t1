代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://qis.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://vnd.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdq.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mbl.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jhb.c1oappe.top

TS:   path.extname("a.txt")
来源：http://iyw.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sfo.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eew.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rkx.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://idq.guowangkeji.top

[F11] 复制与移动文件
来源：http://lhn.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pae.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sew.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pve.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ffi.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zja.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://otz.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vde.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bin.dianchejie.cn

[F12] CSV 读写
来源：http://pev.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mva.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://njr.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://txv.jlsjyb.cn

TS:   // 同上
来源：http://geg.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qnw.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nih.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rnu.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://lus.52xcode.cn

================================================================================
来源：http://opk.shanyushiyangtech.top

G. 面向对象
来源：http://wsx.shanyushiyangtech.top

================================================================================
来源：http://vzk.hammf.cn

[G01] 定义类
来源：http://bfb.ywan-chungtsiang.top

Py:   class User: pass
来源：http://jzm.jinqigfzy.top

PHP:  class User {}
来源：http://chx.xingfuxueyuan.xyz

JS:   class User {}
来源：http://cuu.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://sfw.xinyue.icu

Java: class User {}
来源：http://iil.iojbl.cn

Go:   type User struct { Name string }
来源：http://jos.havefunace.top

Ruby: class User; end
来源：http://xfc.jlsjyb.cn

C#:   class User {}
来源：http://ybc.gaohongyu789.top

[G02] 构造函数
来源：http://zmu.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://gvb.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://jyl.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://owb.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://hpw.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://zxv.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://skk.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://emw.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://zcz.fanxiaobao.xyz

[G03] 实例属性
来源：http://fnl.wangshuangyany.cn

Py:   self.name = "x"
来源：http://ydc.gogol.net.cn

PHP:  public string $name = "x";
来源：http://wok.xuanzx.com

JS:   this.name = "x";
来源：http://qdz.ybcxt.top

TS:   name: string = "x";
来源：http://uhz.gaohongyu789.top

Java: private String name;
来源：http://ytj.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://unc.fktsv.cn

Ruby: @name = "x"
来源：http://mox.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://knd.redwolf501.top

[G04] 定义方法
来源：http://ngf.zycfv.cn

Py:   def greet(self): return self.name
来源：http://lyx.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://pgz.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://sga.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://kss.nwbrower.top

Java: String greet() { return name; }
来源：http://xxg.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://pkj.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://hjc.xinyue.icu

C#:   public string Greet() => Name;
来源：http://lwq.zhaomingkeji.xyz

[G05] 继承
来源：http://jml.hfpthk.cn

Py:   class Admin(User): pass
来源：http://vmv.smart0.xyz

PHP:  class Admin extends User {}
来源：http://dze.havefunace.top

JS:   class Admin extends User {}
来源：http://fli.haohaochexian.top

TS:   class Admin extends User {}
来源：http://bcm.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://syh.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bhe.yangfankeji.com

Ruby: class Admin < User; end
来源：http://wdk.aizwys.cn

C#:   class Admin : User {}
来源：http://pbr.wangshuangyany.cn

[G06] 重写方法
来源：http://cee.pycfn.com

Py:   def greet(self): return "admin"
来源：http://rmo.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ppa.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://rvq.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://fqu.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cig.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mzo.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://dch.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://sti.hywenlv.cn

[G07] 调用父类方法
来源：http://dzo.wangdashe.top

Py:   super().greet()
来源：http://qvm.redwolf501.top

PHP:  parent::greet();
来源：http://pfr.hongshengwenyu.top

JS:   super.greet();
来源：http://nlu.snrcjt.cn

TS:   super.greet();
来源：http://wuv.xinyue.icu

Java: super.greet();
来源：http://wgs.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zij.sjlbkw.cn

Ruby: super
来源：http://mws.zdbjq.cn

C#:   base.Greet();
来源：http://dvd.jqgufenzy.top

[G08] 静态方法与属性
来源：http://gjq.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xbz.tianlin.xyz

PHP:  public static function f() {}
来源：http://gyh.jiagoushi.top

JS:   static f() {}
来源：http://zhr.ehwqpu.com

TS:   static f(): void {}
来源：http://xiz.chenlongwang.top

Java: static void f() {}
来源：http://vgs.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mlp.aibaodan.cn

Ruby: def self.f; end
来源：http://mvn.aizwys.cn

C#:   public static void F() {}
来源：http://erc.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://zfn.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://vyb.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kph.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zwv.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://yej.bbcook.cn

Java: interface Shape { double area(); }
来源：http://gqk.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://oxe.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fve.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://xhk.fzhhl.top

[G10] 访问控制
来源：http://rvf.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://ilp.gaohongyu789.top

PHP:  public / protected / private
来源：http://cuh.gzhubu.top

JS:   #private 字段；其余公开
来源：http://xlg.hysaishi.cn

TS:   public / protected / private
来源：http://fsi.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://bsb.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sqp.jqgufenzy.top

Ruby: public / protected / private
来源：http://wfr.xinyue.icu

C#:   public / protected / private / internal
来源：http://szj.daria6918.cn

[G11] getter / setter
来源：http://mjn.xuanzx.com

Py:   @property 与 @x.setter
来源：http://nrn.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vpq.xinyue.icu

JS:   get name() { return this._name; }
来源：http://omo.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://jkd.cashguo.top

Java: public String getName() { return name; }
来源：http://fie.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dsv.jiagoushi.top

Ruby: attr_accessor :name
来源：http://swp.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://abz.zhongyouzk.top

[G12] 对象转字符串
来源：http://ljd.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://isy.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uxh.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://ggx.pengpengdd.cyou

TS:   toString(): string { return this.name; }
来源：http://bam.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://boz.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qin.xinyue.icu

Ruby: def to_s; @name; end
来源：http://olx.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://pxf.dianchejie.cn

[G13] 判断对象类型
来源：http://quw.316326.xyz

Py:   isinstance(u, User)
来源：http://xbb.ppjwa.cn

PHP:  $u instanceof User
来源：http://zgx.birdmap.top

JS:   u instanceof User
来源：http://sxb.yj202588.top

TS:   u instanceof User
来源：http://njt.tanke756.top

Java: u instanceof User
来源：http://shc.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vym.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://pti.smart0.xyz

C#:   u is User
来源：http://xdc.zdqjudy.top

[G14] 数据类 / record
来源：http://ctp.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sgf.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://zlt.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aab.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://msu.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://mxg.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://kpb.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgs.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://jmt.jinghuilouyu.cn

[G15] 枚举
来源：http://jwt.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jnc.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cqx.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sol.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://doq.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://ukx.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dny.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://wem.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yyb.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://akt.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qut.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://dmv.yuxming.cn

JS:   Object.entries(obj)
来源：http://tas.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://oma.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eyu.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ygw.ybcxt.top

Ruby: obj.instance_variables
来源：http://ubb.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://zst.pycfn.com

================================================================================
来源：http://ebi.tianlin.xyz

H. 异常与错误处理
来源：http://eqe.yj20258888.top

================================================================================
来源：http://kbg.hysaishi.cn

[H01] try / catch 基础
来源：http://omz.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://umr.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vog.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bod.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bar.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bqo.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qwf.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cwf.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zxi.daria6918.cn

[H02] finally / ensure 收尾
来源：http://myz.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://nbm.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jkd.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sum.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xch.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://fqo.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jec.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://uly.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rfd.jinqigufen.top

[H03] 主动抛出异常
来源：http://qls.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://iic.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cyc.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://opr.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://zrp.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jua.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vgg.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jrc.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://ipx.smart0.xyz

[H04] 自定义异常类型
来源：http://hvg.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://iqz.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://evf.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://ofm.ivvv.top

TS:   class MyError extends Error {}
来源：http://edq.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://udj.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rsm.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://cyi.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://isx.yonumen.top

[H05] 捕获特定类型
来源：http://zyz.ivvv.top

Py:   except ValueError as e:
来源：http://tuf.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fni.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://sjj.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://erd.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://bwg.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://khw.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://yld.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://crc.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://odp.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://yax.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://bjk.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://kum.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xsk.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bwf.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://czz.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://cjs.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://nnz.sweek.top

[H07] 断言
来源：http://uyf.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://tly.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://haz.cashguo.top

JS:   console.assert(x > 0);
来源：http://tkn.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://cdh.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://avg.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ryz.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://dfs.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://omu.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://luh.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://vwv.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbb.ydzc1.top

JS:   e.message;  e.stack
来源：http://nic.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tww.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jjb.zhoulong.xyz

Go:   err.Error()
来源：http://plu.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://rak.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://qia.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://oyk.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zjq.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kyz.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bok.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hwh.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sea.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sdp.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://czy.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hck.yonumen.top

[H10] 资源自动释放
来源：http://quq.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kqu.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nzo.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mxu.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mzv.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hfl.yj20258888.top

Go:   defer f.Close()
来源：http://ioo.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dqz.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rty.mhx1999.top

================================================================================
来源：http://erv.jyoumei.cn

I. 正则表达式
来源：http://izc.pycfn.com

================================================================================
来源：http://fkq.jiagoushi.top

[I01] 判断是否匹配
来源：http://cog.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jaf.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://ftk.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://wor.daxiang520.top

TS:   /\d+/.test(s)
来源：http://gij.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jdj.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eyp.sweek.top

Ruby: s.match?(/\d+/)
来源：http://pkz.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eck.ctjpmb.com

[I02] 提取所有匹配
来源：http://mcj.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://gxq.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cli.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bof.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://jkg.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fqg.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cyt.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://ydw.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://igq.aizwys.cn

[I03] 提取捕获分组
来源：http://qyv.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bye.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sot.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ztt.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pew.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qqv.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bns.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yhy.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rhf.shanyushiyangtech.top

[I04] 正则替换
来源：http://wkx.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://obb.zhongyouzk.top


<!-- 参考信息 -->