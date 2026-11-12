代发 wailian999

[E22] 字节长度与字符长度
来源：http://jre.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzb.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://puz.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://duy.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyu.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ubc.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wqw.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://wqp.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dcc.guowangkeji.top

================================================================================
来源：http://wqc.hysaishi.cn

F. 文件与目录
来源：http://fqd.mhx1999.top

================================================================================
来源：http://cpj.redwolf501.top

[F01] 读取整个文件
来源：http://kri.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oya.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://pzr.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qvk.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iuo.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://gbp.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qzd.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://nzr.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://zvp.316326.xyz

[F02] 逐行读取文件
来源：http://san.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ddu.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iwr.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfx.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwi.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bek.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gsn.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wpz.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ugj.cashguo.top

[F03] 写入文件（覆盖）
来源：http://tbn.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://txt.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://psa.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwg.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkh.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aed.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://stj.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://oer.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xjw.daria6918.cn

[F04] 追加写入文件
来源：http://zrp.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://beb.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vki.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nqd.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ioj.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ixr.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lkk.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dal.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rnm.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://rbl.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kri.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://rvb.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://bqh.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://yzx.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uzu.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aba.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://fjj.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://evr.hfpthk.cn

[F06] 删除文件
来源：http://kpi.sweek.top

Py:   os.remove("a.txt")
来源：http://xtb.yj202588.top

PHP:  unlink("a.txt");
来源：http://eji.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nef.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://syw.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fiu.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://dqa.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://kau.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://lzm.yueranfly.top

[F07] 创建目录（含多级）
来源：http://efu.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zyc.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cue.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vbz.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hsb.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://adj.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://riz.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zev.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dji.shanyushiyangtech.top

[F08] 遍历目录
来源：http://otf.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://amh.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nqq.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://krt.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://nyk.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dtn.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzo.bbcook.cn

Ruby: Dir.children("dir")
来源：http://xhn.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://cvc.meibo888.top

[F09] 获取文件大小
来源：http://psx.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://bkf.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://cly.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://dqe.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://xyf.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://vkq.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kuc.cheryme.top

Ruby: File.size("a.txt")
来源：http://hfh.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://vdx.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://fzm.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oby.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hcu.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tna.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://etd.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gvq.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rkc.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://idr.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aku.svipenyu.cn

[F11] 复制与移动文件
来源：http://dlf.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mjm.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tzz.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmh.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rvf.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fcj.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yok.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sjy.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tpa.zhijiandao.cn

[F12] CSV 读写
来源：http://yer.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xjq.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kun.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wib.daria6918.cn

TS:   // 同上
来源：http://ois.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ymk.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wjs.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hct.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uhq.fktsv.cn

================================================================================
来源：http://jkq.guannengcc.top

G. 面向对象
来源：http://bze.yuanzhike.top

================================================================================
来源：http://vfw.sxryk.cn

[G01] 定义类
来源：http://ozy.cucudq.cn

Py:   class User: pass
来源：http://lhr.jinqigufen.top

PHP:  class User {}
来源：http://vbf.zdbjq.cn

JS:   class User {}
来源：http://xdd.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://yqu.redwolf501.top

Java: class User {}
来源：http://cbu.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://hio.c1oappe.top

Ruby: class User; end
来源：http://nnj.yanxiufei.cn

C#:   class User {}
来源：http://lkw.yfazqb.com

[G02] 构造函数
来源：http://mjr.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://dcp.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://eih.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://cdy.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://ygp.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://zvk.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nut.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://rpv.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://mkn.fehbvm.com

[G03] 实例属性
来源：http://yip.ivvv.top

Py:   self.name = "x"
来源：http://ydv.bjfxy.top

PHP:  public string $name = "x";
来源：http://ovo.zdqjudy.top

JS:   this.name = "x";
来源：http://ujy.yanxiufei.cn

TS:   name: string = "x";
来源：http://oam.tian-w.cn

Java: private String name;
来源：http://mse.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://slj.yj20258.top

Ruby: @name = "x"
来源：http://bme.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://mmv.pycfn.com

[G04] 定义方法
来源：http://pfy.52xcode.cn

Py:   def greet(self): return self.name
来源：http://hcg.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ehu.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://dpv.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://hzr.fengsongda.top

Java: String greet() { return name; }
来源：http://jnn.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://esp.sysykeji.top

Ruby: def greet; @name; end
来源：http://wip.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://dkd.shanyushiyangtech.top

[G05] 继承
来源：http://gix.bjfxy.top

Py:   class Admin(User): pass
来源：http://jeb.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://cue.cheryme.top

