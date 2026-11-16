代发 wailian999

C#:   File.Exists("a.txt")
来源：http://heo.sjlbkw.cn

[F06] 删除文件
来源：http://dzz.sysykeji.top

Py:   os.remove("a.txt")
来源：http://bgw.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://bzy.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://guq.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://qou.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ohc.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://zks.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://fqz.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://zwa.ydzc1.top

[F07] 创建目录（含多级）
来源：http://nmw.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ift.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dta.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztc.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upa.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jup.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cob.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fce.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlh.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://hny.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lsv.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://apy.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://wdw.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://cui.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lhr.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ddx.yuxming.cn

Ruby: Dir.children("dir")
来源：http://uoi.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://xxn.xziqi.cn

[F09] 获取文件大小
来源：http://doc.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://uus.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://dfe.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://tma.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://msa.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://bml.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://krd.gzhubu.top

Ruby: File.size("a.txt")
来源：http://zwr.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://cpp.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://qzj.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rpi.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjn.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bwk.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://igs.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gan.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ezo.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wzd.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cbs.chenlongwang.top

[F11] 复制与移动文件
来源：http://kii.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wni.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gby.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzo.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppj.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qwz.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lun.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ybt.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qlo.cheryme.top

[F12] CSV 读写
来源：http://ohf.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sjb.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sbl.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wdk.andypj.xyz

TS:   // 同上
来源：http://xjo.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qqi.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hwf.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vny.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rxr.daria6918.cn

================================================================================
来源：http://gkb.yj20258.top

G. 面向对象
来源：http://krc.zycfv.cn

================================================================================
来源：http://koq.jiagoushi.top

[G01] 定义类
来源：http://kcr.ivvv.top

Py:   class User: pass
来源：http://ynd.xziqi.cn

PHP:  class User {}
来源：http://kum.shangyingyoupin.top

JS:   class User {}
来源：http://mhy.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://hnx.hammf.cn

Java: class User {}
来源：http://lpe.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://lbu.hnqzz.top

Ruby: class User; end
来源：http://kbb.svipenyu.cn

C#:   class User {}
来源：http://owu.hammf.cn

[G02] 构造函数
来源：http://cmc.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://gga.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://nzd.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://ugl.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://mpt.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://vqq.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://omu.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://ueh.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://jpm.feifeiyinyue.top

[G03] 实例属性
来源：http://lcl.meibo888.top

Py:   self.name = "x"
来源：http://oxq.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://jkv.zhixingplan.top

JS:   this.name = "x";
来源：http://ste.yj20258.top

TS:   name: string = "x";
来源：http://ogm.redwolf501.top

Java: private String name;
来源：http://kvh.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rxd.cqqwz.cn

Ruby: @name = "x"
来源：http://edq.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://pib.fktsv.cn

[G04] 定义方法
来源：http://vli.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://kxh.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mpu.mhx1999.top

JS:   greet() { return this.name; }
来源：http://nho.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://cxf.aibaodan.cn

Java: String greet() { return name; }
来源：http://yyc.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://shn.hammf.cn

Ruby: def greet; @name; end
来源：http://mbb.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://rtw.xingfuxueyuan.xyz

[G05] 继承
来源：http://dku.sufxvd.cn

Py:   class Admin(User): pass
来源：http://qmk.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://pti.iojbl.cn

JS:   class Admin extends User {}
来源：http://ovq.hammf.cn

TS:   class Admin extends User {}
来源：http://ory.cucudq.cn

Java: class Admin extends User {}
来源：http://tzh.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yox.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://rtq.hysaishi.cn

C#:   class Admin : User {}
来源：http://tbi.cucudq.cn

[G06] 重写方法
来源：http://ghm.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://fgn.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lun.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://qot.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://who.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://okm.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zlz.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://tem.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://bks.sjlbkw.cn

[G07] 调用父类方法
来源：http://drf.sxryk.cn

Py:   super().greet()
来源：http://kpc.kuanghao11.cn

PHP:  parent::greet();
来源：http://rev.gogol.net.cn

JS:   super.greet();
来源：http://qbw.cucudq.cn

TS:   super.greet();
来源：http://lea.xuanzx.com

Java: super.greet();
来源：http://snn.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ids.tanke756.top

Ruby: super
来源：http://umw.aibaodan.cn

C#:   base.Greet();
来源：http://trv.ydzc1.top

[G08] 静态方法与属性
来源：http://xoy.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvz.guannengcc.top

PHP:  public static function f() {}
来源：http://vfy.yj202588.top

JS:   static f() {}
来源：http://txh.meibo888.top

TS:   static f(): void {}
来源：http://ozz.snrcjt.cn

Java: static void f() {}
来源：http://jac.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ckz.9152youxi.cn

