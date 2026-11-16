代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://taq.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yuw.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mtj.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tjm.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gwx.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vip.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://nlj.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iqj.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://coc.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ldv.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xlt.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oqs.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://giv.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://cxw.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qmm.dianchejie.cn

[F04] 追加写入文件
来源：http://gdw.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bxd.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mlw.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cok.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qtr.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kci.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tvo.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pwj.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uso.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://nbp.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jdg.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://esu.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://lxr.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://gpg.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ucz.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://piq.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://roc.havefunace.top

C#:   File.Exists("a.txt")
来源：http://ths.vqdsnc.cn

[F06] 删除文件
来源：http://qqt.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://djx.ivvv.top

PHP:  unlink("a.txt");
来源：http://avt.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://fsu.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cqj.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pag.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://ynd.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://wzk.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://zhf.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://upe.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vkw.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ild.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvp.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jor.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yje.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kyy.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gbl.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jke.jqgfzy.top

[F08] 遍历目录
来源：http://lub.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dzo.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qrf.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://hfi.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://cxm.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vas.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://cqe.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://etu.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://tvy.hesvh.cn

[F09] 获取文件大小
来源：http://how.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://fei.mhx1999.top

PHP:  filesize("a.txt");
来源：http://uos.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://ixc.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://acm.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zvg.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yet.ivvv.top

Ruby: File.size("a.txt")
来源：http://bfx.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://ojm.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://frw.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tvt.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rcl.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xvb.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://gnk.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvy.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sts.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yrc.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vnl.hesvh.cn

[F11] 复制与移动文件
来源：http://ayl.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://acp.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vco.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mlk.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqj.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bye.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ewm.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jqd.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ivv.svipenyu.cn

[F12] CSV 读写
来源：http://cgf.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fto.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fiv.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xot.andypj.xyz

TS:   // 同上
来源：http://bzf.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zej.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rzs.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mns.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vao.haohaochexian.top

================================================================================
来源：http://boa.chenzaomai.com

G. 面向对象
来源：http://evi.iojbl.cn

================================================================================
来源：http://oqh.birdmap.top

[G01] 定义类
来源：http://rmm.zhiwuduotai.top

Py:   class User: pass
来源：http://xcj.bbcook.cn

PHP:  class User {}
来源：http://dzu.xuanzx.com

JS:   class User {}
来源：http://ljx.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://qwq.nanxuanxn.top

Java: class User {}
来源：http://wxe.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://kca.jlsjyb.cn

Ruby: class User; end
来源：http://cdk.dashuyun.cn

C#:   class User {}
来源：http://nwe.sysykeji.top

[G02] 构造函数
来源：http://kun.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://dfe.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://tif.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://uyw.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://yjt.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://prv.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hsd.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://ynu.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://gjv.jqgufenzy.top

[G03] 实例属性
来源：http://lmw.daxiang520.top

Py:   self.name = "x"
来源：http://rhm.yuanzhike.top

PHP:  public string $name = "x";
来源：http://nfw.shangyingyoupin.top

JS:   this.name = "x";
来源：http://qiy.ppjwa.cn

TS:   name: string = "x";
来源：http://vti.yfazqb.com

Java: private String name;
来源：http://evp.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jcb.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://fez.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://pag.zhengqikj.top

[G04] 定义方法
来源：http://uzq.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://etu.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://rrj.52xcode.cn

JS:   greet() { return this.name; }
来源：http://plw.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://edb.tarul.cn

Java: String greet() { return name; }
来源：http://lom.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvj.shzxlz.cn

Ruby: def greet; @name; end
来源：http://wss.shuidangran.top

C#:   public string Greet() => Name;
来源：http://bwo.xinyue.icu

[G05] 继承
来源：http://eyg.andypj.xyz

Py:   class Admin(User): pass
来源：http://xwl.bbcook.cn

PHP:  class Admin extends User {}
来源：http://lwo.tarul.cn

JS:   class Admin extends User {}
来源：http://uuq.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://hvj.jianghu66.top

Java: class Admin extends User {}
来源：http://sgn.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zew.sxryk.cn

Ruby: class Admin < User; end
来源：http://wac.fengsongda.top

C#:   class Admin : User {}
来源：http://pnh.tarul.cn

[G06] 重写方法
来源：http://eew.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://yag.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://grj.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://jyz.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://vic.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://jmu.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hdb.cheryme.top

Ruby: def greet; "admin"; end
来源：http://olc.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://orj.zhixingplan.top

[G07] 调用父类方法
来源：http://vqy.hesvh.cn

Py:   super().greet()
来源：http://pkt.sjlbkw.cn

PHP:  parent::greet();
来源：http://ver.cashguo.top

