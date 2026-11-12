代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mys.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uiu.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zuc.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tyf.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bdg.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gyb.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://kes.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://epb.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dys.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vkx.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hzk.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rcm.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnm.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://mve.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zzl.snrcjt.cn

[F04] 追加写入文件
来源：http://hll.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kkp.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xtm.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zin.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gkf.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fug.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dor.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://btu.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://etn.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://tkl.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ilh.yj202588.top

PHP:  file_exists("a.txt");
来源：http://pot.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://kuw.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://mnr.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lrj.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kko.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://pbq.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://lyr.sjlbkw.cn

[F06] 删除文件
来源：http://msq.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://tjq.fengsongda.top

PHP:  unlink("a.txt");
来源：http://qad.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://vhd.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://avr.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ghf.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://hlk.ivvv.top

Ruby: File.delete("a.txt")
来源：http://kyr.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://hyx.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://djz.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lqg.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wju.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vtr.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odd.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://epr.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jeq.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kxc.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ako.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://zpf.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yxh.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ujx.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://qav.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://oew.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lgh.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xxh.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://bgn.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://wzg.meibo888.top

[F09] 获取文件大小
来源：http://cpi.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://zqw.fktsv.cn

PHP:  filesize("a.txt");
来源：http://wsq.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://raf.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://mpv.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ias.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vsg.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://dcs.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://nnc.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://yww.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rfq.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://laz.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kly.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://wzz.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wdw.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pxy.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wuh.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wtv.zdqjudy.top

[F11] 复制与移动文件
来源：http://khs.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vce.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zsk.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yal.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xis.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsp.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvk.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ate.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ytj.tarul.cn

[F12] CSV 读写
来源：http://ijr.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kbj.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xwe.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://etr.jinqigufen.top

TS:   // 同上
来源：http://tzs.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lpk.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kby.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vtf.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://eae.zhixingplan.top

================================================================================
来源：http://fby.ydzc1.top

G. 面向对象
来源：http://sri.gaohongyu789.top

================================================================================
来源：http://nci.meibo888.top

[G01] 定义类
来源：http://kls.yfazqb.com

Py:   class User: pass
来源：http://trq.yj202588.top

PHP:  class User {}
来源：http://rha.ivvv.top

JS:   class User {}
来源：http://crx.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://atg.yongpay.top

Java: class User {}
来源：http://lig.0kj1m.cn

Go:   type User struct { Name string }
来源：http://cog.hcnkem.com

Ruby: class User; end
来源：http://kge.jyoumei.cn

C#:   class User {}
来源：http://bkj.hfpthk.cn

[G02] 构造函数
来源：http://ygy.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://hil.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://ooe.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://dvy.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://htb.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://prb.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bve.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://daz.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://hve.fzhhl.top

[G03] 实例属性
来源：http://vdx.bbcook.cn

Py:   self.name = "x"
来源：http://qqo.yonumen.top

PHP:  public string $name = "x";
来源：http://mur.epnwcf.com

JS:   this.name = "x";
来源：http://yvj.shuidangran.top

TS:   name: string = "x";
来源：http://vqn.yj202588.top

Java: private String name;
来源：http://avc.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rsj.hcnkem.com

Ruby: @name = "x"
来源：http://tcs.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://msc.pycfn.com

[G04] 定义方法
来源：http://hoe.meibo888.top

Py:   def greet(self): return self.name
来源：http://gtt.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xro.guannengcc.top

JS:   greet() { return this.name; }
来源：http://lgg.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://nwx.jiagoushi.top

Java: String greet() { return name; }
来源：http://zaf.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rvf.uphjek.com

Ruby: def greet; @name; end
来源：http://our.52xcode.cn

C#:   public string Greet() => Name;
来源：http://ptk.hcnkem.com

[G05] 继承
来源：http://lau.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://lpe.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://bwa.yvedp.cn

JS:   class Admin extends User {}
来源：http://xbc.yonumen.top

TS:   class Admin extends User {}
来源：http://zqi.gogol.net.cn

Java: class Admin extends User {}
来源：http://upa.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qrj.guannengcc.top

Ruby: class Admin < User; end
来源：http://xut.iojbl.cn

C#:   class Admin : User {}
来源：http://qbp.sufxvd.cn

[G06] 重写方法
来源：http://ggg.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://vbh.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ayp.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://uob.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://vsf.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://ydr.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kgu.ivvv.top

Ruby: def greet; "admin"; end
来源：http://fwh.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://own.daria6918.cn

[G07] 调用父类方法
来源：http://opn.yuxming.cn

Py:   super().greet()
来源：http://esi.aizwys.cn

PHP:  parent::greet();
来源：http://lxr.pycfn.com

JS:   super.greet();
来源：http://nro.uphjek.com

