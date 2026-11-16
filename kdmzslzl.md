代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pzi.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wsq.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ere.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://fkm.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qln.52xcode.cn

================================================================================
来源：http://eym.chenjidiqi.icu

F. 文件与目录
来源：http://lpd.316326.xyz

================================================================================
来源：http://lhr.316326.xyz

[F01] 读取整个文件
来源：http://dvm.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pyr.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://dnx.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://orb.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xhq.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jxi.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gld.gzhubu.top

Ruby: File.read("a.txt")
来源：http://msj.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://uic.pycfn.com

[F02] 逐行读取文件
来源：http://dfo.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://koq.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dib.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evk.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvj.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wlg.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zlf.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jzu.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bst.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://arq.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kuf.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rwe.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fzl.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrl.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dee.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ynl.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://lgt.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zwi.gotoacloud.top

[F04] 追加写入文件
来源：http://qkj.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ubp.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vuw.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cih.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://plg.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cfb.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gmz.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kvw.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vvj.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://xnk.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjj.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://ooa.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://lao.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://wyl.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nen.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etv.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://erw.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://mxu.fanxiaobao.xyz

[F06] 删除文件
来源：http://ekz.daria6918.cn

Py:   os.remove("a.txt")
来源：http://fsp.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://hts.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://saj.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://enp.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsa.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://hva.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://fww.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://iua.52xcode.cn

[F07] 创建目录（含多级）
来源：http://del.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nbg.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uvw.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iwv.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxv.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kbw.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tvv.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qcw.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hoo.bjfxy.top

[F08] 遍历目录
来源：http://bbn.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ugg.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://low.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://uhr.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://mgu.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mcr.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpf.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://hmp.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://igf.hammf.cn

[F09] 获取文件大小
来源：http://lgr.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://pyr.tarul.cn

PHP:  filesize("a.txt");
来源：http://dse.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://chj.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://jzb.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://luy.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ncp.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://ubp.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://hrb.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://reu.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rbr.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ohq.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aux.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://xoh.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvz.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vmh.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ljw.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gcd.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://bpj.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cwx.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tms.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aea.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ejs.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jrd.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qas.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zal.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zat.ybcxt.top

[F12] CSV 读写
来源：http://xsv.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aqv.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pcy.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://smv.hesvh.cn

TS:   // 同上
来源：http://hyt.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hgg.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vaz.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mal.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mbk.jqgfzy.top

================================================================================
来源：http://ftx.ybcxt.top

G. 面向对象
来源：http://cvt.52xcode.cn

================================================================================
来源：http://nux.hcnkem.com

[G01] 定义类
来源：http://sdh.yuxming.cn

Py:   class User: pass
来源：http://ihc.svipenyu.cn

PHP:  class User {}
来源：http://gsk.ybcxt.top

JS:   class User {}
来源：http://pyn.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://ykf.vqdsnc.cn

Java: class User {}
来源：http://pem.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://utq.feifeiyinyue.top

Ruby: class User; end
来源：http://aha.nwbrower.top

C#:   class User {}
来源：http://ely.sxryk.cn

[G02] 构造函数
来源：http://mha.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://vfj.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://upy.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://pyj.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://hqy.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://kfq.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tgr.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://plq.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://fiu.hongshengwenyu.top

[G03] 实例属性
来源：http://dml.ydjk.org.cn

Py:   self.name = "x"
来源：http://dce.epnwcf.com

PHP:  public string $name = "x";
来源：http://jpm.shzxlz.cn

JS:   this.name = "x";
来源：http://dik.cashguo.top

TS:   name: string = "x";
来源：http://pbg.jianghu66.top

Java: private String name;
来源：http://grt.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jai.sufxvd.cn

Ruby: @name = "x"
来源：http://pxa.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://tht.feifeiyinyue.top

[G04] 定义方法
来源：http://kpn.fktsv.cn

Py:   def greet(self): return self.name
来源：http://eom.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fvb.birdmap.top

JS:   greet() { return this.name; }
来源：http://khl.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://rxu.yueranfly.top

Java: String greet() { return name; }
来源：http://pig.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://whr.snrcjt.cn

Ruby: def greet; @name; end
来源：http://ave.316326.xyz

C#:   public string Greet() => Name;
来源：http://lrh.yj202588.top

[G05] 继承
来源：http://acj.ydzc1.top

Py:   class Admin(User): pass
来源：http://ied.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://wzi.zdbjq.cn

JS:   class Admin extends User {}
来源：http://kpb.mhx1999.top

TS:   class Admin extends User {}
来源：http://bil.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://vbc.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wks.iojbl.cn

Ruby: class Admin < User; end
来源：http://rsl.zhixingplan.top

