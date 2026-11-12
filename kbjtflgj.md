代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ddv.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kis.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://pfw.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jpg.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zol.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kgn.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cni.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mfv.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxb.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://xer.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swr.xinyue.icu

[F04] 追加写入文件
来源：http://sdu.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mya.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zye.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://joa.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bvw.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cpn.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://suc.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ztm.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ulj.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://zfb.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bcd.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://wjo.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://tbg.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://hbg.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oaf.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sxz.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://xgv.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://plw.yueranfly.top

[F06] 删除文件
来源：http://hxe.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://ypj.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://qky.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://oka.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://swf.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fan.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://jtp.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://utj.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://lmr.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://kzr.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqm.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://txa.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://deb.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvw.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://udm.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://icr.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mhq.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ydy.nanxuanxn.top

[F08] 遍历目录
来源：http://xna.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ynv.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vpq.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://vpt.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://hzc.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nul.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://voc.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://rxe.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://ayj.fehbvm.com

[F09] 获取文件大小
来源：http://oho.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://ani.daria6918.cn

PHP:  filesize("a.txt");
来源：http://vnh.hnxiangtu.top

JS:   fs.statSync("a.txt").size
来源：http://ilu.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://erh.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rnd.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bgf.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://jou.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://atb.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ubi.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dcg.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zog.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://psq.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://bcv.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mjg.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fwx.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cwj.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mfo.316326.xyz

[F11] 复制与移动文件
来源：http://eqp.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ubq.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fcl.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ffg.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xom.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://epi.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vyl.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://duw.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://huf.yj20258888.top

[F12] CSV 读写
来源：http://qjm.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rft.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ynz.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ygq.jinqigufen.top

TS:   // 同上
来源：http://myh.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ymd.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tyt.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uba.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://egl.hcnkem.com

================================================================================
来源：http://vgo.quarkkingdee.top

G. 面向对象
来源：http://sft.xingfuxueyuan.xyz

================================================================================
来源：http://ywu.mhx1999.top

[G01] 定义类
来源：http://lwk.ywan-chungtsiang.top

Py:   class User: pass
来源：http://utg.0kj1m.cn

PHP:  class User {}
来源：http://gzu.shanyushiyangtech.top

JS:   class User {}
来源：http://ilq.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://mqn.ydzc1.top

Java: class User {}
来源：http://fkj.xinyue.icu

Go:   type User struct { Name string }
来源：http://iqw.jinyuanbaomall.cn

Ruby: class User; end
来源：http://hnk.yangfankeji.com

C#:   class User {}
来源：http://okb.fktsv.cn

[G02] 构造函数
来源：http://qet.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://pru.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://ogd.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://gli.ivvv.top

TS:   constructor(public name: string) {}
来源：http://arc.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://apw.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dub.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://kns.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://wdp.yj202588.top

[G03] 实例属性
来源：http://tgp.feifeiyinyue.top

Py:   self.name = "x"
来源：http://jha.xylfe.cn

PHP:  public string $name = "x";
来源：http://sxb.xylfe.cn

JS:   this.name = "x";
来源：http://ion.gzhubu.top

TS:   name: string = "x";
来源：http://noe.vehdjk.com

Java: private String name;
来源：http://ckd.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gna.jinqigfzy.top

Ruby: @name = "x"
来源：http://gjb.yfazqb.com

C#:   public string Name { get; set; } = "x";
来源：http://acc.tarul.cn

[G04] 定义方法
来源：http://qgi.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://noc.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qyn.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://rgm.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://svs.nanxuanxn.top

Java: String greet() { return name; }
来源：http://usu.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ufa.ivvv.top

Ruby: def greet; @name; end
来源：http://xdk.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://ibr.shuidangran.top

[G05] 继承
来源：http://kfb.xylfe.cn

Py:   class Admin(User): pass
来源：http://hlh.tarul.cn

PHP:  class Admin extends User {}
来源：http://tup.shuidangran.top

JS:   class Admin extends User {}
来源：http://iel.zdqjudy.top

TS:   class Admin extends User {}
来源：http://bms.daria6918.cn

Java: class Admin extends User {}
来源：http://dhi.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://voh.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://ycl.nanxinkj.top

C#:   class Admin : User {}
来源：http://czw.yueranfly.top

[G06] 重写方法
来源：http://yez.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://sou.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://txf.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://ioj.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://abt.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://fml.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://osi.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://vee.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://vuu.jinqigufen.top

[G07] 调用父类方法
来源：http://rrf.aizwys.cn

Py:   super().greet()
来源：http://wrx.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://nok.sxryk.cn

JS:   super.greet();
来源：http://urp.aizwys.cn

