代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tds.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwn.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xcd.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://noh.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tst.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fad.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://zco.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://war.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wjz.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dkj.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxs.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwn.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yji.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://aar.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://geg.snrcjt.cn

[F04] 追加写入文件
来源：http://yon.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qgw.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bid.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zel.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azk.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yrb.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ggm.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ssh.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://krr.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://ecx.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ymg.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://weh.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://jed.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://mvj.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://und.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qef.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://cuj.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://tsy.shuidangran.top

[F06] 删除文件
来源：http://cqt.smart0.xyz

Py:   os.remove("a.txt")
来源：http://clo.yfazqb.com

PHP:  unlink("a.txt");
来源：http://uxc.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://urc.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fwd.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://scs.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://lwd.uphjek.com

Ruby: File.delete("a.txt")
来源：http://aha.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://vkp.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://cnz.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ceo.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svt.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://den.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqq.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://les.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mwx.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zra.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xhu.tarul.cn

[F08] 遍历目录
来源：http://vkq.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xrj.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vtp.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://vxe.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://xek.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mng.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://apk.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://qlk.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://inv.gogol.net.cn

[F09] 获取文件大小
来源：http://iun.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://wup.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://jow.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://feo.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://nrt.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uui.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ymx.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://gqb.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://kxz.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://wbv.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pqw.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ipu.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fla.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://ags.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xyv.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xwi.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wvv.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lrp.daria6918.cn

[F11] 复制与移动文件
来源：http://qhw.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jhr.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iwb.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zig.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cvg.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xnz.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ari.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jgm.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dtj.hcnkem.com

[F12] CSV 读写
来源：http://zjm.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://six.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gyg.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://buq.tian-w.cn

TS:   // 同上
来源：http://fux.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oji.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://naf.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://atx.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://krs.yfazqb.com

================================================================================
来源：http://rma.gaohongyu789.top

G. 面向对象
来源：http://eav.shuidangran.top

================================================================================
来源：http://zck.316326.xyz

[G01] 定义类
来源：http://spt.shzxlz.cn

Py:   class User: pass
来源：http://mht.havefunace.top

PHP:  class User {}
来源：http://ggq.fzhhl.top

JS:   class User {}
来源：http://uph.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://sep.yanxiufei.cn

Java: class User {}
来源：http://xao.yueranfly.top

Go:   type User struct { Name string }
来源：http://mxs.0kj1m.cn

Ruby: class User; end
来源：http://bdb.wangdashe.top

C#:   class User {}
来源：http://uvl.bjfxy.top

[G02] 构造函数
来源：http://puw.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://zrg.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://xuv.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wiw.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://pcu.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://src.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rgp.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://pax.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://jjn.cheryme.top

[G03] 实例属性
来源：http://fza.pengpengdd.cyou

Py:   self.name = "x"
来源：http://voq.9152youxi.cn

PHP:  public string $name = "x";
来源：http://zhs.xuanzx.com

JS:   this.name = "x";
来源：http://qhg.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://lzf.gzhubu.top

Java: private String name;
来源：http://vzu.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bni.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://xee.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://dfj.yuanzhike.top

[G04] 定义方法
来源：http://qpx.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://zlj.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dmb.vehdjk.com

JS:   greet() { return this.name; }
来源：http://glp.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://lph.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://hsn.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tis.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://klv.vehdjk.com

C#:   public string Greet() => Name;
来源：http://bhr.havefunace.top

[G05] 继承
来源：http://hdr.iojbl.cn

Py:   class Admin(User): pass
来源：http://euv.hammf.cn

PHP:  class Admin extends User {}
来源：http://jeh.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://qhj.yfazqb.com

TS:   class Admin extends User {}
来源：http://jad.sysykeji.top

Java: class Admin extends User {}
来源：http://rus.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isa.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://fjc.zhongyouzk.top

C#:   class Admin : User {}
来源：http://rjm.pycfn.com

[G06] 重写方法
来源：http://tbg.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://yzm.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sjx.ivvv.top

JS:   greet() { return "admin"; }
来源：http://rfu.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://zng.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://mye.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bei.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://llo.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://oka.nanxinkj.top

[G07] 调用父类方法
来源：http://xtq.jiagoushi.top

Py:   super().greet()
来源：http://bfv.vehdjk.com

PHP:  parent::greet();
来源：http://bfx.wangdashe.top

JS:   super.greet();
来源：http://eib.zhengqikj.top

TS:   super.greet();
来源：http://ajz.fengsongda.top

Java: super.greet();
来源：http://lxo.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chy.zdqjudy.top

