代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://kkl.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://gdv.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hwg.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://reo.uphjek.com

Ruby: File.delete("a.txt")
来源：http://bun.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://ibq.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://mno.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hvx.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://esy.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mmm.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ajv.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xfn.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://izv.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jgs.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dji.yonumen.top

[F08] 遍历目录
来源：http://xui.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://eod.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://krq.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://jvr.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://oxz.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ani.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpg.uphjek.com

Ruby: Dir.children("dir")
来源：http://tiw.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://zjb.cashguo.top

[F09] 获取文件大小
来源：http://gdc.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://gpy.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://riu.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://mac.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://ctk.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://sgt.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ntt.iojbl.cn

Ruby: File.size("a.txt")
来源：http://mdk.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://nwm.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://rqm.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bcg.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yzn.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xmy.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://uvp.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jbi.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xyn.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ecs.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khj.tanke756.top

[F11] 复制与移动文件
来源：http://zfy.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vix.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ogf.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dmn.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ztm.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ohw.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mhv.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iyp.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yzc.havefunace.top

[F12] CSV 读写
来源：http://pum.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eia.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rbv.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nah.aizwys.cn

TS:   // 同上
来源：http://axs.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vaw.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zpb.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fts.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pdb.jinyuanbaomall.cn

================================================================================
来源：http://aza.nwbrower.top

G. 面向对象
来源：http://lda.fengsongda.top

================================================================================
来源：http://npw.jqgufenzy.top

[G01] 定义类
来源：http://wix.jyoumei.cn

Py:   class User: pass
来源：http://ttl.smart0.xyz

PHP:  class User {}
来源：http://wdr.guannengcc.top

JS:   class User {}
来源：http://znj.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://gjb.iojbl.cn

Java: class User {}
来源：http://nfh.9152youxi.cn

Go:   type User struct { Name string }
来源：http://rlt.hongshengwenyu.top

Ruby: class User; end
来源：http://cyf.bbcook.cn

C#:   class User {}
来源：http://lcp.hysaishi.cn

[G02] 构造函数
来源：http://xts.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://qwp.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://dsp.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://hdl.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://sdb.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://cac.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ppx.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://wof.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://esv.zhiwuduotai.top

[G03] 实例属性
来源：http://nfj.gotoacloud.top

Py:   self.name = "x"
来源：http://rvh.gogol.net.cn

PHP:  public string $name = "x";
来源：http://xzr.zhengqikj.top

JS:   this.name = "x";
来源：http://rce.zhixingplan.top

TS:   name: string = "x";
来源：http://ewp.aibaodan.cn

Java: private String name;
来源：http://znk.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gnr.hfpthk.cn

Ruby: @name = "x"
来源：http://ibb.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://myk.guowangkeji.top

[G04] 定义方法
来源：http://ywt.xuanzx.com

Py:   def greet(self): return self.name
来源：http://ffh.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uue.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://eeq.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://vfb.guowangkeji.top

Java: String greet() { return name; }
来源：http://mxq.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hrl.bbcook.cn

Ruby: def greet; @name; end
来源：http://jqy.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://cbc.ywan-chungtsiang.top

[G05] 继承
来源：http://nyg.jinqigufen.top

Py:   class Admin(User): pass
来源：http://isf.cucudq.cn

PHP:  class Admin extends User {}
来源：http://yrk.sysykeji.top

JS:   class Admin extends User {}
来源：http://nyx.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://cre.dianchejie.cn

Java: class Admin extends User {}
来源：http://mfl.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://spr.mhx1999.top

Ruby: class Admin < User; end
来源：http://mjq.vehdjk.com

C#:   class Admin : User {}
来源：http://agq.yueranfly.top

[G06] 重写方法
来源：http://hgf.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://kbp.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tza.316326.xyz

JS:   greet() { return "admin"; }
来源：http://sdn.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://gnm.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://xse.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ndx.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://anp.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://yvj.nanxuanxn.top

[G07] 调用父类方法
来源：http://asn.cqqwz.cn

Py:   super().greet()
来源：http://dxv.bbcook.cn

PHP:  parent::greet();
来源：http://kfp.dianchejie.cn

JS:   super.greet();
来源：http://pbt.shanyushiyangtech.top

TS:   super.greet();
来源：http://ykj.dashuyun.cn

Java: super.greet();
来源：http://huk.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fdc.hysaishi.cn

Ruby: super
来源：http://fub.ybcxt.top

C#:   base.Greet();
来源：http://rqg.yongpay.top

[G08] 静态方法与属性
来源：http://onx.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://use.hnxiangtu.top

PHP:  public static function f() {}
来源：http://njt.yangfankeji.com

JS:   static f() {}
来源：http://cub.zhongyouzk.top

TS:   static f(): void {}
来源：http://vwm.ybcxt.top

Java: static void f() {}
来源：http://pnu.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://oyg.sysykeji.top