TS:   super.greet();
来源：http://ohx.redwolf501.top

Java: super.greet();
来源：http://ejj.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxj.tarul.cn

Ruby: super
来源：http://mtn.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://plr.yongpay.top

[G08] 静态方法与属性
来源：http://mjh.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://byg.hywenlv.cn

PHP:  public static function f() {}
来源：http://mru.zhijiandao.cn

JS:   static f() {}
来源：http://hlw.pycfn.com

TS:   static f(): void {}
来源：http://wqi.xylfe.cn

Java: static void f() {}
来源：http://izb.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jyk.redwolf501.top

Ruby: def self.f; end
来源：http://kjn.birdmap.top

C#:   public static void F() {}
来源：http://tti.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://ntv.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://lxw.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://inp.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ttt.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://wme.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://fwg.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://koa.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xlj.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://nmr.0kj1m.cn

[G10] 访问控制
来源：http://rmk.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://pea.uphjek.com

PHP:  public / protected / private
来源：http://fws.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://gie.haohaochexian.top

TS:   public / protected / private
来源：http://bhy.jlsjyb.cn

Java: public / protected / private / 默认包级
来源：http://uwf.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://wvj.nanxinkj.top

Ruby: public / protected / private
来源：http://iss.xinyue.icu

C#:   public / protected / private / internal
来源：http://qiu.xuanzx.com

[G11] getter / setter
来源：http://nsn.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://beg.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ykj.sysykeji.top

JS:   get name() { return this._name; }
来源：http://bkx.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://rcf.sweek.top

Java: public String getName() { return name; }
来源：http://xym.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://lut.gogol.net.cn

Ruby: attr_accessor :name
来源：http://yaj.cheryme.top

C#:   public string Name { get; set; }
来源：http://bdl.gaohongyu789.top

[G12] 对象转字符串
来源：http://smc.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://vbu.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lsv.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://ukc.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://lsg.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://dfi.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://brd.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://zvn.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://dxp.iojbl.cn

[G13] 判断对象类型
来源：http://aji.52xcode.cn

Py:   isinstance(u, User)
来源：http://oad.guowangkeji.top

PHP:  $u instanceof User
来源：http://rcz.cashguo.top

JS:   u instanceof User
来源：http://crj.zhengqikj.top

TS:   u instanceof User
来源：http://rvb.xziqi.cn

Java: u instanceof User
来源：http://iuu.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dqi.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://rkm.bjfxy.top

C#:   u is User
来源：http://ugb.epnwcf.com

[G14] 数据类 / record
来源：http://mpf.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cuh.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://wru.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://yvg.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://nxj.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://fyf.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://mkh.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tew.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://rad.xinyue.icu

[G15] 枚举
来源：http://wqy.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mcg.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jml.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jss.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zej.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://bch.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://glk.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://nrs.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lzt.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://ghx.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fpt.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://rqy.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://ljc.sxryk.cn

TS:   Object.entries(obj)
来源：http://glz.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tql.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vge.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://gxn.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://bwz.xuetiantiany.cn

================================================================================
来源：http://ikh.yfazqb.com

H. 异常与错误处理
来源：http://unm.aizwys.cn

================================================================================
来源：http://pkz.yj20258888.top

[H01] try / catch 基础
来源：http://mwm.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cfg.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://edt.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ryf.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jnf.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ynz.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ewr.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzu.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ymb.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://ttm.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://whx.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jnc.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vzd.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://agt.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://jit.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbz.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kty.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eft.smart0.xyz

[H03] 主动抛出异常
来源：http://mty.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://oqh.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fdr.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://hjm.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://lfc.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qvo.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mpd.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ihk.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ggz.dashuyun.cn

[H04] 自定义异常类型
来源：http://fqc.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://isb.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://luy.uphjek.com

JS:   class MyError extends Error {}
来源：http://xtg.fehbvm.com

TS:   class MyError extends Error {}
来源：http://uwu.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://cin.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://krm.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://wuq.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://hig.jyoumei.cn

[H05] 捕获特定类型
来源：http://ldo.chenzaomai.com

Py:   except ValueError as e:
来源：http://pxs.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jzp.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://azy.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://bga.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://gac.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kjb.sweek.top

Ruby: rescue ArgumentError => e
来源：http://zdp.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rmb.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://bqt.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://kfx.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wwk.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://oqz.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://ajv.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cud.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://eey.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://agm.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://lic.zdbjq.cn

[H07] 断言
来源：http://xqe.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://rkr.sysykeji.top

PHP:  assert($x > 0);
来源：http://owt.gzhubu.top

JS:   console.assert(x > 0);
来源：http://eix.nanxuanxn.top


<!-- 参考信息 -->