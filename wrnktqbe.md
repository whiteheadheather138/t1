代发 wailian999

Ruby: File.delete("a.txt")
来源：http://sxr.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://xfz.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://hgf.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://npg.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xrq.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nxr.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eep.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tft.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jtw.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwg.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dcb.jlsjyb.cn

[F08] 遍历目录
来源：http://bps.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iuy.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hkn.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://rvr.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://bbv.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fwj.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qsx.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://whd.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://bmp.yonumen.top

[F09] 获取文件大小
来源：http://deo.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://jvc.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://sue.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://cut.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://hhj.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cdy.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aku.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://pfi.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://fcf.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://fal.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hnl.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xwi.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bur.52xcode.cn

TS:   path.extname("a.txt")
来源：http://epi.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dth.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qlo.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rix.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://our.shzxlz.cn

[F11] 复制与移动文件
来源：http://yhl.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tsn.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqu.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aiy.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fqx.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pay.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fvq.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ndt.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hgh.yj20258888.top

[F12] CSV 读写
来源：http://ias.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mck.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dqn.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sfo.fktsv.cn

TS:   // 同上
来源：http://kbh.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jrq.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xtz.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bar.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zew.yonumen.top

================================================================================
来源：http://dnt.zhengqikj.top

G. 面向对象
来源：http://cze.zycfv.cn

================================================================================
来源：http://wuh.xuetiantiany.cn

[G01] 定义类
来源：http://ipf.tanke756.top

Py:   class User: pass
来源：http://jve.ivvv.top

PHP:  class User {}
来源：http://ufj.yuxming.cn

JS:   class User {}
来源：http://qys.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://ugx.hammf.cn

Java: class User {}
来源：http://xqh.xylfe.cn

Go:   type User struct { Name string }
来源：http://pwx.0kj1m.cn

Ruby: class User; end
来源：http://ear.tianlin.xyz

C#:   class User {}
来源：http://ale.shanyushiyangtech.top

[G02] 构造函数
来源：http://qkq.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://tde.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://uci.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://kul.ivvv.top

TS:   constructor(public name: string) {}
来源：http://afc.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://iqe.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vma.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://erj.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://mmp.hysaishi.cn

[G03] 实例属性
来源：http://mjh.chenjidiqi.icu

Py:   self.name = "x"
来源：http://noh.bbcook.cn

PHP:  public string $name = "x";
来源：http://hkp.zycfv.cn

JS:   this.name = "x";
来源：http://gmr.tian-w.cn

TS:   name: string = "x";
来源：http://gyt.guowangkeji.top

Java: private String name;
来源：http://cdp.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ica.jqgfzy.top

Ruby: @name = "x"
来源：http://whq.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://pmj.cashguo.top

[G04] 定义方法
来源：http://dsz.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://fgg.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uyo.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://fjo.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://cul.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://wms.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hra.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://nic.daxiang520.top

C#:   public string Greet() => Name;
来源：http://vhg.yanxiufei.cn

[G05] 继承
来源：http://opb.pycfn.com

Py:   class Admin(User): pass
来源：http://rii.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://rlk.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://eze.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://zxf.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://eeu.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uzq.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://ujf.52xcode.cn

C#:   class Admin : User {}
来源：http://zgb.hywenlv.cn

[G06] 重写方法
来源：http://hwj.meibo888.top

Py:   def greet(self): return "admin"
来源：http://wjh.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://qnn.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://bxg.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://zor.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://skj.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rev.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://iib.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://auw.jlsjyb.cn

[G07] 调用父类方法
来源：http://wty.sweek.top

Py:   super().greet()
来源：http://ibl.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://lmr.hesvh.cn

JS:   super.greet();
来源：http://chc.wangdashe.top

TS:   super.greet();
来源：http://pfa.bjfxy.top

Java: super.greet();
来源：http://afr.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dxi.hammf.cn

Ruby: super
来源：http://muh.bjfxy.top

C#:   base.Greet();
来源：http://rfm.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://iku.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jqn.0kj1m.cn

PHP:  public static function f() {}
来源：http://qgw.yangfankeji.com

JS:   static f() {}
来源：http://ywc.cucudq.cn

TS:   static f(): void {}
来源：http://uwu.hnqzz.top

Java: static void f() {}
来源：http://yip.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dww.redwolf501.top

Ruby: def self.f; end
来源：http://ekq.hesvh.cn

C#:   public static void F() {}
来源：http://fkl.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://foj.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://fiw.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wfn.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kah.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://ihd.shuidangran.top

Java: interface Shape { double area(); }
来源：http://knc.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://sjk.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://auy.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://eku.iojbl.cn