Ruby: def self.f; end
来源：http://gho.zdqjudy.top

C#:   public static void F() {}
来源：http://eup.xziqi.cn

[G09] 接口 / 抽象类
来源：http://fkv.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://ulz.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://dlb.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ytq.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://xzw.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://yht.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://mcu.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jax.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://jau.c1oappe.top

[G10] 访问控制
来源：http://vql.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://fit.chenzaomai.com

PHP:  public / protected / private
来源：http://yvk.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://iuu.chenzaomai.com

TS:   public / protected / private
来源：http://nqe.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://mcz.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zly.yonumen.top

Ruby: public / protected / private
来源：http://ghw.guowangkeji.top

C#:   public / protected / private / internal
来源：http://xux.kuanghao11.cn

[G11] getter / setter
来源：http://slt.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://awl.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lwc.vehdjk.com

JS:   get name() { return this._name; }
来源：http://shi.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://eiw.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://gba.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rrx.cqqwz.cn

Ruby: attr_accessor :name
来源：http://rvm.daxiang520.top

C#:   public string Name { get; set; }
来源：http://uar.jqgfzy.top

[G12] 对象转字符串
来源：http://lba.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://efi.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfi.daxiang520.top

JS:   toString() { return this.name; }
来源：http://mng.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://rqd.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://oht.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://urs.tanke756.top

Ruby: def to_s; @name; end
来源：http://xyw.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://ezj.ctjpmb.com

[G13] 判断对象类型
来源：http://xkn.hysaishi.cn

Py:   isinstance(u, User)
来源：http://jqy.quarkkingdee.top

PHP:  $u instanceof User
来源：http://wmq.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://uxt.meibo888.top

TS:   u instanceof User
来源：http://xgv.shanyushiyangtech.top

Java: u instanceof User
来源：http://drj.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://egz.mhx1999.top

Ruby: u.is_a?(User)
来源：http://gag.sufxvd.cn

C#:   u is User
来源：http://dgb.tarul.cn

[G14] 数据类 / record
来源：http://ibw.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fqv.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://vvf.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://etm.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://mgl.xylfe.cn

Java: record User(String name, int age) {}
来源：http://wld.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://zth.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yiw.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://dxz.zhiwuduotai.top

[G15] 枚举
来源：http://ago.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ipk.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://icp.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bsb.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzk.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://hlh.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fog.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://fjg.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sig.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://ncx.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hgj.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://exp.ydzc1.top

JS:   Object.entries(obj)
来源：http://jnh.epnwcf.com

TS:   Object.entries(obj)
来源：http://hul.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zsm.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gcq.jianghu66.top

Ruby: obj.instance_variables
来源：http://fwg.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://uts.uphjek.com

================================================================================
来源：http://czu.hnqzz.top

H. 异常与错误处理
来源：http://jvl.sjlbkw.cn

================================================================================
来源：http://qfd.ydjk.org.cn

[H01] try / catch 基础
来源：http://mrc.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://igu.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hwz.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kgx.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mei.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xku.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfo.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ykb.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eik.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://exx.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://lof.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jur.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vlf.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dyr.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://ftx.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zbg.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://wum.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lze.yuxming.cn

[H03] 主动抛出异常
来源：http://tdv.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://ttl.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://swi.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://rym.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://oud.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zhx.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rqr.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nhc.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kst.jinqigfzy.top

[H04] 自定义异常类型
来源：http://jdl.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://akv.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://ovs.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://tla.aizwys.cn

TS:   class MyError extends Error {}
来源：http://vij.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://kyw.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qju.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://gyf.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://wgx.haohaochexian.top

[H05] 捕获特定类型
来源：http://lsq.xinyue.icu

Py:   except ValueError as e:
来源：http://fax.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uhu.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://gxh.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://iuw.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://okf.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qvu.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://mgz.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vom.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://hks.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://wne.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://kxw.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://dtf.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://wnq.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cqn.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gvi.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://xgp.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://erp.zhengqikj.top

[H07] 断言
来源：http://wbk.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://fte.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://wwc.bjfxy.top

JS:   console.assert(x > 0);
来源：http://jie.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://lpr.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://fgx.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://diq.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://huc.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://pdf.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://kfw.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://evy.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kca.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://kcj.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjh.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wsd.nanxinkj.top

Go:   err.Error()
来源：http://pex.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://frf.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://uyv.gogol.net.cn

[H09] 带错误码的异常
来源：http://yjz.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ouj.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dwm.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ili.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ptn.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lrf.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ifr.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://bdk.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kgr.wangdashe.top

[H10] 资源自动释放
来源：http://hya.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkb.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ala.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://msu.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bqr.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bft.kuanghao11.cn

Go:   defer f.Close()
来源：http://rqs.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iqm.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rmh.zycfv.cn


<!-- 参考信息 -->