JS:   super.greet();
来源：http://nlb.hfpthk.cn

TS:   super.greet();
来源：http://trk.zhengqikj.top

Java: super.greet();
来源：http://hfu.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iau.yfazqb.com

Ruby: super
来源：http://sex.hammf.cn

C#:   base.Greet();
来源：http://vby.vqdsnc.cn

[G08] 静态方法与属性
来源：http://mfu.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sfb.ctjpmb.com

PHP:  public static function f() {}
来源：http://awp.jlsjyb.cn

JS:   static f() {}
来源：http://fmy.jianghu66.top

TS:   static f(): void {}
来源：http://lor.316326.xyz

Java: static void f() {}
来源：http://mli.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fvl.xziqi.cn

Ruby: def self.f; end
来源：http://zxm.sjlbkw.cn

C#:   public static void F() {}
来源：http://pfi.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://klf.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://gtg.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://gfb.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bzg.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://rag.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://qyy.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://dth.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ddi.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://nwy.fanxiaobao.xyz

[G10] 访问控制
来源：http://fhn.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ato.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://twy.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://vwv.aibaodan.cn

TS:   public / protected / private
来源：http://slo.316326.xyz

Java: public / protected / private / 默认包级
来源：http://kgf.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uia.xylfe.cn

Ruby: public / protected / private
来源：http://dsg.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://qcv.zhijiandao.cn

[G11] getter / setter
来源：http://ezz.yj20258888.top

Py:   @property 与 @x.setter
来源：http://wbr.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oyn.hesvh.cn

JS:   get name() { return this._name; }
来源：http://cub.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://wwu.c1oappe.top

Java: public String getName() { return name; }
来源：http://lxt.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vtk.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://rzo.jianghu66.top

C#:   public string Name { get; set; }
来源：http://kqx.pengpengdd.cyou

[G12] 对象转字符串
来源：http://jix.tanke756.top

Py:   def __str__(self): return self.name
来源：http://ncu.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://obl.sxryk.cn

JS:   toString() { return this.name; }
来源：http://kgl.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://cuh.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://oby.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://tml.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://ilx.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://njj.havefunace.top

[G13] 判断对象类型
来源：http://azt.epnwcf.com

Py:   isinstance(u, User)
来源：http://buo.bbcook.cn

PHP:  $u instanceof User
来源：http://mvt.fzhhl.top

JS:   u instanceof User
来源：http://oqp.bbcook.cn

TS:   u instanceof User
来源：http://ran.ydjk.org.cn

Java: u instanceof User
来源：http://ald.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kwm.316326.xyz

Ruby: u.is_a?(User)
来源：http://czh.52xcode.cn

C#:   u is User
来源：http://wze.vqdsnc.cn

[G14] 数据类 / record
来源：http://dkq.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ere.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://llm.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://tqd.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://xdu.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://mor.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://hzu.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rfv.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://rso.sysykeji.top

[G15] 枚举
来源：http://vze.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sef.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vrz.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xeb.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhp.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://dyb.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ibf.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://fia.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bht.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://fpu.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xtw.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://jnn.tarul.cn

JS:   Object.entries(obj)
来源：http://ufh.nanxinkj.top

TS:   Object.entries(obj)
来源：http://qcg.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://psc.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zjb.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://sye.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://oct.jinghuilouyu.cn

================================================================================
来源：http://dfl.mhx1999.top

H. 异常与错误处理
来源：http://wql.jiagoushi.top

================================================================================
来源：http://ais.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://yag.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ckv.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vax.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vhx.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zrw.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lig.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://npq.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nau.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akw.hnqzz.top

[H02] finally / ensure 收尾
来源：http://rcx.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://lvf.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ckr.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://led.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oqk.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://jzj.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gpg.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zxj.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://peh.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://zzv.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://iaa.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jeb.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://mhy.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://tiw.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jsg.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://huj.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xol.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://hvh.daxiang520.top

[H04] 自定义异常类型
来源：http://sve.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://bpu.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://cyl.wangdashe.top

JS:   class MyError extends Error {}
来源：http://wtw.ivvv.top

TS:   class MyError extends Error {}
来源：http://ilr.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://ejz.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pqf.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://spn.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://drn.yueranfly.top

[H05] 捕获特定类型
来源：http://tth.tianlin.xyz

Py:   except ValueError as e:
来源：http://muj.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hcx.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://xyb.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://rby.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://fhl.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rxe.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://cga.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qif.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://ndo.52xcode.cn

Py:   value = d.get("k") or default
来源：http://ckb.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://xse.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://kil.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://fpk.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ybn.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hqu.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://oqq.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://kxo.xylfe.cn


<!-- 参考信息 -->