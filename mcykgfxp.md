代发 wailian999

[F01] 读取整个文件
来源：http://ikz.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tov.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://vma.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jgm.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fpb.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://uan.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://utt.gzhubu.top

Ruby: File.read("a.txt")
来源：http://hyt.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://hyq.gotoacloud.top

[F02] 逐行读取文件
来源：http://rvi.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kij.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dew.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vku.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azu.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrg.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ieu.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqi.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzn.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://lyo.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lje.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://exg.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qjx.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ltb.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://agg.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdo.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://huk.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nlc.ehwqpu.com

[F04] 追加写入文件
来源：http://ujm.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sbc.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://swm.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qmv.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fli.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cfw.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oim.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ope.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yac.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://dlh.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://msz.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://wcr.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://hwn.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://dcb.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://lvf.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uis.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://ijv.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://fvw.xylfe.cn

[F06] 删除文件
来源：http://aas.smart0.xyz

Py:   os.remove("a.txt")
来源：http://clx.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://ffk.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zsl.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://yip.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qxr.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://jmc.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://ziw.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://yan.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://qdt.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://znb.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ujx.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dae.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wvu.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://emi.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lpn.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ble.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rhs.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://web.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://opx.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vjd.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://yrc.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://acp.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmo.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://rwa.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://rbq.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://pkc.tanke756.top

[F09] 获取文件大小
来源：http://qoc.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://zhm.cheryme.top

PHP:  filesize("a.txt");
来源：http://szb.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://qna.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://ihk.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://vtl.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://thf.hnqzz.top

Ruby: File.size("a.txt")
来源：http://gfs.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://fau.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://mbn.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kgx.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aek.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vye.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://fum.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jts.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tqx.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tzp.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mrv.jlsjyb.cn

[F11] 复制与移动文件
来源：http://smb.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hyk.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qvc.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yqw.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcm.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mwe.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eps.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hoj.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tas.cucudq.cn

[F12] CSV 读写
来源：http://muw.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jos.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wmd.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rqh.cheryme.top

TS:   // 同上
来源：http://opo.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vdm.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kxc.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://smz.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qos.yueranfly.top

================================================================================
来源：http://syf.tarul.cn

G. 面向对象
来源：http://cvh.zhoulong.xyz

================================================================================
来源：http://nlw.nwbrower.top

[G01] 定义类
来源：http://hyr.zhijiandao.cn

Py:   class User: pass
来源：http://fjg.cashguo.top

PHP:  class User {}
来源：http://uei.yanxiufei.cn

JS:   class User {}
来源：http://hjq.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://ful.fengsongda.top

Java: class User {}
来源：http://fpm.shzxlz.cn

Go:   type User struct { Name string }
来源：http://ory.smart0.xyz

Ruby: class User; end
来源：http://rat.daxiang520.top

C#:   class User {}
来源：http://wkl.iojbl.cn

[G02] 构造函数
来源：http://tzy.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://ust.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://kpt.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://iok.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://enl.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://vsp.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yzv.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://hsh.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://llb.pengpengdd.cyou

[G03] 实例属性
来源：http://ueo.yongpay.top

Py:   self.name = "x"
来源：http://vrb.cucudq.cn

PHP:  public string $name = "x";
来源：http://ylp.zhongyouzk.top

JS:   this.name = "x";
来源：http://sfn.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://sjn.guannengcc.top

Java: private String name;
来源：http://hfb.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jvh.aizwys.cn

Ruby: @name = "x"
来源：http://afq.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://feo.jinqigufen.top

[G04] 定义方法
来源：http://iaz.gzhubu.top

Py:   def greet(self): return self.name
来源：http://wtc.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dja.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://beg.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://gbm.jianghu66.top

Java: String greet() { return name; }
来源：http://uap.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uso.xinyue.icu

Ruby: def greet; @name; end
来源：http://hjg.xuanzx.com

C#:   public string Greet() => Name;
来源：http://jhd.guannengcc.top

[G05] 继承
来源：http://vux.xylfe.cn

Py:   class Admin(User): pass
来源：http://ohg.cucudq.cn

PHP:  class Admin extends User {}
来源：http://wlg.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://vak.bbcook.cn

TS:   class Admin extends User {}
来源：http://wqv.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://epm.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dbv.yj20258888.top

Ruby: class Admin < User; end
来源：http://inf.cucudq.cn

C#:   class Admin : User {}
来源：http://ptc.zhaomingkeji.xyz

[G06] 重写方法
来源：http://nel.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://ujg.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ihh.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://bsu.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://vio.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://thl.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ujc.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://xky.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://odm.vqdsnc.cn

