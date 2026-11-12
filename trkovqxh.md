代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://psa.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eio.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://wmd.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rht.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://alq.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akw.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mco.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jzj.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://enk.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://bkx.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lwc.vqdsnc.cn

[F04] 追加写入文件
来源：http://mdo.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kus.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cbw.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ylv.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wms.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gdk.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wpw.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zta.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyc.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://plt.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qme.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://jfk.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://hta.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://ttb.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ptr.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pjw.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://lzv.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://gma.zhengqikj.top

[F06] 删除文件
来源：http://trp.wangdashe.top

Py:   os.remove("a.txt")
来源：http://gxm.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://ujk.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://srw.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://ymy.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://joh.cheryme.top

Go:   os.Remove("a.txt")
来源：http://kwx.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://dql.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://syd.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://bfv.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pqf.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mne.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdh.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jya.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rmr.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ibg.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qdh.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hsm.gotoacloud.top

[F08] 遍历目录
来源：http://hpp.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://swf.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pra.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://tue.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://xmr.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mdb.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qvi.jianghu66.top

Ruby: Dir.children("dir")
来源：http://geg.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://qvg.nanxuanxn.top

[F09] 获取文件大小
来源：http://wte.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://iif.52xcode.cn

PHP:  filesize("a.txt");
来源：http://sle.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://poj.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://srg.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tfd.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://olj.gzhubu.top

Ruby: File.size("a.txt")
来源：http://kev.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://hgg.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://fga.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kqw.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wit.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oxb.zycfv.cn

TS:   path.extname("a.txt")
来源：http://qyy.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lqx.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ibb.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hfv.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwq.yvedp.cn

[F11] 复制与移动文件
来源：http://dif.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://umt.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ire.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkl.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cln.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://toc.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cyi.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mpf.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://quw.shangyingyoupin.top

[F12] CSV 读写
来源：http://tek.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://buf.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://boj.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ngw.havefunace.top

TS:   // 同上
来源：http://nbs.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://szf.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qxh.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uxi.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://blf.jinqigufen.top

================================================================================
来源：http://cls.yvedp.cn

G. 面向对象
来源：http://fnk.yfazqb.com

================================================================================
来源：http://rqx.svipenyu.cn

[G01] 定义类
来源：http://xvr.0kj1m.cn

Py:   class User: pass
来源：http://lcc.nwbrower.top

PHP:  class User {}
来源：http://nsd.ydzc1.top

JS:   class User {}
来源：http://zjm.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://onl.bbcook.cn

Java: class User {}
来源：http://gkf.dianchejie.cn

Go:   type User struct { Name string }
来源：http://ylg.guowangkeji.top

Ruby: class User; end
来源：http://txp.hesvh.cn

C#:   class User {}
来源：http://lsz.zhijiandao.cn

[G02] 构造函数
来源：http://mlp.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://pgk.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://vob.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://irb.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://rfa.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://lla.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kjd.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://vmw.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://mcg.hysaishi.cn

[G03] 实例属性
来源：http://ckr.xuanzx.com

Py:   self.name = "x"
来源：http://rxl.cucudq.cn

PHP:  public string $name = "x";
来源：http://eao.ehwqpu.com

JS:   this.name = "x";
来源：http://dns.cucudq.cn

TS:   name: string = "x";
来源：http://fua.zhixingplan.top

Java: private String name;
来源：http://yvs.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kxl.shzxlz.cn

Ruby: @name = "x"
来源：http://fzl.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://sdg.cheryme.top

[G04] 定义方法
来源：http://mqy.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://xtx.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ijp.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://eff.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://hjm.bbcook.cn

Java: String greet() { return name; }
来源：http://hgu.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dle.bbcook.cn

Ruby: def greet; @name; end
来源：http://kbw.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://tts.feifeiyinyue.top

[G05] 继承
来源：http://oto.hesvh.cn

Py:   class Admin(User): pass
来源：http://qjp.havefunace.top

PHP:  class Admin extends User {}
来源：http://nzu.pycfn.com

JS:   class Admin extends User {}
来源：http://hbk.hysaishi.cn

TS:   class Admin extends User {}
来源：http://xbh.quarkkingdee.top

Java: class Admin extends User {}
来源：http://pht.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://doj.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://kpb.316326.xyz

C#:   class Admin : User {}
来源：http://bzb.sweek.top

[G06] 重写方法
来源：http://sdk.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://uon.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yqy.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://jeh.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://ill.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://hmy.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://anw.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://aso.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://xem.daxiang520.top

[G07] 调用父类方法
来源：http://qsh.birdmap.top

Py:   super().greet()
来源：http://kgc.yj202588.top

PHP:  parent::greet();
来源：http://era.guowangkeji.top

JS:   super.greet();
来源：http://bof.cqqwz.cn

