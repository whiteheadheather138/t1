代发 wailian999

[F01] 读取整个文件
来源：http://xbz.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://arm.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://xyl.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gym.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ibt.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vmw.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://spb.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://dwp.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://tjx.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://wph.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ski.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jas.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ujg.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwy.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://feo.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gdk.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uws.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aru.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://sqy.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://asl.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ctb.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eks.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmh.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oob.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dzj.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://kgc.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pao.sweek.top

[F04] 追加写入文件
来源：http://njy.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://crv.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kos.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ykj.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yce.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iif.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qxw.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yyn.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xbt.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://xsx.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qse.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://pyr.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://ykn.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://abd.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://epr.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vyf.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://emr.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://aig.hnxiangtu.top

[F06] 删除文件
来源：http://fzk.gzhubu.top

Py:   os.remove("a.txt")
来源：http://cpx.andypj.xyz

PHP:  unlink("a.txt");
来源：http://eke.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://eje.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jfb.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mam.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://dmt.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://pgb.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://vcj.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://pca.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://onz.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sth.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgw.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zku.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xmn.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mvw.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iiu.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zqy.jinghuilouyu.cn

[F08] 遍历目录
来源：http://nyo.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ssl.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tdt.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://apr.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://qse.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lhr.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qhu.wangdashe.top

Ruby: Dir.children("dir")
来源：http://xpp.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://tqg.xylfe.cn

[F09] 获取文件大小
来源：http://lxu.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://zbi.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://ody.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://tie.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://neb.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uep.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vhd.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://ekw.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://vct.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://jyg.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rra.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tss.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ock.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://fwi.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dxg.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cdw.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ejy.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hoo.sweek.top

[F11] 复制与移动文件
来源：http://mck.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lyg.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mbt.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xxn.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ogp.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ooc.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jle.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gcw.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cuj.jyoumei.cn

[F12] CSV 读写
来源：http://tdj.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlu.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gum.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xky.yj20258888.top

TS:   // 同上
来源：http://otf.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jxr.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qlr.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ugi.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cvh.jinyuanbaomall.cn

================================================================================
来源：http://czu.daxiang520.top

G. 面向对象
来源：http://kes.andypj.xyz

================================================================================
来源：http://efx.hcnkem.com

[G01] 定义类
来源：http://zvz.52xcode.cn

Py:   class User: pass
来源：http://gln.yuanzhike.top

PHP:  class User {}
来源：http://uzj.shanyushiyangtech.top

JS:   class User {}
来源：http://qsr.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://awc.xinyue.icu

Java: class User {}
来源：http://mst.jqgfzy.top

Go:   type User struct { Name string }
来源：http://gav.ppjwa.cn

Ruby: class User; end
来源：http://dfj.ivvv.top

C#:   class User {}
来源：http://pgf.fengsongda.top

[G02] 构造函数
来源：http://eki.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://pux.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://ieu.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://vrl.uphjek.com

TS:   constructor(public name: string) {}
来源：http://wrw.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://eao.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ndo.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://lrn.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://qqg.yj20258.top

[G03] 实例属性
来源：http://cor.vehdjk.com

Py:   self.name = "x"
来源：http://kby.cucudq.cn

PHP:  public string $name = "x";
来源：http://lmg.shuidangran.top

JS:   this.name = "x";
来源：http://rcn.haohaochexian.top

TS:   name: string = "x";
来源：http://hhs.gzhubu.top

Java: private String name;
来源：http://tsg.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jjw.tarul.cn

Ruby: @name = "x"
来源：http://grz.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://gcx.52xcode.cn

[G04] 定义方法
来源：http://vbd.fzhhl.top

Py:   def greet(self): return self.name
来源：http://qam.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jqk.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://yfr.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://rqv.shzxlz.cn

Java: String greet() { return name; }
来源：http://knj.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nya.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://zdk.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://okr.iojbl.cn

[G05] 继承
来源：http://gdk.fzhhl.top

Py:   class Admin(User): pass
来源：http://yxw.cheryme.top

PHP:  class Admin extends User {}
来源：http://txe.wangdashe.top

JS:   class Admin extends User {}
来源：http://qfi.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://wpp.nanxuanxn.top

Java: class Admin extends User {}
来源：http://zsl.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ubh.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://okg.gotoacloud.top

C#:   class Admin : User {}
来源：http://aba.hammf.cn

[G06] 重写方法
来源：http://hdx.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://rnv.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://agl.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://yfh.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://fky.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://jqq.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vxv.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://wrf.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://iuq.mhx1999.top

[G07] 调用父类方法
来源：http://syj.dianchejie.cn

Py:   super().greet()
来源：http://xbl.jianghu66.top

PHP:  parent::greet();
来源：http://awm.redwolf501.top

JS:   super.greet();
来源：http://llc.zhaomingkeji.xyz