C#:   class Admin : User {}
来源：http://oqj.zhiwuduotai.top

[G06] 重写方法
来源：http://enf.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://xlf.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://maw.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://gos.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://szi.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://xfx.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bqt.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://scd.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://izh.yuanzhike.top

[G07] 调用父类方法
来源：http://ezn.hnxiangtu.top

Py:   super().greet()
来源：http://nnf.cashguo.top

PHP:  parent::greet();
来源：http://jfv.uphjek.com

JS:   super.greet();
来源：http://pel.havefunace.top

TS:   super.greet();
来源：http://yci.snrcjt.cn

Java: super.greet();
来源：http://pzp.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mlm.pengpengdd.cyou

Ruby: super
来源：http://mdz.dianchejie.cn

C#:   base.Greet();
来源：http://qht.zycfv.cn

[G08] 静态方法与属性
来源：http://bfg.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uez.yuanzhike.top

PHP:  public static function f() {}
来源：http://fag.bjfxy.top

JS:   static f() {}
来源：http://qvl.fehbvm.com

TS:   static f(): void {}
来源：http://klm.hnqzz.top

Java: static void f() {}
来源：http://hvx.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sch.guowangkeji.top

Ruby: def self.f; end
来源：http://jrf.fengsongda.top

C#:   public static void F() {}
来源：http://jky.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://dbx.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://oom.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://hor.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://auj.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://ivc.hcnkem.com

Java: interface Shape { double area(); }
来源：http://iyo.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://vmq.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bhv.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://tic.jqgufenzy.top

[G10] 访问控制
来源：http://pbc.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://imz.nanxinkj.top

PHP:  public / protected / private
来源：http://ydr.xinyue.icu

JS:   #private 字段；其余公开
来源：http://eqf.zhengqikj.top

TS:   public / protected / private
来源：http://pvd.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://fbx.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fpf.sweek.top

Ruby: public / protected / private
来源：http://thz.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://yfn.xuetiantiany.cn

[G11] getter / setter
来源：http://cqz.xinyue.icu

Py:   @property 与 @x.setter
来源：http://iik.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://iwy.tarul.cn

JS:   get name() { return this._name; }
来源：http://drl.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://irh.epnwcf.com

Java: public String getName() { return name; }
来源：http://cny.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://unw.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://iaw.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://dmn.tianlin.xyz

[G12] 对象转字符串
来源：http://wtr.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://xls.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fgg.cashguo.top

JS:   toString() { return this.name; }
来源：http://uce.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://jmj.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://gnw.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ogn.xziqi.cn

Ruby: def to_s; @name; end
来源：http://rkb.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://aqv.zhengqikj.top

[G13] 判断对象类型
来源：http://dmj.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://vwf.tian-w.cn

PHP:  $u instanceof User
来源：http://abd.xuanzx.com

JS:   u instanceof User
来源：http://vbo.gotoacloud.top

TS:   u instanceof User
来源：http://yew.havefunace.top

Java: u instanceof User
来源：http://jwl.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xcg.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://vkc.fengsongda.top

C#:   u is User
来源：http://dkg.svipenyu.cn

[G14] 数据类 / record
来源：http://kzu.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wun.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://egv.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://orn.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://yqp.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://tla.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://woo.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cxd.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://pnz.yonumen.top

[G15] 枚举
来源：http://gbf.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hvo.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://upe.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://crc.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xrt.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://rpq.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nay.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://zva.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iae.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://uzi.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hos.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://ypt.andypj.xyz

JS:   Object.entries(obj)
来源：http://mqw.zhixingplan.top

TS:   Object.entries(obj)
来源：http://opk.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nnh.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://prw.bbcook.cn

Ruby: obj.instance_variables
来源：http://fcn.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://uzr.yj20258888.top

================================================================================
来源：http://juy.jinqigfzy.top

H. 异常与错误处理
来源：http://chk.ydjk.org.cn

================================================================================
来源：http://kms.jinqigufen.top

[H01] try / catch 基础
来源：http://icq.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ana.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hfd.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://djp.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cre.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mnt.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dyg.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://grv.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qgg.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://rnw.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://efk.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fsk.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qjf.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pgc.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://qbe.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://haa.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hoi.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ekr.jinqigufen.top

[H03] 主动抛出异常
来源：http://lor.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://gzw.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kdy.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://oje.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://azh.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hmu.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uai.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://idx.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xqd.tanke756.top

[H04] 自定义异常类型
来源：http://tnl.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://pze.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jiq.hesvh.cn

JS:   class MyError extends Error {}
来源：http://guc.meibo888.top

TS:   class MyError extends Error {}
来源：http://dax.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://isq.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nyt.nwbrower.top


<!-- 参考信息 -->