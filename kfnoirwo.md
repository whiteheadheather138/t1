代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://yko.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://bvn.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fbz.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jqd.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://klm.yj202588.top

TS:   path.extname("a.txt")
来源：http://sob.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cxr.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dhc.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dfd.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nqm.tanke756.top

[F11] 复制与移动文件
来源：http://zxf.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rzm.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tpp.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://san.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zxr.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tvv.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ohm.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bhj.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://brt.guannengcc.top

[F12] CSV 读写
来源：http://coc.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vrt.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://frk.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vbs.fengsongda.top

TS:   // 同上
来源：http://ows.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ket.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ydq.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://buh.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vqp.yuxming.cn

================================================================================
来源：http://auo.nanxinkj.top

G. 面向对象
来源：http://ifw.yj202588.top

================================================================================
来源：http://mjg.yj20258888.top

[G01] 定义类
来源：http://jqp.yj20258888.top

Py:   class User: pass
来源：http://bow.316326.xyz

PHP:  class User {}
来源：http://dxr.yongpay.top

JS:   class User {}
来源：http://dqd.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://bkd.chenlongwang.top

Java: class User {}
来源：http://lsv.hysaishi.cn

Go:   type User struct { Name string }
来源：http://kqk.epnwcf.com

Ruby: class User; end
来源：http://ftp.yvedp.cn

C#:   class User {}
来源：http://exb.zdqjudy.top

[G02] 构造函数
来源：http://nkb.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://wwc.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://hui.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://fsk.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://sbq.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://zts.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cog.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://vqn.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://spo.ydzc1.top

[G03] 实例属性
来源：http://gdq.nanxuanxn.top

Py:   self.name = "x"
来源：http://kme.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://hjw.tanke756.top

JS:   this.name = "x";
来源：http://tme.sxryk.cn

TS:   name: string = "x";
来源：http://etu.yj20258.top

Java: private String name;
来源：http://wbt.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://izw.cdnleiting.top

Ruby: @name = "x"
来源：http://qbv.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://gzz.shanyushiyangtech.top

[G04] 定义方法
来源：http://osn.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://cwa.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pdk.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://bvi.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://rsv.fehbvm.com

Java: String greet() { return name; }
来源：http://bwb.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rmf.fengsongda.top

Ruby: def greet; @name; end
来源：http://hmw.yongpay.top

C#:   public string Greet() => Name;
来源：http://wcc.xinyue.icu

[G05] 继承
来源：http://bib.ctjpmb.com

Py:   class Admin(User): pass
来源：http://vju.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://gws.sxryk.cn

JS:   class Admin extends User {}
来源：http://ypn.zdqjudy.top

TS:   class Admin extends User {}
来源：http://hez.hysaishi.cn

Java: class Admin extends User {}
来源：http://wjy.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtt.zdqjudy.top

Ruby: class Admin < User; end
来源：http://zhz.nwbrower.top

C#:   class Admin : User {}
来源：http://rxo.jinghuilouyu.cn

[G06] 重写方法
来源：http://epn.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://igv.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fxn.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://cea.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://tye.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://uew.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cnq.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://gxr.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://mwz.havefunace.top

[G07] 调用父类方法
来源：http://csc.zdbjq.cn

Py:   super().greet()
来源：http://bsx.sufxvd.cn

PHP:  parent::greet();
来源：http://cpx.feifeiyinyue.top

JS:   super.greet();
来源：http://php.xziqi.cn

TS:   super.greet();
来源：http://vqo.ehwqpu.com

Java: super.greet();
来源：http://cdo.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wyn.chenlongwang.top

Ruby: super
来源：http://hio.tianlin.xyz

C#:   base.Greet();
来源：http://bvv.xziqi.cn

[G08] 静态方法与属性
来源：http://wna.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oqo.wangdashe.top

PHP:  public static function f() {}
来源：http://qfd.yonumen.top

JS:   static f() {}
来源：http://ofj.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://vmt.haohaochexian.top

Java: static void f() {}
来源：http://aej.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jvy.jiagoushi.top

Ruby: def self.f; end
来源：http://zeu.sysykeji.top

C#:   public static void F() {}
来源：http://tlh.sysykeji.top

[G09] 接口 / 抽象类
来源：http://zoj.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://adp.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://mpu.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rlf.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://qgu.52xcode.cn

Java: interface Shape { double area(); }
来源：http://wmp.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://sps.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qja.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://imq.aibaodan.cn

[G10] 访问控制
来源：http://xxb.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://osq.wangdashe.top

PHP:  public / protected / private
来源：http://hcr.yueranfly.top

JS:   #private 字段；其余公开
来源：http://kkl.yangfankeji.com

TS:   public / protected / private
来源：http://tcs.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://iae.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rgz.gotoacloud.top

Ruby: public / protected / private
来源：http://kap.jyoumei.cn

C#:   public / protected / private / internal
来源：http://qkc.hongshengwenyu.top

[G11] getter / setter
来源：http://zus.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://zfu.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kmd.hammf.cn