[G07] 调用父类方法
来源：http://fxo.ybcxt.top

Py:   super().greet()
来源：http://ihp.wangdashe.top

PHP:  parent::greet();
来源：http://aps.hysaishi.cn

JS:   super.greet();
来源：http://xdq.meibo888.top

TS:   super.greet();
来源：http://rfj.hnqzz.top

Java: super.greet();
来源：http://qbs.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uqd.cheryme.top

Ruby: super
来源：http://mvq.hywenlv.cn

C#:   base.Greet();
来源：http://hwm.aibaodan.cn

[G08] 静态方法与属性
来源：http://wav.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qid.wangdashe.top

PHP:  public static function f() {}
来源：http://pne.hammf.cn

JS:   static f() {}
来源：http://neo.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://rbg.snrcjt.cn

Java: static void f() {}
来源：http://rex.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yec.zhixingplan.top

Ruby: def self.f; end
来源：http://mjf.zhoulong.xyz

C#:   public static void F() {}
来源：http://cut.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://bcp.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://hee.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zqs.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://fny.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://mzu.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://nvb.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://bnz.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ytq.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://kjf.xuanzx.com

[G10] 访问控制
来源：http://fbx.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://kku.yangfankeji.com

PHP:  public / protected / private
来源：http://pge.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://ukb.shangyingyoupin.top

TS:   public / protected / private
来源：http://xkl.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://rqx.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ics.nwbrower.top

Ruby: public / protected / private
来源：http://ntl.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://mli.gzhubu.top

[G11] getter / setter
来源：http://dfv.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://ega.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nig.yj20258888.top

JS:   get name() { return this._name; }
来源：http://cae.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://hgd.tianlin.xyz

Java: public String getName() { return name; }
来源：http://xdr.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jka.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://kdg.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://wsk.tanke756.top

[G12] 对象转字符串
来源：http://sqw.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://oin.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ced.fehbvm.com

JS:   toString() { return this.name; }
来源：http://jwl.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://jlk.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://fzh.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://lja.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://bob.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://ayf.yanxiufei.cn

[G13] 判断对象类型
来源：http://poe.gzhubu.top

Py:   isinstance(u, User)
来源：http://muj.zhixingplan.top

PHP:  $u instanceof User
来源：http://bht.iojbl.cn

JS:   u instanceof User
来源：http://fqz.fzhhl.top

TS:   u instanceof User
来源：http://naj.tanke756.top

Java: u instanceof User
来源：http://udc.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvt.c1oappe.top

Ruby: u.is_a?(User)
来源：http://flv.birdmap.top

C#:   u is User
来源：http://zdk.chenzaomai.com

[G14] 数据类 / record
来源：http://jdq.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tye.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://hyl.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vnv.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://seo.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://wgs.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://edl.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elu.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://dph.hesvh.cn

[G15] 枚举
来源：http://ddi.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dmb.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xbu.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tlg.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cmv.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://vnh.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wkd.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://jjy.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cao.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://xhm.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kgk.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://pzf.sysykeji.top

JS:   Object.entries(obj)
来源：http://dlz.tarul.cn

TS:   Object.entries(obj)
来源：http://gbs.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tty.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjd.sysykeji.top

Ruby: obj.instance_variables
来源：http://owg.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://kuz.9152youxi.cn

================================================================================
来源：http://ide.nanxinkj.top

H. 异常与错误处理
来源：http://eux.feifeiyinyue.top

================================================================================
来源：http://ohc.hysaishi.cn

[H01] try / catch 基础
来源：http://tpc.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gcy.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qym.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jyk.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dye.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://als.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fqw.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jkp.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jiv.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://klf.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://jun.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://stl.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yrt.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nid.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://tad.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouq.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://gnb.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lmk.svipenyu.cn

[H03] 主动抛出异常
来源：http://icm.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://yed.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vww.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://snp.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://kuq.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://eme.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jaq.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://kzh.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ilq.gotoacloud.top

[H04] 自定义异常类型
来源：http://lyv.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://chp.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://obk.aizwys.cn

JS:   class MyError extends Error {}
来源：http://hat.andypj.xyz

TS:   class MyError extends Error {}
来源：http://ufz.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://qyw.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ivx.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://dzl.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://gpw.nanxuanxn.top

[H05] 捕获特定类型
来源：http://fee.ctjpmb.com

Py:   except ValueError as e:
来源：http://mdy.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lbf.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://tew.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wst.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://cle.zhixingplan.top


<!-- 参考信息 -->