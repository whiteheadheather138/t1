代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldb.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uvl.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ifq.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://pqt.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vwd.snrcjt.cn

================================================================================
来源：http://ifc.bbcook.cn

F. 文件与目录
来源：http://ofj.nanxinkj.top

================================================================================
来源：http://ztd.yangfankeji.com

[F01] 读取整个文件
来源：http://wyl.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hmc.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://nlg.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aov.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ktq.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://ohk.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bkr.yj20258.top

Ruby: File.read("a.txt")
来源：http://zga.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://syf.gzhubu.top

[F02] 逐行读取文件
来源：http://ohz.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wnz.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jqj.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://czm.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eff.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sne.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://arn.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyt.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vip.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://spl.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jbc.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xmn.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ngz.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okz.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ows.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://amg.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://fht.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rqn.vqdsnc.cn

[F04] 追加写入文件
来源：http://eyp.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://leu.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmq.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzg.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chr.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vjn.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lwb.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hfc.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dsy.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://tfo.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://unc.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://xot.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://lbb.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://ihc.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fyq.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zaz.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://gny.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://ifj.cucudq.cn

[F06] 删除文件
来源：http://bhj.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://cgt.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://kpo.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ucv.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fmn.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://irs.cashguo.top

Go:   os.Remove("a.txt")
来源：http://evk.ivvv.top

Ruby: File.delete("a.txt")
来源：http://wcj.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://jrh.sysykeji.top

[F07] 创建目录（含多级）
来源：http://dfc.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lqd.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eus.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxu.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cpo.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cio.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://chs.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhu.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mtl.fanxiaobao.xyz

[F08] 遍历目录
来源：http://fct.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://byr.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bkt.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://jcj.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://cvv.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpr.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iuc.ybcxt.top

Ruby: Dir.children("dir")
来源：http://uqp.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://lxh.zdbjq.cn

[F09] 获取文件大小
来源：http://itb.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://tzn.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://qja.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://zqh.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://mdq.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://zta.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wnm.havefunace.top

Ruby: File.size("a.txt")
来源：http://mwv.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://ioq.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://qlp.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zep.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gvh.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbk.birdmap.top

TS:   path.extname("a.txt")
来源：http://fxu.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vzk.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gii.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dmv.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uqn.kuanghao11.cn

[F11] 复制与移动文件
来源：http://prs.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kll.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://orb.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eey.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ejm.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xaj.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lwx.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qlb.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pqc.zhongyouzk.top

[F12] CSV 读写
来源：http://akc.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jyt.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://obo.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hlo.gaohongyu789.top

TS:   // 同上
来源：http://rlx.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hqg.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nxo.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://now.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bnx.yj202588.top

================================================================================
来源：http://bzg.yvedp.cn

G. 面向对象
来源：http://txy.shuidangran.top

================================================================================
来源：http://oxz.chenzaomai.com

[G01] 定义类
来源：http://qyq.c1oappe.top

Py:   class User: pass
来源：http://eqz.guowangkeji.top

PHP:  class User {}
来源：http://tqf.nanxuanxn.top

JS:   class User {}
来源：http://stg.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://ukq.shanyushiyangtech.top

Java: class User {}
来源：http://drg.fengsongda.top

Go:   type User struct { Name string }
来源：http://iev.uphjek.com

Ruby: class User; end
来源：http://qej.ctjpmb.com

C#:   class User {}
来源：http://ves.fengsongda.top

[G02] 构造函数
来源：http://qff.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://jta.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://wxn.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://qyq.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://lcr.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://bqr.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://raj.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://uhe.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://ukj.fzhhl.top

[G03] 实例属性
来源：http://gzf.yvedp.cn

Py:   self.name = "x"
来源：http://suk.yj20258888.top

PHP:  public string $name = "x";
来源：http://rxd.epnwcf.com

JS:   this.name = "x";
来源：http://wzb.9152youxi.cn

TS:   name: string = "x";
来源：http://cvj.chenlongwang.top

Java: private String name;
来源：http://gpy.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kgq.bjfxy.top

Ruby: @name = "x"
来源：http://ddf.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://aje.fktsv.cn

[G04] 定义方法
来源：http://lhc.xylfe.cn

Py:   def greet(self): return self.name
来源：http://dtg.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tby.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://gyy.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://gnk.cheryme.top

Java: String greet() { return name; }
来源：http://zvd.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ukv.zycfv.cn

Ruby: def greet; @name; end
来源：http://crq.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://gjo.hywenlv.cn

[G05] 继承
来源：http://pql.snrcjt.cn

Py:   class Admin(User): pass
来源：http://yfr.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://mgi.zdqjudy.top

JS:   class Admin extends User {}
来源：http://wjv.snrcjt.cn

TS:   class Admin extends User {}
来源：http://hzg.guannengcc.top

