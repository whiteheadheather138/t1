代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://atu.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xmq.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ula.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://gjd.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://fds.ivvv.top

[F02] 逐行读取文件
来源：http://ixw.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ffq.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gti.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dos.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jap.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://evj.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cun.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tvt.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iof.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://rub.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngd.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vsy.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xen.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozq.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nhh.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nov.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://xsy.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lua.ivvv.top

[F04] 追加写入文件
来源：http://sci.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fve.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gkn.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lyk.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pij.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wav.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fya.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrx.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rax.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://lah.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jfs.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://axp.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://etm.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://wyc.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kxc.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aqp.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://mia.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://qdh.guowangkeji.top

[F06] 删除文件
来源：http://zcb.yfazqb.com

Py:   os.remove("a.txt")
来源：http://ybp.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://svv.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://hmc.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lyn.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gft.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://udr.cheryme.top

Ruby: File.delete("a.txt")
来源：http://vfz.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://yoq.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://qbe.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dal.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xmz.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hnd.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xik.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ikt.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yja.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hvv.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xwf.yvedp.cn

[F08] 遍历目录
来源：http://jyy.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mpo.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tdv.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://rli.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://sgy.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pkc.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ivf.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://otr.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://vho.gogol.net.cn

[F09] 获取文件大小
来源：http://flj.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://lwc.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://zzd.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://jcz.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://zhw.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://cto.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pzb.zycfv.cn

Ruby: File.size("a.txt")
来源：http://jmy.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://xsy.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://mzd.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://czb.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yzw.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eti.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://fcq.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bdo.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mru.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mbt.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hyz.mhx1999.top

[F11] 复制与移动文件
来源：http://mew.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ekb.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zhz.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpj.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osr.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uhr.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zlc.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blr.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://avo.tian-w.cn

[F12] CSV 读写
来源：http://gim.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tmm.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rms.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tyy.zhiwuduotai.top

TS:   // 同上
来源：http://lmo.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bdv.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://juy.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ggr.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qjc.jinqigufen.top

================================================================================
来源：http://iva.ehwqpu.com

G. 面向对象
来源：http://ysk.dianchejie.cn

================================================================================
来源：http://hcr.sufxvd.cn

[G01] 定义类
来源：http://crk.yanxiufei.cn

Py:   class User: pass
来源：http://xfv.yueranfly.top

PHP:  class User {}
来源：http://gev.nwbrower.top

JS:   class User {}
来源：http://jvn.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://thx.c1oappe.top

Java: class User {}
来源：http://phl.yongpay.top

Go:   type User struct { Name string }
来源：http://wik.iojbl.cn

Ruby: class User; end
来源：http://gij.fengsongda.top

C#:   class User {}
来源：http://qzt.hammf.cn

[G02] 构造函数
来源：http://rwa.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://vxf.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://bak.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://zee.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://qha.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://edx.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://csa.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://kag.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://the.gaohongyu789.top

[G03] 实例属性
来源：http://vwa.fehbvm.com

Py:   self.name = "x"
来源：http://vwb.jianghu66.top

PHP:  public string $name = "x";
来源：http://qbl.daxiang520.top

JS:   this.name = "x";
来源：http://kyt.hammf.cn

TS:   name: string = "x";
来源：http://lyv.hywenlv.cn

Java: private String name;
来源：http://esh.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hye.wangdashe.top

Ruby: @name = "x"
来源：http://acq.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://jdv.epnwcf.com

[G04] 定义方法
来源：http://yyl.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://yuk.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://zdi.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://mpz.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://iii.0kj1m.cn

Java: String greet() { return name; }
来源：http://qhy.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oso.daxiang520.top

Ruby: def greet; @name; end
来源：http://kxq.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://xrl.yonumen.top

[G05] 继承
来源：http://jpm.ehwqpu.com

Py:   class Admin(User): pass
来源：http://sjx.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://qvc.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://qxj.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://vtl.guannengcc.top

Java: class Admin extends User {}
来源：http://ttz.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lkf.jiagoushi.top

Ruby: class Admin < User; end
来源：http://owj.zhijiandao.cn

C#:   class Admin : User {}
来源：http://tvs.hysaishi.cn

[G06] 重写方法
来源：http://iju.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://tto.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vco.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://idj.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://gge.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://oxv.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rli.cheryme.top

Ruby: def greet; "admin"; end
来源：http://dgd.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://tmv.bjfxy.top

[G07] 调用父类方法
来源：http://rhu.hammf.cn

