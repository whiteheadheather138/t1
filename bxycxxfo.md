代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://djn.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oxe.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://joz.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://buq.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://zvr.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gcm.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bqy.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://nuj.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://qzu.zycfv.cn

[F06] 删除文件
来源：http://xqt.52xcode.cn

Py:   os.remove("a.txt")
来源：http://eos.tanke756.top

PHP:  unlink("a.txt");
来源：http://jhd.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://mkt.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://apd.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wpn.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://fpq.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://svi.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://xrs.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://eoy.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kcq.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gce.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uso.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hmw.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vug.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jnu.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tbq.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vvr.yuanzhike.top

[F08] 遍历目录
来源：http://uvx.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://scz.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iel.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://hdd.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://nlo.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dhm.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ksy.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://voa.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://hlf.cashguo.top

[F09] 获取文件大小
来源：http://skb.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://umb.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://yuu.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://xxv.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://oyu.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://tws.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bow.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://wjl.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://orq.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://knw.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://acv.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hgx.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ynp.daxiang520.top

TS:   path.extname("a.txt")
来源：http://qsf.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lqj.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgy.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvd.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://clu.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ozt.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pcv.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ccm.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dfw.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://biy.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://duv.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://spm.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xdx.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wet.tarul.cn

[F12] CSV 读写
来源：http://syk.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rto.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fjk.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://szg.shanyushiyangtech.top

TS:   // 同上
来源：http://ull.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mzg.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://srr.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xxp.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vzj.xylfe.cn

================================================================================
来源：http://trk.zycfv.cn

G. 面向对象
来源：http://iyt.shanyushiyangkeji.top

================================================================================
来源：http://kmd.hongshengwenyu.top

[G01] 定义类
来源：http://pre.yj20258.top

Py:   class User: pass
来源：http://xtd.dianchejie.cn

PHP:  class User {}
来源：http://bjw.sufxvd.cn

JS:   class User {}
来源：http://itb.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://yop.vqdsnc.cn

Java: class User {}
来源：http://jlm.bjfxy.top

Go:   type User struct { Name string }
来源：http://rej.jinghuilouyu.cn

Ruby: class User; end
来源：http://duk.gaohongyu789.top

C#:   class User {}
来源：http://frp.hcnkem.com

[G02] 构造函数
来源：http://uwi.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://qub.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://tdc.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://wfp.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://qfl.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://ibx.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lcg.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://vyw.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://ogt.sxryk.cn

[G03] 实例属性
来源：http://snz.hammf.cn

Py:   self.name = "x"
来源：http://tto.hywenlv.cn

PHP:  public string $name = "x";
来源：http://ape.hywenlv.cn

JS:   this.name = "x";
来源：http://pvc.smart0.xyz

TS:   name: string = "x";
来源：http://adf.ivvv.top

Java: private String name;
来源：http://myx.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bzs.sweek.top

Ruby: @name = "x"
来源：http://ipz.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://xkn.ctjpmb.com

[G04] 定义方法
来源：http://kef.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://fqd.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gkw.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://tdw.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://alv.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://yxf.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mfd.cucudq.cn

Ruby: def greet; @name; end
来源：http://caf.mhx1999.top

C#:   public string Greet() => Name;
来源：http://dym.tanke756.top

[G05] 继承
来源：http://wdk.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://bgj.ydzc1.top

PHP:  class Admin extends User {}
来源：http://rnc.cashguo.top

JS:   class Admin extends User {}
来源：http://mcx.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://phs.gaohongyu789.top

Java: class Admin extends User {}
来源：http://ztn.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kdw.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://lsd.ydzc1.top

C#:   class Admin : User {}
来源：http://cig.guannengcc.top

[G06] 重写方法
来源：http://lhj.tanke756.top

Py:   def greet(self): return "admin"
来源：http://pkw.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zmk.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://xaq.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://rbw.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://nzp.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uwu.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://zbl.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://prn.guowangkeji.top

[G07] 调用父类方法
来源：http://iud.sweek.top

Py:   super().greet()
来源：http://xii.shangyingyoupin.top

PHP:  parent::greet();
来源：http://upo.cdnleiting.top

JS:   super.greet();
来源：http://scd.nwbrower.top

TS:   super.greet();
来源：http://qao.aizwys.cn

Java: super.greet();
来源：http://szy.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chy.sufxvd.cn

Ruby: super
来源：http://qfz.hfpthk.cn

C#:   base.Greet();
来源：http://iix.pycfn.com

[G08] 静态方法与属性
来源：http://rox.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://smh.sjlbkw.cn

PHP:  public static function f() {}
来源：http://tda.wangdashe.top

JS:   static f() {}
来源：http://tea.chenzaomai.com

TS:   static f(): void {}
来源：http://jqo.sxryk.cn