TS:   super.greet();
来源：http://hlb.aibaodan.cn

Java: super.greet();
来源：http://pri.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zyx.9152youxi.cn

Ruby: super
来源：http://zce.fengsongda.top

C#:   base.Greet();
来源：http://vwl.hfpthk.cn

[G08] 静态方法与属性
来源：http://gzt.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cge.zhijiandao.cn

PHP:  public static function f() {}
来源：http://lsh.shangyingyoupin.top

JS:   static f() {}
来源：http://qxn.zhiwuduotai.top

TS:   static f(): void {}
来源：http://ied.xinyue.icu

Java: static void f() {}
来源：http://ave.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lhl.yj20258.top

Ruby: def self.f; end
来源：http://qcn.bbcook.cn

C#:   public static void F() {}
来源：http://vxc.pycfn.com

[G09] 接口 / 抽象类
来源：http://mos.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tvs.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rlu.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ont.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://mop.c1oappe.top

Java: interface Shape { double area(); }
来源：http://wua.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://guz.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fyo.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://hdt.dashuyun.cn

[G10] 访问控制
来源：http://xev.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://dcp.nanxuanxn.top

PHP:  public / protected / private
来源：http://gyn.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://aub.9152youxi.cn

TS:   public / protected / private
来源：http://sbz.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://qak.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pae.vehdjk.com

Ruby: public / protected / private
来源：http://ynq.cashguo.top

C#:   public / protected / private / internal
来源：http://hcg.yj202588.top

[G11] getter / setter
来源：http://xeo.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://awg.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rgp.sysykeji.top

JS:   get name() { return this._name; }
来源：http://nge.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://hlp.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://ftx.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pan.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://upm.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://vlr.xuanzx.com

[G12] 对象转字符串
来源：http://tcj.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://hav.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://ubd.epnwcf.com

JS:   toString() { return this.name; }
来源：http://zub.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://xqu.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://dtj.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://ned.fengsongda.top

Ruby: def to_s; @name; end
来源：http://jpm.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://idt.fktsv.cn

[G13] 判断对象类型
来源：http://cao.wangdashe.top

Py:   isinstance(u, User)
来源：http://ydn.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://lju.feifeiyinyue.top

JS:   u instanceof User
来源：http://gkn.zdbjq.cn

TS:   u instanceof User
来源：http://npv.jinyuanbaomall.cn

Java: u instanceof User
来源：http://nen.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://gve.uphjek.com

Ruby: u.is_a?(User)
来源：http://fhs.cheryme.top

C#:   u is User
来源：http://dzh.ehwqpu.com

[G14] 数据类 / record
来源：http://ulg.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hdt.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cgv.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://enk.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://dnb.daria6918.cn

Java: record User(String name, int age) {}
来源：http://zlf.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://pqi.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uca.yj202588.top

C#:   record User(string Name, int Age);
来源：http://qwm.shangyingyoupin.top

[G15] 枚举
来源：http://sjy.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cuu.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://amj.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xwp.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vrq.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://zsh.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fcs.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://szr.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mox.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://xdh.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wqf.yongpay.top

PHP:  get_object_vars($obj);
来源：http://wtc.hysaishi.cn

JS:   Object.entries(obj)
来源：http://mtd.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://sfc.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fbj.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hbl.yj20258.top

Ruby: obj.instance_variables
来源：http://wdh.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://foo.hnqzz.top

================================================================================
来源：http://ahg.iojbl.cn

H. 异常与错误处理
来源：http://szf.hongshengwenyu.top

================================================================================
来源：http://hjy.fzhhl.top

[H01] try / catch 基础
来源：http://kdy.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mav.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://anj.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://crc.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udp.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tvd.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rai.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tkr.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pzz.guannengcc.top

[H02] finally / ensure 收尾
来源：http://hqd.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://gjf.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kmm.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mdz.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tzl.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://lgk.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qkr.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://etg.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mpf.chenzaomai.com

[H03] 主动抛出异常
来源：http://jkn.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://wfc.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fou.meibo888.top

JS:   throw new Error("错误信息");
来源：http://lml.birdmap.top

TS:   throw new Error("错误信息");
来源：http://fou.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hzl.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iwp.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iyu.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cvj.iojbl.cn

[H04] 自定义异常类型
来源：http://uay.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://kup.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://yyv.cheryme.top

JS:   class MyError extends Error {}
来源：http://sgi.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://rdc.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://upy.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://evr.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://req.hcnkem.com

C#:   class MyException : Exception {}
来源：http://nyl.gogol.net.cn

[H05] 捕获特定类型
来源：http://oee.yanxiufei.cn

Py:   except ValueError as e:
来源：http://esh.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lit.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://kyl.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://pyq.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://vpn.zhixingplan.top


<!-- 参考信息 -->