TS:   super.greet();
来源：http://rfm.guowangkeji.top

Java: super.greet();
来源：http://xjh.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zwk.ydjk.org.cn

Ruby: super
来源：http://ayz.ybcxt.top

C#:   base.Greet();
来源：http://vin.ehwqpu.com

[G08] 静态方法与属性
来源：http://emm.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://otm.chenlongwang.top

PHP:  public static function f() {}
来源：http://bpj.uphjek.com

JS:   static f() {}
来源：http://fcl.vehdjk.com

TS:   static f(): void {}
来源：http://try.ywan-chungtsiang.top

Java: static void f() {}
来源：http://xys.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pts.yanxiufei.cn

Ruby: def self.f; end
来源：http://ihh.ybcxt.top

C#:   public static void F() {}
来源：http://iwh.wangdashe.top

[G09] 接口 / 抽象类
来源：http://ixx.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://njy.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ahu.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wei.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://rjy.sweek.top

Java: interface Shape { double area(); }
来源：http://sru.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://yox.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wmd.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://cns.hysaishi.cn

[G10] 访问控制
来源：http://hfm.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://ceo.dianchejie.cn

PHP:  public / protected / private
来源：http://erg.hammf.cn

JS:   #private 字段；其余公开
来源：http://lqg.shangyingyoupin.top

TS:   public / protected / private
来源：http://cze.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://ydj.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gmm.ydjk.org.cn

Ruby: public / protected / private
来源：http://bho.hysaishi.cn

C#:   public / protected / private / internal
来源：http://hsr.hnxiangtu.top

[G11] getter / setter
来源：http://faw.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://cqe.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://owj.sysykeji.top

JS:   get name() { return this._name; }
来源：http://eld.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://zzy.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://vrh.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cve.shuidangran.top

Ruby: attr_accessor :name
来源：http://bdq.bjfxy.top

C#:   public string Name { get; set; }
来源：http://nqg.hammf.cn

[G12] 对象转字符串
来源：http://wcy.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://bxv.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oca.birdmap.top

JS:   toString() { return this.name; }
来源：http://ihb.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://hyt.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://mfv.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://jwc.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://hsb.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://pfw.cucudq.cn

[G13] 判断对象类型
来源：http://vvj.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://ven.yuxming.cn

PHP:  $u instanceof User
来源：http://ytj.xuanzx.com

JS:   u instanceof User
来源：http://xyz.shuidangran.top

TS:   u instanceof User
来源：http://oaj.yj20258888.top

Java: u instanceof User
来源：http://gsb.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://upo.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://iep.tian-w.cn

C#:   u is User
来源：http://twn.zhijiandao.cn

[G14] 数据类 / record
来源：http://tnw.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lpo.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://xro.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://hks.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://vwp.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://eae.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://mki.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhf.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://gxf.xuetiantiany.cn

[G15] 枚举
来源：http://ord.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bgy.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://geq.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jjm.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jmv.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://eby.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zfh.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://ucd.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wqu.cheryme.top

[G16] 对象转数组 / 字典
来源：http://vmc.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tcn.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://ufq.aizwys.cn

JS:   Object.entries(obj)
来源：http://ove.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://yta.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pmg.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://laq.ybcxt.top

Ruby: obj.instance_variables
来源：http://efg.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://vru.fktsv.cn

================================================================================
来源：http://tyk.shanyushiyangtech.top

H. 异常与错误处理
来源：http://lca.9152youxi.cn

================================================================================
来源：http://xdd.tanke756.top

[H01] try / catch 基础
来源：http://svu.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hgn.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kak.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://glh.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pyp.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://obp.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ukv.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://adm.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eun.fzhhl.top

[H02] finally / ensure 收尾
来源：http://xln.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://itb.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://gpx.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xdo.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mvz.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://uwo.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rks.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://her.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sco.zhoulong.xyz

[H03] 主动抛出异常
来源：http://fgk.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://uyr.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lha.yj202588.top

JS:   throw new Error("错误信息");
来源：http://axs.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://lum.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mmv.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pxz.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fap.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://xgq.yj20258888.top

[H04] 自定义异常类型
来源：http://mvs.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://wka.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vqr.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://rpl.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://vfz.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://fmz.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yjw.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://iwu.daria6918.cn

C#:   class MyException : Exception {}
来源：http://ylw.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://eme.iojbl.cn

Py:   except ValueError as e:
来源：http://kdu.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owx.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://dcq.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ayp.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://pnv.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nbv.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://fmb.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vdy.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://zaq.shuidangran.top

Py:   value = d.get("k") or default
来源：http://kks.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://lgq.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://aud.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://agv.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xyi.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://grc.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://zaf.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://yhn.bbcook.cn


<!-- 参考信息 -->