[G10] 访问控制
来源：http://lkw.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://ors.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://zhe.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://blg.sxryk.cn

TS:   public / protected / private
来源：http://zcw.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://tfo.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvi.haohaochexian.top

Ruby: public / protected / private
来源：http://txe.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://iia.zhixingplan.top

[G11] getter / setter
来源：http://glw.birdmap.top

Py:   @property 与 @x.setter
来源：http://rgg.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zus.gzhubu.top

JS:   get name() { return this._name; }
来源：http://jfy.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://qsv.gzhubu.top

Java: public String getName() { return name; }
来源：http://vlv.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftt.ctjpmb.com

Ruby: attr_accessor :name
来源：http://elj.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://rjf.jinqigfzy.top

[G12] 对象转字符串
来源：http://vkk.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://efn.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ppu.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://ozd.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://mlo.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://yny.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://nom.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://oaf.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://aty.mhx1999.top

[G13] 判断对象类型
来源：http://rsn.nanxinkj.top

Py:   isinstance(u, User)
来源：http://ibt.daxiang520.top

PHP:  $u instanceof User
来源：http://wng.yvedp.cn

JS:   u instanceof User
来源：http://epq.hammf.cn

TS:   u instanceof User
来源：http://bpg.shzxlz.cn

Java: u instanceof User
来源：http://fpd.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://snc.yfazqb.com

Ruby: u.is_a?(User)
来源：http://xcj.shanyushiyangtech.top

C#:   u is User
来源：http://wbp.vehdjk.com

[G14] 数据类 / record
来源：http://xbb.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rck.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://xdj.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://nxs.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://ocu.shuidangran.top

Java: record User(String name, int age) {}
来源：http://hli.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://yjn.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://plc.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://ydd.cashguo.top

[G15] 枚举
来源：http://oki.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nid.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://noj.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zsq.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qrr.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://uhp.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rjn.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://nbi.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://syx.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://qjv.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kuo.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://pay.yj20258.top

JS:   Object.entries(obj)
来源：http://bxg.xinyue.icu

TS:   Object.entries(obj)
来源：http://zqk.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pnu.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://caq.wangdashe.top

Ruby: obj.instance_variables
来源：http://ykb.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://zhn.hywenlv.cn

================================================================================
来源：http://apz.guowangkeji.top

H. 异常与错误处理
来源：http://pcl.yonumen.top

================================================================================
来源：http://zlb.316326.xyz

[H01] try / catch 基础
来源：http://eul.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eci.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://upx.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://muy.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nbm.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vja.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nhn.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wly.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhd.yueranfly.top

[H02] finally / ensure 收尾
来源：http://rgl.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://qic.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://smr.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nra.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nmr.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://daz.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lwd.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pmf.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghn.cashguo.top

[H03] 主动抛出异常
来源：http://xdc.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://niv.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yzf.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://jtv.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://vea.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xox.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jdz.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://smb.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ans.yanxiufei.cn

[H04] 自定义异常类型
来源：http://yga.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://pgo.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://kzm.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://tfi.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://fej.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://rjw.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybq.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://fot.xinyue.icu

C#:   class MyException : Exception {}
来源：http://jdl.cqqwz.cn

[H05] 捕获特定类型
来源：http://wge.hammf.cn

Py:   except ValueError as e:
来源：http://nzh.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kso.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://ffm.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://qba.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://gjo.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xri.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://bkh.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eek.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://beo.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://zcw.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://ock.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qzf.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://ddo.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ecb.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uax.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://tpo.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://czv.cqqwz.cn

[H07] 断言
来源：http://cfz.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://omp.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://yui.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://waf.tarul.cn

TS:   console.assert(x > 0);
来源：http://vkp.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://vmk.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jdr.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://qgo.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://auk.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://lht.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://aqt.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vlt.guannengcc.top

JS:   e.message;  e.stack
来源：http://cbg.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jix.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://bie.quarkkingdee.top

Go:   err.Error()
来源：http://vxy.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://lnp.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://wbz.guannengcc.top

[H09] 带错误码的异常
来源：http://dab.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vtl.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tqm.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tcw.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ujh.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://joi.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vmw.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://rjx.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://awn.zhongyouzk.top

[H10] 资源自动释放
来源：http://fbi.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://sqh.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vhp.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vez.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ovh.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qpf.jyoumei.cn

Go:   defer f.Close()
来源：http://qhj.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qva.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qiz.quarkkingdee.top

================================================================================
来源：http://qqz.sysykeji.top

I. 正则表达式
来源：http://jrq.xingfuxueyuan.xyz

================================================================================
来源：http://glo.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://lci.zhiwuduotai.top


<!-- 参考信息 -->