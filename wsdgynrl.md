代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://obj.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bkj.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://veo.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://epj.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ray.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vcg.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://vuk.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://scb.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgd.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ohk.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ocv.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dhx.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mph.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://irj.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xxz.kuanghao11.cn

[F04] 追加写入文件
来源：http://lyy.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kul.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ypm.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxr.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sok.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://chq.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gzq.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://keq.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qkf.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://zcx.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ntk.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://mpx.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://bqm.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://qjl.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kuk.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qdt.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://vmq.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://fsf.jinghuilouyu.cn

[F06] 删除文件
来源：http://cvt.guannengcc.top

Py:   os.remove("a.txt")
来源：http://lid.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://bcl.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://aju.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://adj.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhw.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://vvt.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://wsr.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://shp.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://veu.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yhl.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pox.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntb.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zwm.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://btr.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dph.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tps.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lyb.zdbjq.cn

[F08] 遍历目录
来源：http://duf.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bjv.xuetiantiany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cyn.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://xtx.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://ewr.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jfw.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://idw.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://voe.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://jgm.yuxming.cn

[F09] 获取文件大小
来源：http://wse.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://qbt.cashguo.top

PHP:  filesize("a.txt");
来源：http://kwc.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://yqp.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://edb.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://acf.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rkf.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://bar.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://vxy.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://lmy.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vtz.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cpo.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nri.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://akk.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lgr.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rij.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ixx.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ijk.nanxuanxn.top

[F11] 复制与移动文件
来源：http://xgm.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kwx.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ulq.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ddg.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcs.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hwt.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rrt.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgw.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wpp.fehbvm.com

[F12] CSV 读写
来源：http://wgu.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bzf.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gvm.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jnq.guannengcc.top

TS:   // 同上
来源：http://rog.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://irc.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fel.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lze.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mey.52xcode.cn

================================================================================
来源：http://ltr.cashguo.top

G. 面向对象
来源：http://zcv.hnxiangtu.top

================================================================================
来源：http://tif.0kj1m.cn

[G01] 定义类
来源：http://twt.xylfe.cn

Py:   class User: pass
来源：http://ylo.uphjek.com

PHP:  class User {}
来源：http://mur.hywenlv.cn

JS:   class User {}
来源：http://ama.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://ezh.vehdjk.com

Java: class User {}
来源：http://ahc.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://tzt.fzhhl.top

Ruby: class User; end
来源：http://qor.cashguo.top

C#:   class User {}
来源：http://dnv.cashguo.top

[G02] 构造函数
来源：http://cyw.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://gtl.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://qtr.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://wtk.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://nxz.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://toh.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kyn.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://niz.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://nvn.ydjk.org.cn

[G03] 实例属性
来源：http://rgh.snrcjt.cn

Py:   self.name = "x"
来源：http://rdx.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://cve.yj202588.top

JS:   this.name = "x";
来源：http://wtn.gogol.net.cn

TS:   name: string = "x";
来源：http://ooy.gaohongyu789.top

Java: private String name;
来源：http://shi.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://apw.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://yek.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://yof.cqqwz.cn

[G04] 定义方法
来源：http://cyy.jianghu66.top

Py:   def greet(self): return self.name
来源：http://afi.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ncz.cheryme.top

JS:   greet() { return this.name; }
来源：http://imd.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://lcb.yj20258.top

Java: String greet() { return name; }
来源：http://blb.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fhq.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://mts.sweek.top

C#:   public string Greet() => Name;
来源：http://mci.jqgfzy.top

[G05] 继承
来源：http://vfe.xylfe.cn

Py:   class Admin(User): pass
来源：http://dah.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://dmn.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://ymw.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://pkh.nanxuanxn.top

Java: class Admin extends User {}
来源：http://eru.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lbk.xuanzx.com

Ruby: class Admin < User; end
来源：http://qbf.jinqigufen.top

C#:   class Admin : User {}
来源：http://fdb.chenlongwang.top

[G06] 重写方法
来源：http://gua.hammf.cn

Py:   def greet(self): return "admin"
来源：http://ucs.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rdu.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://lph.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://mhm.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://pgi.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qbf.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://tcn.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://ipu.ctjpmb.com

[G07] 调用父类方法
来源：http://chz.jyoumei.cn

Py:   super().greet()
来源：http://umh.redwolf501.top

PHP:  parent::greet();
来源：http://jjr.yongpay.top

JS:   super.greet();
来源：http://bay.pycfn.com

TS:   super.greet();
来源：http://drg.jiagoushi.top

Java: super.greet();
来源：http://dhp.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uwn.zhiwuduotai.top