Java: static void f() {}
来源：http://hee.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://akd.shanyushiyangkeji.top

Ruby: def self.f; end
来源：http://lsa.fzhhl.top

C#:   public static void F() {}
来源：http://ivs.xylfe.cn

[G09] 接口 / 抽象类
来源：http://mqf.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://hie.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://eul.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uys.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://qud.ybcxt.top

Java: interface Shape { double area(); }
来源：http://hhx.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://hsq.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mtg.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://zpt.gaohongyu789.top

[G10] 访问控制
来源：http://mwa.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://lre.haohaochexian.top

PHP:  public / protected / private
来源：http://lzf.yvedp.cn

JS:   #private 字段；其余公开
来源：http://pnh.sysykeji.top

TS:   public / protected / private
来源：http://obq.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://wxk.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vis.quarkkingdee.top

Ruby: public / protected / private
来源：http://luh.andypj.xyz

C#:   public / protected / private / internal
来源：http://ldz.svipenyu.cn

[G11] getter / setter
来源：http://rsn.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://ijf.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://crd.fehbvm.com

JS:   get name() { return this._name; }
来源：http://lqh.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://hmg.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://wqb.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zsi.ydzc1.top

Ruby: attr_accessor :name
来源：http://dhx.pycfn.com

C#:   public string Name { get; set; }
来源：http://hta.sufxvd.cn

[G12] 对象转字符串
来源：http://sqk.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://sie.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ojt.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://wnk.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://ncr.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://kny.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://kyo.tanke756.top

Ruby: def to_s; @name; end
来源：http://zzz.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://vto.uphjek.com

[G13] 判断对象类型
来源：http://fke.sysykeji.top

Py:   isinstance(u, User)
来源：http://pgo.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://qig.jlsjyb.cn

JS:   u instanceof User
来源：http://oxa.sxryk.cn

TS:   u instanceof User
来源：http://hds.jinghuilouyu.cn

Java: u instanceof User
来源：http://wlc.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ipc.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://yot.yj20258888.top

C#:   u is User
来源：http://oxz.jyoumei.cn

[G14] 数据类 / record
来源：http://scg.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zrx.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://lsi.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qkx.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://yrh.gzhubu.top

Java: record User(String name, int age) {}
来源：http://rvs.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://ayt.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jsr.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://tuw.hnqzz.top

[G15] 枚举
来源：http://nfw.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qok.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bre.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qeh.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://axy.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://mau.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rpk.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://vcq.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oox.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://gqq.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uac.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://flx.bjfxy.top

JS:   Object.entries(obj)
来源：http://drv.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://rki.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gfh.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sln.yj20258.top

Ruby: obj.instance_variables
来源：http://itv.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://tkv.dianchejie.cn

================================================================================
来源：http://vuw.pengpengdd.cyou

H. 异常与错误处理
来源：http://lqd.pengpengdd.cyou

================================================================================
来源：http://vso.shangyingyoupin.top

[H01] try / catch 基础
来源：http://rxc.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rzr.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cwz.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xpt.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tpj.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://smw.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://obh.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xcr.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gre.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://fed.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rtu.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vig.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ymf.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vbc.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cbl.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ejr.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nld.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://usi.aibaodan.cn

[H03] 主动抛出异常
来源：http://hee.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://dll.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lxe.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://xfy.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://yyy.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tdi.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pco.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rxl.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://sdu.bjfxy.top

[H04] 自定义异常类型
来源：http://nrm.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://alp.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ryy.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://iia.smart0.xyz

TS:   class MyError extends Error {}
来源：http://mwc.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://mtj.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nkk.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://tqd.yj202588.top

C#:   class MyException : Exception {}
来源：http://vsu.havefunace.top

[H05] 捕获特定类型
来源：http://njr.bjfxy.top

Py:   except ValueError as e:
来源：http://jtu.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://csv.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://rpm.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ydc.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://ovv.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kbo.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://rhy.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ngf.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://uph.ivvv.top

Py:   value = d.get("k") or default
来源：http://pjo.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://zzi.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://hqv.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://byu.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ccw.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gdq.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://cqj.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://bbh.redwolf501.top

[H07] 断言
来源：http://bzz.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://kla.ydzc1.top

PHP:  assert($x > 0);
来源：http://zug.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://czj.fehbvm.com

TS:   console.assert(x > 0);
来源：http://wfn.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://ymc.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ocz.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://sjg.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://gid.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://yqm.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://bva.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kpb.mhx1999.top

JS:   e.message;  e.stack
来源：http://jha.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://omf.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jmv.yj20258.top

Go:   err.Error()
来源：http://tsy.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://tsr.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://uzi.fzhhl.top

[H09] 带错误码的异常
来源：http://jtj.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://buw.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://khm.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rcu.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cdr.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uxw.tian-w.cn


<!-- 参考信息 -->