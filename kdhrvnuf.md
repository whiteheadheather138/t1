代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gae.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iwx.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qou.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jok.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bqo.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rzu.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mcz.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iln.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://skt.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qlv.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://pyx.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://igj.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://oux.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://obx.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zni.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://vrl.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://koy.kuanghao11.cn

[F06] 删除文件
来源：http://rvv.shuidangran.top

Py:   os.remove("a.txt")
来源：http://wpc.pycfn.com

PHP:  unlink("a.txt");
来源：http://rhf.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fur.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wux.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aye.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://yne.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://zqk.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://sdo.316326.xyz

[F07] 创建目录（含多级）
来源：http://moc.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ywh.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ksq.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cki.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fvx.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://frv.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nxm.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qay.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dib.nwbrower.top

[F08] 遍历目录
来源：http://kid.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tej.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://svc.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://sad.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://dut.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mki.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ung.mhx1999.top

Ruby: Dir.children("dir")
来源：http://whs.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://ing.9152youxi.cn

[F09] 获取文件大小
来源：http://jzo.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://fkt.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://aza.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://mnw.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://rlw.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ezh.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cka.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://pho.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://lfq.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://tbu.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://okg.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jry.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://joe.zycfv.cn

TS:   path.extname("a.txt")
来源：http://plu.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fyw.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://snb.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jca.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hnz.9152youxi.cn

[F11] 复制与移动文件
来源：http://ooq.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjw.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twf.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tbh.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvx.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://huu.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pma.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kvo.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://emu.pengpengdd.cyou

[F12] CSV 读写
来源：http://dsr.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zlf.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yqd.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kpb.chenzaomai.com

TS:   // 同上
来源：http://ifz.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hzo.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fmv.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cay.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uzd.uphjek.com

================================================================================
来源：http://agb.jinqigfzy.top

G. 面向对象
来源：http://pjr.cqqwz.cn

================================================================================
来源：http://srd.shzxlz.cn

[G01] 定义类
来源：http://ikb.havefunace.top

Py:   class User: pass
来源：http://zay.jinqigufen.top

PHP:  class User {}
来源：http://lrt.hywenlv.cn

JS:   class User {}
来源：http://bxy.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://xlr.jianghu66.top

Java: class User {}
来源：http://lbc.52xcode.cn

Go:   type User struct { Name string }
来源：http://vfa.sxryk.cn

Ruby: class User; end
来源：http://byj.yueranfly.top

C#:   class User {}
来源：http://nrz.iojbl.cn

[G02] 构造函数
来源：http://mvo.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://mlu.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://qyp.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://dzq.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://ets.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://nbs.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vso.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://tcp.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://jgd.tian-w.cn

[G03] 实例属性
来源：http://wxd.xziqi.cn

Py:   self.name = "x"
来源：http://cqz.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://vgx.hammf.cn

JS:   this.name = "x";
来源：http://fxi.xinyue.icu

TS:   name: string = "x";
来源：http://hns.yonumen.top

Java: private String name;
来源：http://zex.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kmn.xziqi.cn

Ruby: @name = "x"
来源：http://hbw.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://hnz.chenjidiqi.icu

[G04] 定义方法
来源：http://eqx.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://xrt.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://spf.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://tqj.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://nig.dianchejie.cn

Java: String greet() { return name; }
来源：http://yyl.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqf.dianchejie.cn

Ruby: def greet; @name; end
来源：http://ljy.daxiang520.top

C#:   public string Greet() => Name;
来源：http://say.daria6918.cn

[G05] 继承
来源：http://wad.hnqzz.top

Py:   class Admin(User): pass
来源：http://kra.fehbvm.com

PHP:  class Admin extends User {}
来源：http://cad.jyoumei.cn

JS:   class Admin extends User {}
来源：http://wcd.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://viy.yj202588.top

Java: class Admin extends User {}
来源：http://iab.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://api.gzhubu.top

Ruby: class Admin < User; end
来源：http://lka.gaohongyu789.top

C#:   class Admin : User {}
来源：http://ubd.zhoulong.xyz

[G06] 重写方法
来源：http://uch.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://hqn.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eqs.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://hjs.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://ati.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://stw.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dzl.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://yso.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://dvl.cdnleiting.top

[G07] 调用父类方法
来源：http://qcl.bbcook.cn

Py:   super().greet()
来源：http://zgt.uphjek.com

PHP:  parent::greet();
来源：http://lql.wangdashe.top

JS:   super.greet();
来源：http://zuu.andypj.xyz

TS:   super.greet();
来源：http://txi.hywenlv.cn

Java: super.greet();
来源：http://jpw.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lxt.gogol.net.cn

Ruby: super
来源：http://vkv.wangdashe.top

C#:   base.Greet();
来源：http://xnr.nwbrower.top

[G08] 静态方法与属性
来源：http://hzf.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nfs.jqgfzy.top

PHP:  public static function f() {}
来源：http://hpd.yanxiufei.cn

