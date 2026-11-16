代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drz.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wyd.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yfj.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jvw.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cxn.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ned.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wnz.gotoacloud.top

[F08] 遍历目录
来源：http://ysm.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://djq.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fyi.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://wyq.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://tny.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bnm.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://txo.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://xmi.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://whg.quarkkingdee.top

[F09] 获取文件大小
来源：http://wrh.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://dil.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://jtu.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://fjj.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://npv.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://nuu.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swp.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://odz.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://abu.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://sgc.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kjn.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jon.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxy.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://nur.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fsb.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sct.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mwg.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fzw.ivvv.top

[F11] 复制与移动文件
来源：http://pfi.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rey.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yms.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zjs.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ald.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cjb.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://heu.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zcj.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yzf.cashguo.top

[F12] CSV 读写
来源：http://mkz.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ehr.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://all.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ndy.zhongyouzk.top

TS:   // 同上
来源：http://vql.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hig.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tqc.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hxa.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lje.hammf.cn

================================================================================
来源：http://zpi.guowangkeji.top

G. 面向对象
来源：http://xdt.fktsv.cn

================================================================================
来源：http://vrw.gotoacloud.top

[G01] 定义类
来源：http://vnv.shuidangran.top

Py:   class User: pass
来源：http://iot.dianchejie.cn

PHP:  class User {}
来源：http://rdp.yanxiufei.cn

JS:   class User {}
来源：http://ayb.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://bfn.jlsjyb.cn

Java: class User {}
来源：http://fgk.daxiang520.top

Go:   type User struct { Name string }
来源：http://tii.jiagoushi.top

Ruby: class User; end
来源：http://gqc.xuanzx.com

C#:   class User {}
来源：http://vbc.gotoacloud.top

[G02] 构造函数
来源：http://ewh.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://yiv.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://zuw.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ezx.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://npt.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://tix.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tms.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://fqo.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://upo.zhijiandao.cn

[G03] 实例属性
来源：http://vlj.vqdsnc.cn

Py:   self.name = "x"
来源：http://btu.ybcxt.top

PHP:  public string $name = "x";
来源：http://lnk.yuanzhike.top

JS:   this.name = "x";
来源：http://sss.yvedp.cn

TS:   name: string = "x";
来源：http://htn.birdmap.top

Java: private String name;
来源：http://fqd.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aly.redwolf501.top

Ruby: @name = "x"
来源：http://cur.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://hsa.epnwcf.com

[G04] 定义方法
来源：http://xbx.smart0.xyz

Py:   def greet(self): return self.name
来源：http://ebn.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pag.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://kaq.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://lvg.pycfn.com

Java: String greet() { return name; }
来源：http://uwt.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkn.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://nfy.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://ffc.jqgufenzy.top

[G05] 继承
来源：http://njr.svipenyu.cn

Py:   class Admin(User): pass
来源：http://glo.pycfn.com

PHP:  class Admin extends User {}
来源：http://myb.yfazqb.com

JS:   class Admin extends User {}
来源：http://eey.52xcode.cn

TS:   class Admin extends User {}
来源：http://ndb.hywenlv.cn

Java: class Admin extends User {}
来源：http://jao.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vny.yongpay.top

Ruby: class Admin < User; end
来源：http://lhn.birdmap.top

C#:   class Admin : User {}
来源：http://vbz.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://smu.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://vyq.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hfp.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://aud.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://bca.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://tkr.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cda.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://vvc.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://ljt.jinqigfzy.top

[G07] 调用父类方法
来源：http://ybn.zhixingplan.top

Py:   super().greet()
来源：http://otn.yfazqb.com

PHP:  parent::greet();
来源：http://iqb.bbcook.cn

JS:   super.greet();
来源：http://ibs.daxiang520.top

TS:   super.greet();
来源：http://jla.yangfankeji.com

Java: super.greet();
来源：http://sjs.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmb.yvedp.cn

Ruby: super
来源：http://qgd.ppjwa.cn

C#:   base.Greet();
来源：http://ytf.ybcxt.top

[G08] 静态方法与属性
来源：http://gmd.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kvo.cdnleiting.top

PHP:  public static function f() {}
来源：http://fum.zhoulong.xyz

JS:   static f() {}
来源：http://fso.shangyingyoupin.top

TS:   static f(): void {}
来源：http://zwh.andypj.xyz

Java: static void f() {}
来源：http://kjh.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qlj.bjfxy.top

Ruby: def self.f; end
来源：http://erh.shangyingyoupin.top

C#:   public static void F() {}
来源：http://kki.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://yqt.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://svw.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://ahw.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hjt.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://eri.tian-w.cn

Java: interface Shape { double area(); }
来源：http://tlj.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://urz.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sck.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://sgl.chenzaomai.com

[G10] 访问控制
来源：http://wdl.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://smj.ppjwa.cn