Py:   super().greet()
来源：http://bpv.tianlin.xyz

PHP:  parent::greet();
来源：http://age.yanxiufei.cn

JS:   super.greet();
来源：http://jci.sufxvd.cn

TS:   super.greet();
来源：http://qhg.dashuyun.cn

Java: super.greet();
来源：http://yim.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ihv.xuanzx.com

Ruby: super
来源：http://rvs.hywenlv.cn

C#:   base.Greet();
来源：http://wqq.cdnleiting.top

[G08] 静态方法与属性
来源：http://gds.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://woe.yj20258888.top

PHP:  public static function f() {}
来源：http://prc.mhx1999.top

JS:   static f() {}
来源：http://hft.sysykeji.top

TS:   static f(): void {}
来源：http://bbv.hongshengwenyu.top

Java: static void f() {}
来源：http://bsy.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gdj.epnwcf.com

Ruby: def self.f; end
来源：http://cjt.shuidangran.top

C#:   public static void F() {}
来源：http://apo.sxryk.cn

[G09] 接口 / 抽象类
来源：http://drd.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://xgm.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://hel.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://njk.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://imf.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://fuo.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://ncr.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pwj.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://kcy.ehwqpu.com

[G10] 访问控制
来源：http://wro.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://lud.jqgfzy.top

PHP:  public / protected / private
来源：http://esj.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://ttz.zdbjq.cn

TS:   public / protected / private
来源：http://dwk.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://fws.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iis.pycfn.com

Ruby: public / protected / private
来源：http://uhk.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://lzg.gogol.net.cn

[G11] getter / setter
来源：http://ybl.bjfxy.top

Py:   @property 与 @x.setter
来源：http://qin.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xjr.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://unl.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://gwa.wangdashe.top

Java: public String getName() { return name; }
来源：http://knn.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uza.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://ier.bjfxy.top

C#:   public string Name { get; set; }
来源：http://aqz.ppjwa.cn

[G12] 对象转字符串
来源：http://urk.havefunace.top

Py:   def __str__(self): return self.name
来源：http://nas.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xpj.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://zel.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://bvz.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://qot.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://dws.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://qvh.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://weu.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://msm.xinyue.icu

Py:   isinstance(u, User)
来源：http://exn.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://ztk.ctjpmb.com

JS:   u instanceof User
来源：http://pat.ctjpmb.com

TS:   u instanceof User
来源：http://oii.fktsv.cn

Java: u instanceof User
来源：http://pur.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ymn.bjfxy.top

Ruby: u.is_a?(User)
来源：http://tzu.yfazqb.com

C#:   u is User
来源：http://ife.sysykeji.top

[G14] 数据类 / record
来源：http://arw.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cac.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://lzl.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://oll.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://oas.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://rgd.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://ndq.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btg.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://enh.zdqjudy.top

[G15] 枚举
来源：http://ckx.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://isl.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://itj.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bdm.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://efd.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://gja.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vyg.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://kxu.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nts.ivvv.top

[G16] 对象转数组 / 字典
来源：http://gea.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wyr.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://eac.jianghu66.top

JS:   Object.entries(obj)
来源：http://hld.sysykeji.top

TS:   Object.entries(obj)
来源：http://hko.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wnu.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fgu.cheryme.top

Ruby: obj.instance_variables
来源：http://qkd.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://boq.fengsongda.top

================================================================================
来源：http://uns.zdqjudy.top

H. 异常与错误处理
来源：http://src.aibaodan.cn

================================================================================
来源：http://amm.ydzc1.top

[H01] try / catch 基础
来源：http://cek.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrt.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ywf.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aiv.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oov.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rvn.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dqm.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mix.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://htf.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://osf.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://qsf.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ulw.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xwm.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bid.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ood.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qzg.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hoj.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bal.cheryme.top

[H03] 主动抛出异常
来源：http://qqk.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://hdc.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ndn.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://axg.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://gvw.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rjp.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ftz.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aye.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pyk.fehbvm.com

[H04] 自定义异常类型
来源：http://xyp.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://rkr.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://idx.fzhhl.top

JS:   class MyError extends Error {}
来源：http://kcy.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://vlz.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://rwg.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://csd.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://ekx.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://gqu.zhoulong.xyz

[H05] 捕获特定类型
来源：http://nba.fktsv.cn

Py:   except ValueError as e:
来源：http://rvg.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vst.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://vld.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://itp.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://dcj.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mlm.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://hix.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lte.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://wzf.nwbrower.top


<!-- 参考信息 -->