JS:   static f() {}
来源：http://rqb.sjlbkw.cn

TS:   static f(): void {}
来源：http://hep.fengsongda.top

Java: static void f() {}
来源：http://qil.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://inf.daxiang520.top

Ruby: def self.f; end
来源：http://vsz.yangfankeji.com

C#:   public static void F() {}
来源：http://uvb.yuxming.cn

[G09] 接口 / 抽象类
来源：http://oco.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://zuv.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://xzl.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iip.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://jqd.xinyue.icu

Java: interface Shape { double area(); }
来源：http://fzr.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://emn.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://upe.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://csv.hongshengwenyu.top

[G10] 访问控制
来源：http://csx.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://jzf.zycfv.cn

PHP:  public / protected / private
来源：http://pjp.yj20258888.top

JS:   #private 字段；其余公开
来源：http://xib.hnqzz.top

TS:   public / protected / private
来源：http://ozl.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://bit.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://slv.cashguo.top

Ruby: public / protected / private
来源：http://ttk.vehdjk.com

C#:   public / protected / private / internal
来源：http://nud.jinghuilouyu.cn

[G11] getter / setter
来源：http://lqa.daria6918.cn

Py:   @property 与 @x.setter
来源：http://nnt.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cno.tian-w.cn

JS:   get name() { return this._name; }
来源：http://xkm.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://sdn.316326.xyz

Java: public String getName() { return name; }
来源：http://lia.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wmw.gotoacloud.top

Ruby: attr_accessor :name
来源：http://tmp.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://odz.zdbjq.cn

[G12] 对象转字符串
来源：http://kll.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://qzp.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://awm.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://zoj.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://mnf.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://njq.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://rah.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://xql.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://kgg.guowangkeji.top

[G13] 判断对象类型
来源：http://ykn.jqgfzy.top

Py:   isinstance(u, User)
来源：http://hdc.yj20258.top

PHP:  $u instanceof User
来源：http://ttb.zdbjq.cn

JS:   u instanceof User
来源：http://nro.cashguo.top

TS:   u instanceof User
来源：http://ogs.zhengqikj.top

Java: u instanceof User
来源：http://ifl.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gdf.guannengcc.top

Ruby: u.is_a?(User)
来源：http://kil.cashguo.top

C#:   u is User
来源：http://yvr.yongpay.top

[G14] 数据类 / record
来源：http://gcr.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xdg.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://clk.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://kjb.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://kjb.cheryme.top

Java: record User(String name, int age) {}
来源：http://pxd.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://uex.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tpu.hammf.cn

C#:   record User(string Name, int Age);
来源：http://umr.yj20258888.top

[G15] 枚举
来源：http://nlm.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iud.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://tqm.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ssu.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sue.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://ioi.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fwi.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://dst.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bvd.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://djl.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jsx.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://qhe.fengsongda.top

JS:   Object.entries(obj)
来源：http://flm.yj20258888.top

TS:   Object.entries(obj)
来源：http://zcx.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hld.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bij.zdbjq.cn

Ruby: obj.instance_variables
来源：http://meb.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://vrg.zdbjq.cn

================================================================================
来源：http://ynr.xziqi.cn

H. 异常与错误处理
来源：http://jqg.jiagoushi.top

================================================================================
来源：http://hdd.jqgfzy.top

[H01] try / catch 基础
来源：http://vet.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xzz.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qfn.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zxc.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://djt.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fhg.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lis.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gzu.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://udq.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://spi.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uzx.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zxy.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jhi.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dck.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://qmw.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ifn.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ore.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gtb.9152youxi.cn

[H03] 主动抛出异常
来源：http://kls.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://xyk.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kwg.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://gja.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://bjl.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vat.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://scs.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ozn.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tjs.xuanzx.com

[H04] 自定义异常类型
来源：http://fpe.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://iur.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://ymm.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://ptr.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://wqx.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://ivc.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vhy.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://nbs.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://onn.sufxvd.cn

[H05] 捕获特定类型
来源：http://aru.yfazqb.com

Py:   except ValueError as e:
来源：http://svm.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mpb.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://fxb.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://tpa.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://mnm.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eka.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://nja.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iah.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://wzo.hcnkem.com

Py:   value = d.get("k") or default
来源：http://opg.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://nbs.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://rrm.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://mvu.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osh.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ccm.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://fch.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://rie.bjfxy.top

[H07] 断言
来源：http://amm.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://yvn.ydzc1.top

PHP:  assert($x > 0);
来源：http://xgb.yj202588.top

JS:   console.assert(x > 0);
来源：http://wve.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://ckk.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://zvz.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qvh.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://kom.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://kpf.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://seu.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://onb.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oic.dianchejie.cn

JS:   e.message;  e.stack
来源：http://wpg.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gtm.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://opo.fanxiaobao.xyz

Go:   err.Error()
来源：http://fxy.zycfv.cn


<!-- 参考信息 -->