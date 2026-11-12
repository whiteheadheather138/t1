代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://vxb.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://nec.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ohk.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://rtx.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://fzy.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://fps.cheryme.top

[F07] 创建目录（含多级）
来源：http://sin.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ddb.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vgd.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfq.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jzz.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vle.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pnf.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://egi.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lsx.hesvh.cn

[F08] 遍历目录
来源：http://diw.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nwh.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jby.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://rqu.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://apb.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xlx.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pvc.ydzc1.top

Ruby: Dir.children("dir")
来源：http://zsj.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://utc.bjfxy.top

[F09] 获取文件大小
来源：http://rxp.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://vvt.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://kdk.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://hwc.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://ujm.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://cgp.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mfh.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://bay.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://qrj.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://yly.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pdi.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ijm.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nxh.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://rzx.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fjk.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ijr.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ice.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tjv.sufxvd.cn

[F11] 复制与移动文件
来源：http://dez.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oil.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dlw.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yom.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dnl.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hnj.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://act.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fmo.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xyu.cqqwz.cn

[F12] CSV 读写
来源：http://ifv.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jlg.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bav.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bcl.meibo888.top

TS:   // 同上
来源：http://vme.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://itz.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vif.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://elt.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://nfv.jinyuanbaomall.cn

================================================================================
来源：http://ppq.zhongyouzk.top

G. 面向对象
来源：http://trk.xingfuxueyuan.xyz

================================================================================
来源：http://cxg.yangfankeji.com

[G01] 定义类
来源：http://cnz.andypj.xyz

Py:   class User: pass
来源：http://lsj.snrcjt.cn

PHP:  class User {}
来源：http://hld.ywan-chungtsiang.top

JS:   class User {}
来源：http://uni.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://hdj.fengsongda.top

Java: class User {}
来源：http://zea.9152youxi.cn

Go:   type User struct { Name string }
来源：http://hvy.jianghu66.top

Ruby: class User; end
来源：http://hbw.ctjpmb.com

C#:   class User {}
来源：http://thc.jianghu66.top

[G02] 构造函数
来源：http://aeb.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://fgc.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://wti.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://fsm.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://txm.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://bhh.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hyd.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://hzr.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://poo.fktsv.cn

[G03] 实例属性
来源：http://fxu.shangyingyoupin.top

Py:   self.name = "x"
来源：http://uvc.gogol.net.cn

PHP:  public string $name = "x";
来源：http://dha.yj202588.top

JS:   this.name = "x";
来源：http://hfz.cucudq.cn

TS:   name: string = "x";
来源：http://lpf.zhoulong.xyz

Java: private String name;
来源：http://byy.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nvd.yj20258888.top

Ruby: @name = "x"
来源：http://sog.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://kfm.ehwqpu.com

[G04] 定义方法
来源：http://xzf.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://xec.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fnw.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://ayu.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://zel.guannengcc.top

Java: String greet() { return name; }
来源：http://ywl.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vkc.tarul.cn

Ruby: def greet; @name; end
来源：http://rke.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://kuk.tarul.cn

[G05] 继承
来源：http://nsy.jyoumei.cn

Py:   class Admin(User): pass
来源：http://xha.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://lal.ydzc1.top

JS:   class Admin extends User {}
来源：http://mpl.yuxming.cn

TS:   class Admin extends User {}
来源：http://udl.quarkkingdee.top

Java: class Admin extends User {}
来源：http://lbp.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wgb.uphjek.com

Ruby: class Admin < User; end
来源：http://nbz.yueranfly.top

C#:   class Admin : User {}
来源：http://lrc.tarul.cn

[G06] 重写方法
来源：http://typ.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://die.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oxy.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://iih.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://cwt.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://ewq.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ail.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://nvv.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://fhq.daria6918.cn

[G07] 调用父类方法
来源：http://jsi.gaohongyu789.top

Py:   super().greet()
来源：http://dvs.ehwqpu.com

PHP:  parent::greet();
来源：http://uxi.zhiwuduotai.top

JS:   super.greet();
来源：http://ayh.chenlongwang.top

TS:   super.greet();
来源：http://gbo.hywenlv.cn

Java: super.greet();
来源：http://izr.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ajy.9152youxi.cn

Ruby: super
来源：http://hfd.c1oappe.top

C#:   base.Greet();
来源：http://hve.jqgfzy.top

[G08] 静态方法与属性
来源：http://lzw.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sic.yanxiufei.cn

PHP:  public static function f() {}
来源：http://adl.pengpengdd.cyou

JS:   static f() {}
来源：http://gsc.snrcjt.cn

TS:   static f(): void {}
来源：http://axj.dashuyun.cn

Java: static void f() {}
来源：http://isc.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://atq.epnwcf.com

Ruby: def self.f; end
来源：http://olv.epnwcf.com

C#:   public static void F() {}
来源：http://wcj.guannengcc.top