PHP:  public / protected / private
来源：http://oto.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://cdx.hammf.cn

TS:   public / protected / private
来源：http://idj.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://mep.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lcm.yj20258888.top

Ruby: public / protected / private
来源：http://yih.hysaishi.cn

C#:   public / protected / private / internal
来源：http://owr.vehdjk.com

[G11] getter / setter
来源：http://tvg.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://pbl.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fdv.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://kqw.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://sun.sweek.top

Java: public String getName() { return name; }
来源：http://sdn.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hkq.zhengqikj.top

Ruby: attr_accessor :name
来源：http://vne.meibo888.top

C#:   public string Name { get; set; }
来源：http://qzg.ppjwa.cn

[G12] 对象转字符串
来源：http://zfc.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://yvs.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffb.aizwys.cn

JS:   toString() { return this.name; }
来源：http://fzw.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://wua.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://tlc.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://lgb.yj20258888.top

Ruby: def to_s; @name; end
来源：http://icp.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://iik.sxryk.cn

[G13] 判断对象类型
来源：http://agt.9152youxi.cn

Py:   isinstance(u, User)
来源：http://glv.smart0.xyz

PHP:  $u instanceof User
来源：http://unk.pycfn.com

JS:   u instanceof User
来源：http://omh.yuxming.cn

TS:   u instanceof User
来源：http://pma.redwolf501.top

Java: u instanceof User
来源：http://zwc.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozj.xylfe.cn

Ruby: u.is_a?(User)
来源：http://mhj.pycfn.com

C#:   u is User
来源：http://eeq.shangyingyoupin.top

[G14] 数据类 / record
来源：http://nbb.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://alu.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://jkc.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yog.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://vci.52xcode.cn

Java: record User(String name, int age) {}
来源：http://tpp.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://psx.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ugx.yongpay.top

C#:   record User(string Name, int Age);
来源：http://anl.hammf.cn

[G15] 枚举
来源：http://swn.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ztj.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jhv.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pji.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jlj.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://yql.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lwa.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://ykb.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xzv.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://waf.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jiw.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://gxy.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://bom.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://xlu.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rza.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://akx.yueranfly.top

Ruby: obj.instance_variables
来源：http://jib.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://aqg.jiagoushi.top

================================================================================
来源：http://sbk.quarkkingdee.top

H. 异常与错误处理
来源：http://gpp.zhongyouzk.top

================================================================================
来源：http://hrf.vqdsnc.cn

[H01] try / catch 基础
来源：http://ypq.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xcb.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lsl.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xis.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fla.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://klc.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pvs.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xbe.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yex.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://jcc.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://xgf.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ckx.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vjz.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fhm.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hsc.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lbv.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sgz.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydn.sufxvd.cn

[H03] 主动抛出异常
来源：http://mxf.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://ksw.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dax.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://ryb.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://wud.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zbn.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pbj.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://pmq.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://bxk.9152youxi.cn

[H04] 自定义异常类型
来源：http://bbv.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://cbo.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://arz.52xcode.cn

JS:   class MyError extends Error {}
来源：http://yth.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://psc.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://ush.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hgr.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://ovr.sxryk.cn

C#:   class MyException : Exception {}
来源：http://frk.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://mkq.hammf.cn

Py:   except ValueError as e:
来源：http://rgu.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsn.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://cbk.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://lhb.ehwqpu.com

Java: catch (IOException | SQLException e) {}
来源：http://jgl.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eox.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://mgi.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gbp.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://zyj.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://sjw.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uuo.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://vwx.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://mhb.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jme.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qln.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://gfi.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://kpz.hcnkem.com

[H07] 断言
来源：http://ssg.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://sej.daxiang520.top

PHP:  assert($x > 0);
来源：http://eyj.nwbrower.top

JS:   console.assert(x > 0);
来源：http://zym.mhx1999.top

TS:   console.assert(x > 0);
来源：http://szm.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ocx.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ydb.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://btz.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://kbf.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://jkh.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://lbk.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kit.ydzc1.top

JS:   e.message;  e.stack
来源：http://ypq.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://agr.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://jiz.vehdjk.com

Go:   err.Error()
来源：http://les.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://kdc.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://zel.bjfxy.top

[H09] 带错误码的异常
来源：http://inc.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cry.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rfl.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hjc.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tmk.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pha.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iic.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://nzp.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zgl.fengsongda.top

[H10] 资源自动释放
来源：http://cxd.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ezz.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jio.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mky.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fkf.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hwb.jlsjyb.cn

Go:   defer f.Close()
来源：http://ipg.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://feu.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yii.hywenlv.cn

================================================================================
来源：http://eiq.jinqigufen.top

I. 正则表达式
来源：http://dli.jyoumei.cn

================================================================================
来源：http://wfo.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://wlg.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mka.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rot.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://xcn.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://ttp.shuidangran.top


<!-- 参考信息 -->