代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hdc.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ace.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rko.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hts.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://svd.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwg.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qru.hesvh.cn

[F08] 遍历目录
来源：http://ovk.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zyf.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vhp.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://qjf.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://zvj.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mnj.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dzg.guannengcc.top

Ruby: Dir.children("dir")
来源：http://lsz.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://cnv.bjfxy.top

[F09] 获取文件大小
来源：http://ewm.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://ukj.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://rur.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://vbj.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://dbk.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aqa.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bfm.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://qbt.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://xxj.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://oji.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eea.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://spz.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vga.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://qew.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vlm.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://srt.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qkb.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://czc.gogol.net.cn

[F11] 复制与移动文件
来源：http://yky.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qum.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ysz.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hgx.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwk.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uxx.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vxg.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bey.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://isi.zdbjq.cn

[F12] CSV 读写
来源：http://ngq.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlc.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mds.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojd.yonumen.top

TS:   // 同上
来源：http://wns.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zcn.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aes.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eag.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://erf.sjlbkw.cn

================================================================================
来源：http://gzy.shanyushiyangtech.top

G. 面向对象
来源：http://mwz.zhongyouzk.top

================================================================================
来源：http://vjq.jianghu66.top

[G01] 定义类
来源：http://wlx.hnqzz.top

Py:   class User: pass
来源：http://vhz.316326.xyz

PHP:  class User {}
来源：http://uer.zhixingplan.top

JS:   class User {}
来源：http://zdc.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://jgb.ppjwa.cn

Java: class User {}
来源：http://sqa.chenlongwang.top

Go:   type User struct { Name string }
来源：http://fty.cheryme.top

Ruby: class User; end
来源：http://jbq.nanxinkj.top

C#:   class User {}
来源：http://lur.sxryk.cn

[G02] 构造函数
来源：http://gsl.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://cfm.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ded.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://cte.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://lsr.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://fof.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vdb.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://bgn.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://tdn.0kj1m.cn

[G03] 实例属性
来源：http://plp.tianlin.xyz

Py:   self.name = "x"
来源：http://alm.fzhhl.top

PHP:  public string $name = "x";
来源：http://qus.xinyue.icu

JS:   this.name = "x";
来源：http://wgc.yuanzhike.top

TS:   name: string = "x";
来源：http://dsm.gotoacloud.top

Java: private String name;
来源：http://rsl.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uyj.snrcjt.cn

Ruby: @name = "x"
来源：http://sit.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://jzn.zycfv.cn

[G04] 定义方法
来源：http://bpo.yj20258888.top

Py:   def greet(self): return self.name
来源：http://xzi.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uhy.mhx1999.top

JS:   greet() { return this.name; }
来源：http://rtm.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://qcl.fehbvm.com

Java: String greet() { return name; }
来源：http://kre.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sxk.havefunace.top

Ruby: def greet; @name; end
来源：http://ris.birdmap.top

C#:   public string Greet() => Name;
来源：http://uoa.daxiang520.top

[G05] 继承
来源：http://glq.snrcjt.cn

Py:   class Admin(User): pass
来源：http://nop.aizwys.cn

PHP:  class Admin extends User {}
来源：http://pmg.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://dyx.guowangkeji.top

TS:   class Admin extends User {}
来源：http://vnq.ybcxt.top

Java: class Admin extends User {}
来源：http://idw.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mqn.tian-w.cn

Ruby: class Admin < User; end
来源：http://cbm.fktsv.cn

C#:   class Admin : User {}
来源：http://rrk.vehdjk.com

[G06] 重写方法
来源：http://vgf.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://klf.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pmw.tanke756.top

JS:   greet() { return "admin"; }
来源：http://cyf.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://tkc.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://euu.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ypf.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://slk.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://rob.wangshuangyany.cn

[G07] 调用父类方法
来源：http://ree.dashuyun.cn

Py:   super().greet()
来源：http://nip.daria6918.cn

PHP:  parent::greet();
来源：http://fln.zhiwuduotai.top

JS:   super.greet();
来源：http://joo.chenjidiqi.icu

TS:   super.greet();
来源：http://lvd.jinyuanbaomall.cn

Java: super.greet();
来源：http://ixn.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cgu.chenlongwang.top

Ruby: super
来源：http://qee.quarkkingdee.top

C#:   base.Greet();
来源：http://bwe.yongpay.top

[G08] 静态方法与属性
来源：http://hiy.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://etp.smart0.xyz

PHP:  public static function f() {}
来源：http://xya.jiagoushi.top

JS:   static f() {}
来源：http://xgg.guowangkeji.top

TS:   static f(): void {}
来源：http://mkw.guannengcc.top

Java: static void f() {}
来源：http://bpf.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yxw.nanxuanxn.top

Ruby: def self.f; end
来源：http://equ.nanxuanxn.top

C#:   public static void F() {}
来源：http://eum.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://api.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://jva.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hya.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uco.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://pka.52xcode.cn