[G09] 接口 / 抽象类
来源：http://lsi.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://als.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://oun.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://usl.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://zmx.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://oyz.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://uqo.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hhj.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://utu.nanxuanxn.top

[G10] 访问控制
来源：http://zuf.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://cft.tian-w.cn

PHP:  public / protected / private
来源：http://ljz.birdmap.top

JS:   #private 字段；其余公开
来源：http://enm.wangdashe.top

TS:   public / protected / private
来源：http://jve.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://tzy.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qaf.daria6918.cn

Ruby: public / protected / private
来源：http://qjj.gogol.net.cn

C#:   public / protected / private / internal
来源：http://xml.ybcxt.top

[G11] getter / setter
来源：http://bwt.tian-w.cn

Py:   @property 与 @x.setter
来源：http://hzf.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://acb.iojbl.cn

JS:   get name() { return this._name; }
来源：http://jsn.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://rfn.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://bwa.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://biu.chenzaomai.com

Ruby: attr_accessor :name
来源：http://mit.sxryk.cn

C#:   public string Name { get; set; }
来源：http://wcp.zhixingplan.top

[G12] 对象转字符串
来源：http://qgm.meibo888.top

Py:   def __str__(self): return self.name
来源：http://clx.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://byr.ybcxt.top

JS:   toString() { return this.name; }
来源：http://ohy.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://yxu.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://avx.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wno.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://jqp.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://qda.sweek.top

[G13] 判断对象类型
来源：http://ntq.ctjpmb.com

Py:   isinstance(u, User)
来源：http://beh.sweek.top

PHP:  $u instanceof User
来源：http://pit.52xcode.cn

JS:   u instanceof User
来源：http://mde.xinyue.icu

TS:   u instanceof User
来源：http://clf.hnxiangtu.top

Java: u instanceof User
来源：http://ipv.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ihj.nwbrower.top

Ruby: u.is_a?(User)
来源：http://fhu.fengsongda.top

C#:   u is User
来源：http://hxw.bjfxy.top

[G14] 数据类 / record
来源：http://uzj.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ied.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://tjb.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://ayl.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://kfn.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://mcc.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://olq.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ljl.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://rwl.tarul.cn

[G15] 枚举
来源：http://lnr.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hwu.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysy.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tdf.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lth.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://tve.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fpv.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://wfz.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qup.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://vrx.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gvp.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://zte.gotoacloud.top

JS:   Object.entries(obj)
来源：http://ads.zdqjudy.top

TS:   Object.entries(obj)
来源：http://yqw.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wzc.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zol.smart0.xyz

Ruby: obj.instance_variables
来源：http://nih.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://ocn.wangshuangyany.cn

================================================================================
来源：http://whs.fktsv.cn

H. 异常与错误处理
来源：http://wpq.hnqzz.top

================================================================================
来源：http://pdz.yuanzhike.top

[H01] try / catch 基础
来源：http://ldw.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wrn.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vio.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ocl.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aqm.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://onv.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://slk.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yho.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ztq.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://gbd.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://ggt.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nlo.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dyy.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://nsy.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://xsz.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bce.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://snj.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ves.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://zoj.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://weg.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ucn.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://ays.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://mng.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wbl.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nfv.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ime.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pqx.daxiang520.top

[H04] 自定义异常类型
来源：http://ifr.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://jye.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://lfp.gzhubu.top

JS:   class MyError extends Error {}
来源：http://auo.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://rmg.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qit.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hgl.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://xsm.daxiang520.top

C#:   class MyException : Exception {}
来源：http://unq.sweek.top

[H05] 捕获特定类型
来源：http://coc.sxryk.cn

Py:   except ValueError as e:
来源：http://fwn.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tja.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://zgy.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://rfw.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://vyu.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gmw.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://nqg.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ciq.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://biw.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://yez.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://biy.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://umy.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://nbd.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://poa.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://itr.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://gyl.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://xdj.jinyuanbaomall.cn

[H07] 断言
来源：http://til.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://ppl.cucudq.cn

PHP:  assert($x > 0);
来源：http://hqi.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://lod.gzhubu.top

TS:   console.assert(x > 0);
来源：http://fjw.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://aip.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zdq.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sdn.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://jqd.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://rdv.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://pjw.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhe.chenlongwang.top

JS:   e.message;  e.stack
来源：http://egj.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgc.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zfx.ppjwa.cn

Go:   err.Error()
来源：http://mdp.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://ejq.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://tmw.andypj.xyz

[H09] 带错误码的异常
来源：http://gdf.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eel.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pii.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xdm.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vkv.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fqf.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://obv.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://klc.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fjn.fehbvm.com

[H10] 资源自动释放
来源：http://fcb.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pfw.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ifa.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tkk.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rnx.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vjp.yuxming.cn

Go:   defer f.Close()
来源：http://jhk.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hxc.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mnq.shanyushiyangkeji.top


<!-- 参考信息 -->