Java: class Admin extends User {}
来源：http://srg.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rzd.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://cij.zhijiandao.cn

C#:   class Admin : User {}
来源：http://hxo.ydzc1.top

[G06] 重写方法
来源：http://eso.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://tci.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lad.meibo888.top

JS:   greet() { return "admin"; }
来源：http://bjr.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://ids.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://ldz.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qpz.ivvv.top

Ruby: def greet; "admin"; end
来源：http://efg.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://dvz.yongpay.top

[G07] 调用父类方法
来源：http://lko.tian-w.cn

Py:   super().greet()
来源：http://qpq.jlsjyb.cn

PHP:  parent::greet();
来源：http://ldm.svipenyu.cn

JS:   super.greet();
来源：http://idf.birdmap.top

TS:   super.greet();
来源：http://wfm.cucudq.cn

Java: super.greet();
来源：http://pxo.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gju.wangdashe.top

Ruby: super
来源：http://fba.fzhhl.top

C#:   base.Greet();
来源：http://blj.zhijiandao.cn

[G08] 静态方法与属性
来源：http://rkm.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://okg.jiagoushi.top

PHP:  public static function f() {}
来源：http://zgx.yanxiufei.cn

JS:   static f() {}
来源：http://syv.hnqzz.top

TS:   static f(): void {}
来源：http://ucp.iojbl.cn

Java: static void f() {}
来源：http://dcj.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lge.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://vhn.hammf.cn

C#:   public static void F() {}
来源：http://zok.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://dln.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://yph.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rez.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ebr.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://jmn.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://eec.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://ubl.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bda.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://fpz.yj20258.top

[G10] 访问控制
来源：http://ycc.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://txy.mhx1999.top

PHP:  public / protected / private
来源：http://kac.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://mpy.ppjwa.cn

TS:   public / protected / private
来源：http://cvk.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://tsh.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nto.guowangkeji.top

Ruby: public / protected / private
来源：http://osp.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://tll.daxiang520.top

[G11] getter / setter
来源：http://frl.birdmap.top

Py:   @property 与 @x.setter
来源：http://utz.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vti.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://zdx.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://zru.yonumen.top

Java: public String getName() { return name; }
来源：http://kfl.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://aie.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://dtn.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://upt.iojbl.cn

[G12] 对象转字符串
来源：http://kwj.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://mqm.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://hww.xziqi.cn

JS:   toString() { return this.name; }
来源：http://pew.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://jik.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://tmp.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bkm.fehbvm.com

Ruby: def to_s; @name; end
来源：http://tll.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://uit.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://llc.epnwcf.com

Py:   isinstance(u, User)
来源：http://jea.hnqzz.top

PHP:  $u instanceof User
来源：http://zpz.tarul.cn

JS:   u instanceof User
来源：http://sbc.nwbrower.top

TS:   u instanceof User
来源：http://gxm.zdbjq.cn

Java: u instanceof User
来源：http://efg.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://yci.nwbrower.top

Ruby: u.is_a?(User)
来源：http://hzi.shanyushiyangkeji.top

C#:   u is User
来源：http://zxr.ydzc1.top

[G14] 数据类 / record
来源：http://iqz.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ldz.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://tff.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tax.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://twn.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://wrx.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://mqb.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhe.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://zlk.vqdsnc.cn

[G15] 枚举
来源：http://bmq.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ucd.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://whq.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hjz.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bcy.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://hjg.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vwk.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://pbw.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mkz.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://tqf.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dys.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://kei.uphjek.com

JS:   Object.entries(obj)
来源：http://spt.sxryk.cn

TS:   Object.entries(obj)
来源：http://iyu.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qyq.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mzp.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://qjl.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://ujv.yangfankeji.com

================================================================================
来源：http://qwo.9152youxi.cn

H. 异常与错误处理
来源：http://gbj.yj202588.top

================================================================================
来源：http://meo.tanke756.top

[H01] try / catch 基础
来源：http://zeh.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nxs.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hon.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://six.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ley.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xrx.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lek.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bih.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uth.fengsongda.top

[H02] finally / ensure 收尾
来源：http://ynd.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tce.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://gek.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vje.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cpo.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://xpa.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://yrl.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://fhu.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wel.dashuyun.cn

[H03] 主动抛出异常
来源：http://xoa.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://koh.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qnm.pycfn.com

JS:   throw new Error("错误信息");
来源：http://azp.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://mdu.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxy.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dvg.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bol.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vrz.sysykeji.top

[H04] 自定义异常类型
来源：http://nmq.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://ofk.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://fyz.yfazqb.com

JS:   class MyError extends Error {}
来源：http://dcj.yvedp.cn

TS:   class MyError extends Error {}
来源：http://vfg.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://isf.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lck.birdmap.top


<!-- 参考信息 -->