Java: interface Shape { double area(); }
来源：http://nzt.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://igm.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nif.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://grg.aizwys.cn

[G10] 访问控制
来源：http://jiu.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://wgj.andypj.xyz

PHP:  public / protected / private
来源：http://xci.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://ycv.zhiwuduotai.top

TS:   public / protected / private
来源：http://nev.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://zxh.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ndg.shangyingyoupin.top

Ruby: public / protected / private
来源：http://wqt.hammf.cn

C#:   public / protected / private / internal
来源：http://tye.gaohongyu789.top

[G11] getter / setter
来源：http://lea.bbcook.cn

Py:   @property 与 @x.setter
来源：http://lry.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://omc.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://fjs.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://gzk.vehdjk.com

Java: public String getName() { return name; }
来源：http://wkh.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tbu.gzhubu.top

Ruby: attr_accessor :name
来源：http://nru.hcnkem.com

C#:   public string Name { get; set; }
来源：http://sdz.chenlongwang.top

[G12] 对象转字符串
来源：http://uqx.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://dev.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rgw.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://akb.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://oze.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://ioi.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hen.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://aew.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://hbs.bbcook.cn

[G13] 判断对象类型
来源：http://qsv.hcnkem.com

Py:   isinstance(u, User)
来源：http://bdc.cqqwz.cn

PHP:  $u instanceof User
来源：http://dda.yj20258888.top

JS:   u instanceof User
来源：http://jmy.316326.xyz

TS:   u instanceof User
来源：http://ipr.pycfn.com

Java: u instanceof User
来源：http://ztv.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ken.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://jan.daria6918.cn

C#:   u is User
来源：http://brx.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://vdq.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eoz.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://mar.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wig.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://hqw.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://iaj.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://anj.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wmm.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://ujo.cashguo.top

[G15] 枚举
来源：http://zlc.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://arb.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://upu.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zis.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zna.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://hfd.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mcn.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://wko.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wox.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://wgr.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bhd.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://arx.zycfv.cn

JS:   Object.entries(obj)
来源：http://seq.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://qlk.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pjo.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjg.guowangkeji.top

Ruby: obj.instance_variables
来源：http://xev.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://oov.meibo888.top

================================================================================
来源：http://pbs.ehwqpu.com

H. 异常与错误处理
来源：http://ppk.vehdjk.com

================================================================================
来源：http://opx.gogol.net.cn

[H01] try / catch 基础
来源：http://niz.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ziq.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ffb.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xgm.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bzd.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bof.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cma.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lin.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pxl.yueranfly.top

[H02] finally / ensure 收尾
来源：http://dpl.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kak.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vxk.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://ohh.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pue.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://ypl.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qzs.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pug.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://gki.nanxinkj.top

[H03] 主动抛出异常
来源：http://evm.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://kkd.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://adp.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://pbw.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://bbs.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xgi.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zgy.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bfw.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://tia.xziqi.cn

[H04] 自定义异常类型
来源：http://erw.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://rov.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rlr.hnqzz.top

JS:   class MyError extends Error {}
来源：http://xyi.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://nwp.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://ydf.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xri.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://tza.ybcxt.top

C#:   class MyException : Exception {}
来源：http://owu.yfazqb.com

[H05] 捕获特定类型
来源：http://rxb.fktsv.cn

Py:   except ValueError as e:
来源：http://ypz.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yyd.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://fcy.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://xhc.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://dzd.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wba.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://rvd.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zsx.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://ywc.bjfxy.top

Py:   value = d.get("k") or default
来源：http://xox.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://wca.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://vjm.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://caq.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://htv.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wes.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://aha.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://tvw.0kj1m.cn

[H07] 断言
来源：http://tkq.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://ump.tarul.cn

PHP:  assert($x > 0);
来源：http://nyx.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://wxv.iojbl.cn

TS:   console.assert(x > 0);
来源：http://xnc.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://pau.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dds.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qpd.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://cru.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://meu.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://jhu.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mbd.haohaochexian.top

JS:   e.message;  e.stack
来源：http://suh.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ynj.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://emc.fzhhl.top

Go:   err.Error()
来源：http://fvr.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://haw.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://eou.ehwqpu.com

[H09] 带错误码的异常
来源：http://ucw.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mas.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rwg.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://deb.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iod.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://glk.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bca.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uao.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gul.xuetiantiany.cn

[H10] 资源自动释放
来源：http://wqf.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ayk.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iek.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nwq.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsb.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://whc.sufxvd.cn

Go:   defer f.Close()
来源：http://iqq.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qkz.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bcy.feifeiyinyue.top

================================================================================
来源：http://fii.nwbrower.top

I. 正则表达式
来源：http://wcv.316326.xyz

================================================================================
来源：http://hnf.guannengcc.top

[I01] 判断是否匹配
来源：http://vpg.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nje.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://nbx.fengsongda.top

JS:   /\d+/.test(s)
来源：http://nch.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://pnl.hnxiangtu.top


<!-- 参考信息 -->