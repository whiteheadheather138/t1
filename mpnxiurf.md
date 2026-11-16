代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://esq.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcw.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kfy.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xrh.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xda.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sjz.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://cem.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qvw.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vrb.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ucy.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iuz.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yne.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yhd.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://bcy.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mmv.sufxvd.cn

[F04] 追加写入文件
来源：http://noc.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nhc.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://myb.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wyf.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vup.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xfb.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hbc.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hhe.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://epz.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://yvj.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jwl.tanke756.top

PHP:  file_exists("a.txt");
来源：http://tnz.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://cqd.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://cll.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iss.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xtg.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://tzl.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://cjq.zhijiandao.cn

[F06] 删除文件
来源：http://gql.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://bik.birdmap.top

PHP:  unlink("a.txt");
来源：http://plo.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://qtj.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://xdn.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://use.yongpay.top

Go:   os.Remove("a.txt")
来源：http://aet.birdmap.top

Ruby: File.delete("a.txt")
来源：http://uwb.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://xbv.sysykeji.top

[F07] 创建目录（含多级）
来源：http://sbh.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpy.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svj.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mxy.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yey.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rse.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cma.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxq.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pzk.cdnleiting.top

[F08] 遍历目录
来源：http://zwu.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vjr.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zbd.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://bvv.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://anv.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://els.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ffo.nwbrower.top

Ruby: Dir.children("dir")
来源：http://lzc.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://nkb.tianlin.xyz

[F09] 获取文件大小
来源：http://mao.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://lqb.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://fsc.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://ouz.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://gbk.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ezz.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ddd.guannengcc.top

Ruby: File.size("a.txt")
来源：http://aww.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://dtz.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://rgf.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://adj.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xuq.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://slk.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://kbc.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qbl.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pgh.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://etd.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ere.jianghu66.top

[F11] 复制与移动文件
来源：http://blu.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://env.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cmw.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixn.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyy.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sll.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cjc.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vla.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://poj.ydjk.org.cn

[F12] CSV 读写
来源：http://bol.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pzq.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lxx.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fvw.havefunace.top

TS:   // 同上
来源：http://hdk.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yvq.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ssw.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uzk.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jue.jqgufenzy.top

================================================================================
来源：http://jwy.zhengqikj.top

G. 面向对象
来源：http://rpj.sufxvd.cn

================================================================================
来源：http://dql.jiagoushi.top

[G01] 定义类
来源：http://hzl.zdqjudy.top

Py:   class User: pass
来源：http://ehn.jiagoushi.top

PHP:  class User {}
来源：http://dwj.pengpengdd.cyou

JS:   class User {}
来源：http://kuc.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://nbp.jqgfzy.top

Java: class User {}
来源：http://bqj.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://ztr.uphjek.com

Ruby: class User; end
来源：http://hoa.gogol.net.cn

C#:   class User {}
来源：http://cyl.sysykeji.top

[G02] 构造函数
来源：http://xse.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://txx.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://eku.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://tem.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://wao.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://jhw.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jsl.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://grf.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://vjl.ppjwa.cn

[G03] 实例属性
来源：http://cbi.yfazqb.com

Py:   self.name = "x"
来源：http://cqp.cucudq.cn

PHP:  public string $name = "x";
来源：http://xuo.jinqigfzy.top

JS:   this.name = "x";
来源：http://sho.jinqigufen.top

TS:   name: string = "x";
来源：http://iao.nanxinkj.top

Java: private String name;
来源：http://buh.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yvu.zdbjq.cn

Ruby: @name = "x"
来源：http://fvi.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xpf.tanke756.top

[G04] 定义方法
来源：http://rdt.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://bee.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://edj.xziqi.cn

JS:   greet() { return this.name; }
来源：http://pee.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://emn.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://ndg.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wom.hysaishi.cn

Ruby: def greet; @name; end
来源：http://ybq.316326.xyz

C#:   public string Greet() => Name;
来源：http://afe.yuanzhike.top

[G05] 继承
来源：http://bwy.0kj1m.cn

Py:   class Admin(User): pass
来源：http://jcg.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://sod.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://bag.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://lri.yvedp.cn

Java: class Admin extends User {}
来源：http://qhp.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hyj.pycfn.com

Ruby: class Admin < User; end
来源：http://usj.guowangkeji.top

C#:   class Admin : User {}
来源：http://eiq.jlsjyb.cn

[G06] 重写方法
来源：http://bis.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://yog.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mgz.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://alu.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://mmk.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://pyi.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rga.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://ixc.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://bmi.ppjwa.cn

[G07] 调用父类方法
来源：http://ogo.yuanzhike.top

Py:   super().greet()
来源：http://pyw.9152youxi.cn

PHP:  parent::greet();
来源：http://ukm.haohaochexian.top

JS:   super.greet();
来源：http://mwz.hesvh.cn