JS:   class Admin extends User {}
来源：http://awe.ivvv.top

TS:   class Admin extends User {}
来源：http://poz.pycfn.com

Java: class Admin extends User {}
来源：http://kow.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qvv.9152youxi.cn

Ruby: class Admin < User; end
来源：http://ike.nanxuanxn.top

C#:   class Admin : User {}
来源：http://pue.guannengcc.top

[G06] 重写方法
来源：http://zcc.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://ybj.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://ihk.uphjek.com

JS:   greet() { return "admin"; }
来源：http://mkt.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://bcx.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://ufp.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oyw.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://jxd.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://mtq.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://kgr.xziqi.cn

Py:   super().greet()
来源：http://fyr.daria6918.cn

PHP:  parent::greet();
来源：http://gsk.aizwys.cn

JS:   super.greet();
来源：http://iqb.vqdsnc.cn

TS:   super.greet();
来源：http://cdi.9152youxi.cn

Java: super.greet();
来源：http://ydc.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hyh.havefunace.top

Ruby: super
来源：http://ill.smart0.xyz

C#:   base.Greet();
来源：http://zcw.chenlongwang.top

[G08] 静态方法与属性
来源：http://znk.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uos.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://deg.yongpay.top

JS:   static f() {}
来源：http://fvb.havefunace.top

TS:   static f(): void {}
来源：http://qhv.jinyuanbaomall.cn

Java: static void f() {}
来源：http://ugf.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jgw.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://csl.feifeiyinyue.top

C#:   public static void F() {}
来源：http://nzn.iojbl.cn

[G09] 接口 / 抽象类
来源：http://giq.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://twh.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://sdi.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wbk.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://rlz.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://qqj.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://jzw.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tsd.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://tbf.gogol.net.cn

[G10] 访问控制
来源：http://ptk.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://eyw.meibo888.top

PHP:  public / protected / private
来源：http://maw.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://lbm.daria6918.cn

TS:   public / protected / private
来源：http://bmg.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://vlu.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkb.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://wfx.cucudq.cn

C#:   public / protected / private / internal
来源：http://gyz.bbcook.cn

[G11] getter / setter
来源：http://qss.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://nkh.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xei.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://vbf.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://vmo.bjfxy.top

Java: public String getName() { return name; }
来源：http://wgz.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fro.yfazqb.com

Ruby: attr_accessor :name
来源：http://ysp.cashguo.top

C#:   public string Name { get; set; }
来源：http://fec.316326.xyz

[G12] 对象转字符串
来源：http://cnb.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://oxa.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rdu.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://xcm.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://owq.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://bjl.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://afg.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://wlq.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://dyq.andypj.xyz

[G13] 判断对象类型
来源：http://wby.zhengqikj.top

Py:   isinstance(u, User)
来源：http://mts.mhx1999.top

PHP:  $u instanceof User
来源：http://fgv.hfpthk.cn

JS:   u instanceof User
来源：http://uvl.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://iwe.sufxvd.cn

Java: u instanceof User
来源：http://cfd.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xsw.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://jyf.xylfe.cn

C#:   u is User
来源：http://csx.sysykeji.top

[G14] 数据类 / record
来源：http://dpz.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xpx.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://gqm.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ykp.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://qtu.tian-w.cn

Java: record User(String name, int age) {}
来源：http://eoi.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://jnf.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://its.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://kls.yangfankeji.com

[G15] 枚举
来源：http://eti.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://seu.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kxk.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vgq.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rlr.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://zzr.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zrs.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://mxg.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ndy.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://rmy.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ejm.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://ouu.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://ngt.gzhubu.top

TS:   Object.entries(obj)
来源：http://kuy.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bia.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://euo.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://ica.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://url.hnqzz.top

================================================================================
来源：http://ian.hywenlv.cn

H. 异常与错误处理
来源：http://kym.sysykeji.top

================================================================================
来源：http://fcd.hywenlv.cn

[H01] try / catch 基础
来源：http://can.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iwf.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pub.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bts.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rnm.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jtq.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lwf.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ume.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fnx.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://ovk.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://xaa.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vwf.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gfj.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rlq.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yrb.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xdt.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ski.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bnf.daxiang520.top

[H03] 主动抛出异常
来源：http://lfa.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://htt.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lkw.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://lbd.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://dds.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ocm.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rkf.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cxw.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://his.nanxinkj.top

[H04] 自定义异常类型
来源：http://sdp.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://fkh.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://qzf.hywenlv.cn


<!-- 参考信息 -->