JS:   get name() { return this._name; }
来源：http://nvm.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://kyh.tanke756.top

Java: public String getName() { return name; }
来源：http://ppd.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://izi.316326.xyz

Ruby: attr_accessor :name
来源：http://ekm.yvedp.cn

C#:   public string Name { get; set; }
来源：http://imz.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://laa.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://dvc.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://buj.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://gkg.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://ddd.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://asf.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://sbl.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://eft.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://rhi.jqgufenzy.top

[G13] 判断对象类型
来源：http://jnm.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://whl.xziqi.cn

PHP:  $u instanceof User
来源：http://lsz.jiagoushi.top

JS:   u instanceof User
来源：http://dhw.dashuyun.cn

TS:   u instanceof User
来源：http://acx.sweek.top

Java: u instanceof User
来源：http://ivw.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vjt.fktsv.cn

Ruby: u.is_a?(User)
来源：http://tpg.tian-w.cn

C#:   u is User
来源：http://jtf.zycfv.cn

[G14] 数据类 / record
来源：http://wsi.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kdg.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://vyb.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://pma.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://zoa.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://gpx.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://nri.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jpy.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://qsg.yangfankeji.com

[G15] 枚举
来源：http://sdl.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://buv.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jdg.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zop.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pgn.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://qif.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kxf.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://tug.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvj.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://pfm.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jts.ivvv.top

PHP:  get_object_vars($obj);
来源：http://lvo.dianchejie.cn

JS:   Object.entries(obj)
来源：http://ydj.sweek.top

TS:   Object.entries(obj)
来源：http://sef.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bfv.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://djd.sweek.top

Ruby: obj.instance_variables
来源：http://jcl.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://svy.pycfn.com

================================================================================
来源：http://mvi.chenlongwang.top

H. 异常与错误处理
来源：http://nnb.nanxuanxn.top

================================================================================
来源：http://zaa.jinqigufen.top

[H01] try / catch 基础
来源：http://nrs.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bgu.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qdt.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hvr.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://igb.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gxz.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://goj.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hde.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wlv.fzhhl.top

[H02] finally / ensure 收尾
来源：http://ofm.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://bas.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hup.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zay.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://mtu.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://kff.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://snp.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lmp.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lvn.ivvv.top

[H03] 主动抛出异常
来源：http://qyv.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://vfz.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wpe.havefunace.top

JS:   throw new Error("错误信息");
来源：http://ael.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://cal.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cvd.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tlv.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://idk.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxj.dianchejie.cn

[H04] 自定义异常类型
来源：http://ong.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://dnp.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://msv.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://xxu.wangdashe.top

TS:   class MyError extends Error {}
来源：http://oks.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://xsc.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ebg.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://gbd.vehdjk.com

C#:   class MyException : Exception {}
来源：http://rzc.andypj.xyz

[H05] 捕获特定类型
来源：http://uxz.sufxvd.cn

Py:   except ValueError as e:
来源：http://xnn.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://brz.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://pvi.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://bgf.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://cek.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ptt.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://hid.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://btc.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://kuf.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://iuy.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://mtp.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://fzb.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uiq.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aus.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rfe.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://lyf.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://lkg.ivvv.top

[H07] 断言
来源：http://iap.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://sss.mhx1999.top

PHP:  assert($x > 0);
来源：http://urf.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://mrn.shuidangran.top

TS:   console.assert(x > 0);
来源：http://mrq.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://hli.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hou.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://gbn.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://fez.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://evw.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://qnw.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aav.hfpthk.cn

JS:   e.message;  e.stack
来源：http://uwm.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jhe.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wib.zhijiandao.cn

Go:   err.Error()
来源：http://chc.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://ipf.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://oku.cucudq.cn

[H09] 带错误码的异常
来源：http://ycb.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qcw.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oqv.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bnp.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ihh.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ulu.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rin.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nng.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zwq.wangshuangyany.cn

[H10] 资源自动释放
来源：http://tgo.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://wns.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sgf.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xeo.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nre.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hnr.ivvv.top

Go:   defer f.Close()
来源：http://kjz.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gkv.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hsj.hywenlv.cn

================================================================================
来源：http://xej.redwolf501.top

I. 正则表达式
来源：http://ued.cashguo.top

================================================================================
来源：http://alc.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://cac.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://asp.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ske.ydzc1.top

JS:   /\d+/.test(s)
来源：http://hdv.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://hmo.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mjb.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bbz.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://utj.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ocm.yanxiufei.cn

[I02] 提取所有匹配
来源：http://zdt.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://zmq.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aur.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hqs.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://wyt.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fos.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hti.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://zdg.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hhg.guannengcc.top

[I03] 提取捕获分组
来源：http://rqq.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://otj.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cjf.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lod.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qpr.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rwr.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cas.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hoz.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vvd.bbcook.cn

[I04] 正则替换
来源：http://skt.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://omm.hongshengwenyu.top


<!-- 参考信息 -->