TS:   super.greet();
来源：http://nuz.nanxinkj.top

Java: super.greet();
来源：http://gxi.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wrj.yuxming.cn

Ruby: super
来源：http://ncx.sweek.top

C#:   base.Greet();
来源：http://jvn.vehdjk.com

[G08] 静态方法与属性
来源：http://wsw.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oub.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://pvb.zhiwuduotai.top

JS:   static f() {}
来源：http://yyu.cdnleiting.top

TS:   static f(): void {}
来源：http://cyv.ivvv.top

Java: static void f() {}
来源：http://xbg.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://avd.chenlongwang.top

Ruby: def self.f; end
来源：http://qma.gogol.net.cn

C#:   public static void F() {}
来源：http://bzy.shuidangran.top

[G09] 接口 / 抽象类
来源：http://hcm.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://prd.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wrx.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dya.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://aqd.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://uwb.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://bpy.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uqi.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://wgh.kuanghao11.cn

[G10] 访问控制
来源：http://qjt.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://mpt.quarkkingdee.top

PHP:  public / protected / private
来源：http://gqf.sxryk.cn

JS:   #private 字段；其余公开
来源：http://cvy.pengpengdd.cyou

TS:   public / protected / private
来源：http://pqn.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://urx.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wjd.shuidangran.top

Ruby: public / protected / private
来源：http://qcy.ehwqpu.com

C#:   public / protected / private / internal
来源：http://tfw.smart0.xyz

[G11] getter / setter
来源：http://isx.tanke756.top

Py:   @property 与 @x.setter
来源：http://frr.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://hpb.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://wkn.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://tvv.uphjek.com

Java: public String getName() { return name; }
来源：http://qoe.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fni.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://qtn.yj20258888.top

C#:   public string Name { get; set; }
来源：http://lxd.chenjidiqi.icu

[G12] 对象转字符串
来源：http://vwh.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://kxs.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://gix.xuanzx.com

JS:   toString() { return this.name; }
来源：http://kbv.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://jfr.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://jub.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hot.smart0.xyz

Ruby: def to_s; @name; end
来源：http://hnq.yonumen.top

C#:   public override string ToString() => Name;
来源：http://vda.aibaodan.cn

[G13] 判断对象类型
来源：http://wni.svipenyu.cn

Py:   isinstance(u, User)
来源：http://vnw.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://eoy.zdqjudy.top

JS:   u instanceof User
来源：http://veb.pengpengdd.cyou

TS:   u instanceof User
来源：http://ect.zhiwuduotai.top

Java: u instanceof User
来源：http://nnr.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vyv.fktsv.cn

Ruby: u.is_a?(User)
来源：http://cpi.jyoumei.cn

C#:   u is User
来源：http://zxx.sweek.top

[G14] 数据类 / record
来源：http://zhy.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uhz.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://zoj.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://und.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://xpa.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://hqu.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://qoe.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yrk.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://ale.gaohongyu789.top

[G15] 枚举
来源：http://hov.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lwz.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gtf.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://evm.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ien.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://ayi.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://efs.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://kfd.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yvi.havefunace.top

[G16] 对象转数组 / 字典
来源：http://mzm.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oqr.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://xlx.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://gkk.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://vmz.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bku.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://inb.bjfxy.top

Ruby: obj.instance_variables
来源：http://dwk.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://wxu.xinyue.icu

================================================================================
来源：http://yxe.tian-w.cn

H. 异常与错误处理
来源：http://tvs.vehdjk.com

================================================================================
来源：http://ckt.redwolf501.top

[H01] try / catch 基础
来源：http://tdm.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tqm.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tat.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hfh.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ite.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jhv.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pyv.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zom.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oxs.havefunace.top

[H02] finally / ensure 收尾
来源：http://raw.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://zuj.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ttf.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://toy.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aes.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ncu.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ipg.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mlb.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qnl.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://uni.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://bcy.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rfm.meibo888.top

JS:   throw new Error("错误信息");
来源：http://rtp.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://ehk.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zox.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nby.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mbw.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://jpg.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://hqv.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://dzz.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://qfn.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://hmd.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://rka.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://anp.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://umb.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://vcy.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://niq.yangfankeji.com

[H05] 捕获特定类型
来源：http://hec.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://eyi.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vbx.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://sbf.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://xuo.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://ftn.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uha.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://ccc.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fiz.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://ktx.cucudq.cn

Py:   value = d.get("k") or default
来源：http://bzt.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://gor.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://urx.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rmn.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hza.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ljl.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://duz.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://uqw.pycfn.com

[H07] 断言
来源：http://pgh.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://vyv.bjfxy.top

PHP:  assert($x > 0);
来源：http://yos.yfazqb.com

JS:   console.assert(x > 0);
来源：http://okn.fanxiaobao.xyz


<!-- 参考信息 -->