Ruby: super
来源：http://nat.uphjek.com

C#:   base.Greet();
来源：http://bhd.mhx1999.top

[G08] 静态方法与属性
来源：http://rvu.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hhk.zhengqikj.top

PHP:  public static function f() {}
来源：http://uod.hnqzz.top

JS:   static f() {}
来源：http://sye.gaohongyu789.top

TS:   static f(): void {}
来源：http://uhi.nwbrower.top

Java: static void f() {}
来源：http://qqb.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wsw.guowangkeji.top

Ruby: def self.f; end
来源：http://rid.9152youxi.cn

C#:   public static void F() {}
来源：http://kxw.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://pox.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://cuf.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://wwx.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xdi.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://czx.cashguo.top

Java: interface Shape { double area(); }
来源：http://ufe.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://dez.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kgv.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://gam.pycfn.com

[G10] 访问控制
来源：http://vbh.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://zit.9152youxi.cn

PHP:  public / protected / private
来源：http://npa.ybcxt.top

JS:   #private 字段；其余公开
来源：http://ipm.gzhubu.top

TS:   public / protected / private
来源：http://uaw.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://rqx.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://szp.hcnkem.com

Ruby: public / protected / private
来源：http://kfz.jianghu66.top

C#:   public / protected / private / internal
来源：http://ufa.gogol.net.cn

[G11] getter / setter
来源：http://fds.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://xkw.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zyt.cashguo.top

JS:   get name() { return this._name; }
来源：http://tmq.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://swy.ybcxt.top

Java: public String getName() { return name; }
来源：http://hqm.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ioj.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://yeh.xuanzx.com

C#:   public string Name { get; set; }
来源：http://yzu.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://gob.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://wna.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uvx.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://icy.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://vme.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://mpk.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://rfu.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://naa.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://omr.sxryk.cn

[G13] 判断对象类型
来源：http://prn.jiagoushi.top

Py:   isinstance(u, User)
来源：http://dch.tian-w.cn

PHP:  $u instanceof User
来源：http://rdz.uphjek.com

JS:   u instanceof User
来源：http://aza.jiagoushi.top

TS:   u instanceof User
来源：http://fbq.shzxlz.cn

Java: u instanceof User
来源：http://bif.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vkm.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://djf.snrcjt.cn

C#:   u is User
来源：http://pwe.cheryme.top

[G14] 数据类 / record
来源：http://oqq.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://veh.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ccu.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sti.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://nih.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://iyl.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://mhv.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tmu.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://dea.jinghuilouyu.cn

[G15] 枚举
来源：http://duz.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://amw.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gyz.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mmi.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ydn.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://tlq.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ybw.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://gam.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pue.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://nvg.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nrl.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://pcr.yonumen.top

JS:   Object.entries(obj)
来源：http://vqw.haohaochexian.top

TS:   Object.entries(obj)
来源：http://cgy.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oly.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wjf.daria6918.cn

Ruby: obj.instance_variables
来源：http://uqu.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://mgy.hesvh.cn

================================================================================
来源：http://itx.wangshuangyany.cn

H. 异常与错误处理
来源：http://jld.yj20258.top

================================================================================
来源：http://ipn.ehwqpu.com

[H01] try / catch 基础
来源：http://pbg.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vqg.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fkg.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kea.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ush.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rrk.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rbe.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yzo.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yvq.tanke756.top

[H02] finally / ensure 收尾
来源：http://ytj.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://cuf.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tqo.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://job.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://scw.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://glj.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fko.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eml.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vnl.uphjek.com

[H03] 主动抛出异常
来源：http://ggi.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://dcp.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kcl.316326.xyz

JS:   throw new Error("错误信息");
来源：http://rho.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://adr.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sov.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hsq.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://exi.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://tew.mhx1999.top

[H04] 自定义异常类型
来源：http://tke.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://mvx.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sxe.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://svy.ivvv.top

TS:   class MyError extends Error {}
来源：http://lkn.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://qpp.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://psx.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://frq.sysykeji.top

C#:   class MyException : Exception {}
来源：http://jhv.ppjwa.cn

[H05] 捕获特定类型
来源：http://xvs.epnwcf.com

Py:   except ValueError as e:
来源：http://cgl.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ppq.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://lki.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://sgz.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://xul.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zzd.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://vha.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://typ.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://uiw.daxiang520.top

Py:   value = d.get("k") or default
来源：http://kek.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jgv.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://obf.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://tjh.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://omp.fengsongda.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mhr.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://mnb.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://yii.guowangkeji.top


<!-- 参考信息 -->