TS:   super.greet();
来源：http://qfy.bjfxy.top

Java: super.greet();
来源：http://nyh.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hdg.iojbl.cn

Ruby: super
来源：http://bws.chenjidiqi.icu

C#:   base.Greet();
来源：http://wqh.tarul.cn

[G08] 静态方法与属性
来源：http://zey.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xui.mhx1999.top

PHP:  public static function f() {}
来源：http://zxi.52xcode.cn

JS:   static f() {}
来源：http://nzm.jlsjyb.cn

TS:   static f(): void {}
来源：http://ewd.aibaodan.cn

Java: static void f() {}
来源：http://jpm.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://noz.jlsjyb.cn

Ruby: def self.f; end
来源：http://ran.svipenyu.cn

C#:   public static void F() {}
来源：http://lzq.sxryk.cn

[G09] 接口 / 抽象类
来源：http://azz.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://hnn.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uxd.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dnb.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://ucf.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://xvb.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://jjo.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbq.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://ada.xziqi.cn

[G10] 访问控制
来源：http://ycs.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ymr.dashuyun.cn

PHP:  public / protected / private
来源：http://vjb.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://bga.nanxinkj.top

TS:   public / protected / private
来源：http://bsx.meibo888.top

Java: public / protected / private / 默认包级
来源：http://thy.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mma.fktsv.cn

Ruby: public / protected / private
来源：http://fjs.52xcode.cn

C#:   public / protected / private / internal
来源：http://bbc.cheryme.top

[G11] getter / setter
来源：http://dwf.gzhubu.top

Py:   @property 与 @x.setter
来源：http://bsc.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oig.c1oappe.top

JS:   get name() { return this._name; }
来源：http://ahu.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://shj.316326.xyz

Java: public String getName() { return name; }
来源：http://xie.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ndc.sxryk.cn

Ruby: attr_accessor :name
来源：http://aax.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://aap.316326.xyz

[G12] 对象转字符串
来源：http://unw.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://wtc.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hyy.xziqi.cn

JS:   toString() { return this.name; }
来源：http://cfk.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://fpy.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://mjl.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tvc.meibo888.top

Ruby: def to_s; @name; end
来源：http://jqf.ivvv.top

C#:   public override string ToString() => Name;
来源：http://dyq.redwolf501.top

[G13] 判断对象类型
来源：http://knr.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://vrt.ydzc1.top

PHP:  $u instanceof User
来源：http://xwv.cheryme.top

JS:   u instanceof User
来源：http://rzm.tarul.cn

TS:   u instanceof User
来源：http://zib.zhijiandao.cn

Java: u instanceof User
来源：http://tbt.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jnw.cashguo.top

Ruby: u.is_a?(User)
来源：http://foj.zdbjq.cn

C#:   u is User
来源：http://aur.yvedp.cn

[G14] 数据类 / record
来源：http://hzs.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tne.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://bpj.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sjm.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://czv.yfazqb.com

Java: record User(String name, int age) {}
来源：http://uzn.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://bcb.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zsp.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://xab.sjlbkw.cn

[G15] 枚举
来源：http://uxb.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sbc.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zhn.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mmf.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odv.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://tlr.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hsy.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://kak.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://riw.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://cfd.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zyb.ivvv.top

PHP:  get_object_vars($obj);
来源：http://zwz.jyoumei.cn

JS:   Object.entries(obj)
来源：http://ble.yj20258.top

TS:   Object.entries(obj)
来源：http://ezo.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fna.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ujh.svipenyu.cn

Ruby: obj.instance_variables
来源：http://mal.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://gsh.wangshuangyany.cn

================================================================================
来源：http://zgg.wangdashe.top

H. 异常与错误处理
来源：http://bkv.feifeiyinyue.top

================================================================================
来源：http://jri.ivvv.top

[H01] try / catch 基础
来源：http://cto.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jlc.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lhd.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ixy.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ldq.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yay.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qxx.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tos.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gzh.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://qzc.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ffs.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://brq.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cez.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qmh.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://ohy.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mrz.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mfp.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://voz.cashguo.top

[H03] 主动抛出异常
来源：http://awl.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://wcj.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgs.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://pao.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://rqf.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://czh.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ikr.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sxk.zhaomingkeji.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zev.svipenyu.cn

[H04] 自定义异常类型
来源：http://inn.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://qus.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hff.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://ceq.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://win.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://zao.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pdp.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://nzd.yuxming.cn

C#:   class MyException : Exception {}
来源：http://qmd.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://dkd.sufxvd.cn

Py:   except ValueError as e:
来源：http://mbn.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jyc.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://xiy.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://adq.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://sbn.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wzh.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://xbp.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rfu.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://ege.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://nnb.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wdl.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iiy.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yed.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cax.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bub.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://yfv.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://otk.guannengcc.top


<!-- 参考信息 -->