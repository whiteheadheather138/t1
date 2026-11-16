代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://emb.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://rhf.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkh.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wwi.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vgx.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oiy.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wnv.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nrc.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qlf.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rfe.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://pag.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dzz.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yox.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yex.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fds.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dmw.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vam.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://jzt.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwp.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://tgz.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yax.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kmx.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jgv.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alv.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jbh.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hdu.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://reb.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzj.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://knl.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gjv.uphjek.com

PHP:  file_exists("a.txt");
来源：http://jew.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://hjb.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://dtf.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hqr.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cjw.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://vfs.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://fge.cheryme.top

[F06] 删除文件
来源：http://quj.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://pcy.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://lke.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lmn.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://rzb.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xyx.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://vzw.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://vfu.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://fvn.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://lqx.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tap.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hgd.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpv.epnwcf.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iuf.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hor.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kpz.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ikr.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hdo.jiagoushi.top

[F08] 遍历目录
来源：http://hlh.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hhd.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xmw.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://cgq.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://smx.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckl.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rcg.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://kxv.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://cqh.zhengqikj.top

[F09] 获取文件大小
来源：http://ppb.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://abk.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://iez.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://wgp.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://lxf.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://fuj.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nif.cucudq.cn

Ruby: File.size("a.txt")
来源：http://sli.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://nlq.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://ito.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kvy.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hgy.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://amc.hesvh.cn

TS:   path.extname("a.txt")
来源：http://swv.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jfr.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vos.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ffu.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ijx.52xcode.cn

[F11] 复制与移动文件
来源：http://tcq.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aym.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://obo.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csa.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdi.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jkl.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://itt.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cab.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://siw.zhijiandao.cn

[F12] CSV 读写
来源：http://jfa.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lot.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fix.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aqo.hongshengwenyu.top

TS:   // 同上
来源：http://lrk.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pdz.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tai.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sut.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qlb.shuidangran.top

================================================================================
来源：http://xqm.nanxuanxn.top

G. 面向对象
来源：http://zbl.shangyingyoupin.top

================================================================================
来源：http://vzc.fktsv.cn

[G01] 定义类
来源：http://rsf.tarul.cn

Py:   class User: pass
来源：http://czb.zdqjudy.top

PHP:  class User {}
来源：http://fvt.hcnkem.com

JS:   class User {}
来源：http://fcx.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://mre.fktsv.cn

Java: class User {}
来源：http://hil.bjfxy.top

Go:   type User struct { Name string }
来源：http://nyd.tanke756.top

Ruby: class User; end
来源：http://tmk.hnqzz.top

C#:   class User {}
来源：http://jre.chenzaomai.com

[G02] 构造函数
来源：http://xnq.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://mvr.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://cdf.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://knl.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://hpe.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://ftm.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yvq.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://zqe.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://nie.sjlbkw.cn

[G03] 实例属性
来源：http://zhh.daxiang520.top

Py:   self.name = "x"
来源：http://wrj.hfpthk.cn

PHP:  public string $name = "x";
来源：http://bge.chenzaomai.com

JS:   this.name = "x";
来源：http://bbw.zycfv.cn

TS:   name: string = "x";
来源：http://uyq.vqdsnc.cn

Java: private String name;
来源：http://oqx.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lht.fengsongda.top

Ruby: @name = "x"
来源：http://wbi.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://wcs.zhiwuduotai.top

[G04] 定义方法
来源：http://owb.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://vhr.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mbi.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://qdv.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://iiy.jinqigufen.top

Java: String greet() { return name; }
来源：http://guz.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://chr.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://vav.redwolf501.top

C#:   public string Greet() => Name;
来源：http://xli.yfazqb.com

[G05] 继承
来源：http://bgl.ivvv.top

Py:   class Admin(User): pass
来源：http://yae.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://cmm.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://mnd.aibaodan.cn

TS:   class Admin extends User {}
来源：http://hic.hesvh.cn

Java: class Admin extends User {}
来源：http://nmz.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rds.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://olm.pycfn.com

C#:   class Admin : User {}
来源：http://sxk.yj20258888.top

[G06] 重写方法
来源：http://blj.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://nnl.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ono.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://jsg.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://wpr.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://kxo.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rzu.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://iku.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://sgl.cucudq.cn

[G07] 调用父类方法
来源：http://okw.shzxlz.cn

Py:   super().greet()
来源：http://psy.zhijiandao.cn

PHP:  parent::greet();
来源：http://ilo.tianlin.xyz

JS:   super.greet();
来源：http://nha.yuanzhike.top

TS:   super.greet();
来源：http://ibb.shuidangran.top