Ruby: super
来源：http://pcc.ctjpmb.com

C#:   base.Greet();
来源：http://pti.yvedp.cn

[G08] 静态方法与属性
来源：http://gkw.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ppd.c1oappe.top

PHP:  public static function f() {}
来源：http://xfe.yuanzhike.top

JS:   static f() {}
来源：http://tmi.mhx1999.top

TS:   static f(): void {}
来源：http://kmz.bbcook.cn

Java: static void f() {}
来源：http://uvz.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bdd.yj20258888.top

Ruby: def self.f; end
来源：http://woj.smart0.xyz

C#:   public static void F() {}
来源：http://uiw.xylfe.cn

[G09] 接口 / 抽象类
来源：http://kcf.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://vgi.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xoe.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vrx.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://wmr.aizwys.cn

Java: interface Shape { double area(); }
来源：http://zep.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://jct.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fwh.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://izl.ivvv.top

[G10] 访问控制
来源：http://yeo.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://gmn.sjlbkw.cn

PHP:  public / protected / private
来源：http://utu.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://dfs.jiagoushi.top

TS:   public / protected / private
来源：http://sla.tarul.cn

Java: public / protected / private / 默认包级
来源：http://zwx.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fni.cqqwz.cn

Ruby: public / protected / private
来源：http://wxr.jianghu66.top

C#:   public / protected / private / internal
来源：http://iej.52xcode.cn

[G11] getter / setter
来源：http://lyx.andypj.xyz

Py:   @property 与 @x.setter
来源：http://rmg.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zsm.cucudq.cn

JS:   get name() { return this._name; }
来源：http://zye.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://zzz.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://hrr.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wun.fzhhl.top

Ruby: attr_accessor :name
来源：http://nal.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://xfu.ctjpmb.com

[G12] 对象转字符串
来源：http://fmf.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://tuj.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xtq.gzhubu.top

JS:   toString() { return this.name; }
来源：http://zwg.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://fps.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://blk.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://wcz.wangdashe.top

Ruby: def to_s; @name; end
来源：http://cck.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://scb.zhijiandao.cn

[G13] 判断对象类型
来源：http://ipe.vehdjk.com

Py:   isinstance(u, User)
来源：http://uoi.hesvh.cn

PHP:  $u instanceof User
来源：http://mjt.shanyushiyangtech.top

JS:   u instanceof User
来源：http://yvw.tarul.cn

TS:   u instanceof User
来源：http://roh.haohaochexian.top

Java: u instanceof User
来源：http://jfh.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tsq.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://sst.wangdashe.top

C#:   u is User
来源：http://ccz.fengsongda.top

[G14] 数据类 / record
来源：http://sqp.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zrc.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://qkk.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cqm.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://amf.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://qdh.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://xmh.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://spe.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://vie.jiagoushi.top

[G15] 枚举
来源：http://ary.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qhf.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hat.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wkv.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eal.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://qad.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ezt.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://sfu.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uvb.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://xdm.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gue.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://rrg.sysykeji.top

JS:   Object.entries(obj)
来源：http://ntx.chenzaomai.com

TS:   Object.entries(obj)
来源：http://pyf.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://obv.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mex.bjfxy.top

Ruby: obj.instance_variables
来源：http://fst.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://pqx.vehdjk.com

================================================================================
来源：http://ltr.nanxuanxn.top

H. 异常与错误处理
来源：http://zfr.epnwcf.com

================================================================================
来源：http://tju.xylfe.cn

[H01] try / catch 基础
来源：http://mzm.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qzz.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqs.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xkj.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://asm.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jeb.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lea.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jpe.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fab.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://apx.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dun.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pux.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sit.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xvg.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://sit.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzz.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://opb.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uao.yongpay.top

[H03] 主动抛出异常
来源：http://lyx.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://jhb.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nqf.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://ciq.pycfn.com

TS:   throw new Error("错误信息");
来源：http://zdc.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kmd.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dev.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://whh.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ked.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://rce.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://itv.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qrd.aizwys.cn

JS:   class MyError extends Error {}
来源：http://abf.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://wfq.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://oot.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jwn.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://awc.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://zzx.hesvh.cn

[H05] 捕获特定类型
来源：http://dpm.0kj1m.cn

Py:   except ValueError as e:
来源：http://vch.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tvs.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://ykw.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://tkb.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://ipp.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jrt.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://rpp.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kvg.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://krs.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://lid.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mre.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zxf.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vli.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ncz.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://rii.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://fcw.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://sjx.jlsjyb.cn


<!-- 参考信息 -->