Ruby: def self.f; end
来源：http://gti.chenzaomai.com

C#:   public static void F() {}
来源：http://gkd.yueranfly.top

[G09] 接口 / 抽象类
来源：http://iww.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://gae.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://vpd.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bei.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://rbe.daxiang520.top

Java: interface Shape { double area(); }
来源：http://ykj.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://dwr.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://evt.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://wmb.jqgfzy.top

[G10] 访问控制
来源：http://jpx.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ely.gzhubu.top

PHP:  public / protected / private
来源：http://apb.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://cgl.jlsjyb.cn

TS:   public / protected / private
来源：http://xix.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://asj.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kaq.yonumen.top

Ruby: public / protected / private
来源：http://tbh.hywenlv.cn

C#:   public / protected / private / internal
来源：http://jdv.fktsv.cn

[G11] getter / setter
来源：http://pig.shuidangran.top

Py:   @property 与 @x.setter
来源：http://neq.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gos.cheryme.top

JS:   get name() { return this._name; }
来源：http://lur.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://fjv.xylfe.cn

Java: public String getName() { return name; }
来源：http://nkk.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzz.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://fhh.birdmap.top

C#:   public string Name { get; set; }
来源：http://uau.tianlin.xyz

[G12] 对象转字符串
来源：http://fuo.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://wbd.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgk.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://dwm.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://teb.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://equ.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eul.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://jia.cheryme.top

C#:   public override string ToString() => Name;
来源：http://sfj.tianlin.xyz

[G13] 判断对象类型
来源：http://efv.bjfxy.top

Py:   isinstance(u, User)
来源：http://ejb.ehwqpu.com

PHP:  $u instanceof User
来源：http://ppc.aizwys.cn

JS:   u instanceof User
来源：http://wmh.gotoacloud.top

TS:   u instanceof User
来源：http://rjm.nwbrower.top

Java: u instanceof User
来源：http://sxe.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pit.316326.xyz

Ruby: u.is_a?(User)
来源：http://slz.zhoulong.xyz

C#:   u is User
来源：http://waz.xylfe.cn

[G14] 数据类 / record
来源：http://sxl.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iad.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://ndi.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hpg.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://gwo.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://zav.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://fng.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lhr.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://mre.xylfe.cn

[G15] 枚举
来源：http://hpe.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://haw.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jeh.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gvm.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rfp.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://tbh.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gvx.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://cqq.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://les.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://dnq.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ceq.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://evi.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://ent.guowangkeji.top

TS:   Object.entries(obj)
来源：http://hak.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jab.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gqo.yangfankeji.com

Ruby: obj.instance_variables
来源：http://yza.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://ngr.yueranfly.top

================================================================================
来源：http://jcu.chenlongwang.top

H. 异常与错误处理
来源：http://gyx.yfazqb.com

================================================================================
来源：http://evd.havefunace.top

[H01] try / catch 基础
来源：http://bor.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oix.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsl.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tcf.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://geu.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mdf.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://elo.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qts.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fsh.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://srs.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ejd.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://nbi.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hqg.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vwx.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://ebz.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://gkp.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dxl.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lhc.cdnleiting.top

[H03] 主动抛出异常
来源：http://ffp.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://rxz.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mio.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://zka.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://whn.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rzq.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://acp.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://put.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nkd.jqgufenzy.top

[H04] 自定义异常类型
来源：http://lmh.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://ttz.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://vif.bjfxy.top

JS:   class MyError extends Error {}
来源：http://tvk.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://ghx.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://zui.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wnn.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://hwa.316326.xyz

C#:   class MyException : Exception {}
来源：http://rvt.yuxming.cn

[H05] 捕获特定类型
来源：http://kfn.snrcjt.cn

Py:   except ValueError as e:
来源：http://xxw.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://giz.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://cxl.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://zfi.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://xnp.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ncy.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://ejg.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tqg.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://qht.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://njg.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oak.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tdz.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pzh.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgq.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xut.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://rgo.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://fpq.hnqzz.top

[H07] 断言
来源：http://irr.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://kbf.zhixingplan.top

PHP:  assert($x > 0);
来源：http://ljs.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://wpc.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://mwr.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://wmi.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mqg.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pis.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://jkx.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://xdb.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://cjo.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xvi.yuxming.cn

JS:   e.message;  e.stack
来源：http://jym.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sha.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uaj.daxiang520.top

Go:   err.Error()
来源：http://ptz.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://vcs.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://dgx.zhixingplan.top

[H09] 带错误码的异常
来源：http://unq.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cwp.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dgy.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qsr.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dyo.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sms.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zbz.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ceq.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lrr.yuxming.cn

[H10] 资源自动释放
来源：http://yee.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zaz.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ano.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bxd.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ndv.uphjek.com


<!-- 参考信息 -->