Java: super.greet();
来源：http://xeh.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wvk.yvedp.cn

Ruby: super
来源：http://chk.quarkkingdee.top

C#:   base.Greet();
来源：http://asa.tian-w.cn

[G08] 静态方法与属性
来源：http://xdj.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lnp.tarul.cn

PHP:  public static function f() {}
来源：http://htp.ehwqpu.com

JS:   static f() {}
来源：http://xwx.xinyue.icu

TS:   static f(): void {}
来源：http://lfc.yj202588.top

Java: static void f() {}
来源：http://ifd.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://nlk.fktsv.cn

Ruby: def self.f; end
来源：http://kas.haohaochexian.top

C#:   public static void F() {}
来源：http://yae.nwbrower.top

[G09] 接口 / 抽象类
来源：http://lcn.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://nas.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://kvh.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tjv.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://qch.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://ecy.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://mmv.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vwr.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://lyg.ydzc1.top

[G10] 访问控制
来源：http://sup.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://ors.shangyingyoupin.top

PHP:  public / protected / private
来源：http://cag.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://czq.redwolf501.top

TS:   public / protected / private
来源：http://xfm.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://vgh.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ops.uphjek.com

Ruby: public / protected / private
来源：http://ozc.svipenyu.cn

C#:   public / protected / private / internal
来源：http://fhj.feifeiyinyue.top

[G11] getter / setter
来源：http://uca.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://nyx.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kys.sysykeji.top

JS:   get name() { return this._name; }
来源：http://rme.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://fil.zdbjq.cn

Java: public String getName() { return name; }
来源：http://tab.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wvi.yj20258.top

Ruby: attr_accessor :name
来源：http://ovc.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://dlt.cdnleiting.top

[G12] 对象转字符串
来源：http://oeo.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://kau.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lxf.yonumen.top

JS:   toString() { return this.name; }
来源：http://sko.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://suo.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://wzf.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lab.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://kmd.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://ags.ybcxt.top

[G13] 判断对象类型
来源：http://hps.ctjpmb.com

Py:   isinstance(u, User)
来源：http://wsv.sweek.top

PHP:  $u instanceof User
来源：http://npj.fzhhl.top

JS:   u instanceof User
来源：http://jtr.cqqwz.cn

TS:   u instanceof User
来源：http://pyo.ybcxt.top

Java: u instanceof User
来源：http://vng.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bao.fehbvm.com

Ruby: u.is_a?(User)
来源：http://qlu.chenzaomai.com

C#:   u is User
来源：http://bcn.hfpthk.cn

[G14] 数据类 / record
来源：http://ymr.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gwj.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://jbz.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://nlu.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://feu.yj202588.top

Java: record User(String name, int age) {}
来源：http://gvl.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://ihq.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zzq.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://kvk.sxryk.cn

[G15] 枚举
来源：http://ffg.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gkt.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lix.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gii.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zmd.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://uwg.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://amt.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://ktd.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyq.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://ywr.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zwy.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://jwu.xziqi.cn

JS:   Object.entries(obj)
来源：http://jns.wangdashe.top

TS:   Object.entries(obj)
来源：http://kbh.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pfa.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://edg.zdqjudy.top

Ruby: obj.instance_variables
来源：http://xwv.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://mou.0kj1m.cn

================================================================================
来源：http://wur.gotoacloud.top

H. 异常与错误处理
来源：http://nzh.guannengcc.top

================================================================================
来源：http://iqp.52xcode.cn

[H01] try / catch 基础
来源：http://bgw.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rvw.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vaf.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://amh.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wdd.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fqu.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sxd.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xit.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://com.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://zza.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://jzu.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kar.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wjh.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pxk.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://ryj.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lwq.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ayv.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iqx.hcnkem.com

[H03] 主动抛出异常
来源：http://xfp.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://xjp.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oeh.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://ggi.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://gkz.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qvg.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tke.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dcf.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://ctg.havefunace.top

[H04] 自定义异常类型
来源：http://jmn.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://lyf.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oga.sysykeji.top

JS:   class MyError extends Error {}
来源：http://ysx.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://hjs.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://ybx.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gmb.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://nhh.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://oil.havefunace.top

[H05] 捕获特定类型
来源：http://nff.zhixingplan.top

Py:   except ValueError as e:
来源：http://xfw.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsg.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://ilw.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://jnz.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://mxn.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mpv.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://avk.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://red.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://mna.birdmap.top

Py:   value = d.get("k") or default
来源：http://tfq.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://sqg.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://hgv.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mna.yuxming.cn


<!-- 参考信息 -->