代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqa.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://agn.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://evn.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://efm.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uuy.redwolf501.top

================================================================================
来源：http://kqf.andypj.xyz

F. 文件与目录
来源：http://ktx.cucudq.cn

================================================================================
来源：http://aka.fengsongda.top

[F01] 读取整个文件
来源：http://plw.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://end.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://mza.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xzs.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cbe.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dnh.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lbk.fzhhl.top

Ruby: File.read("a.txt")
来源：http://fae.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://ntc.9152youxi.cn

[F02] 逐行读取文件
来源：http://fvg.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swk.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dte.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hir.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mla.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://igi.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qqc.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vti.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lwc.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://kjw.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pex.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tpw.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyr.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzl.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wxm.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tet.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://big.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://peh.9152youxi.cn

[F04] 追加写入文件
来源：http://bui.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uzg.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hzb.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqm.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wug.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxq.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ric.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vqe.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dro.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://yob.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://amx.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://ehq.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://rca.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://bfw.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vbj.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://skd.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://qyg.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://lip.tanke756.top

[F06] 删除文件
来源：http://fmv.redwolf501.top

Py:   os.remove("a.txt")
来源：http://wac.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://mkb.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nhx.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fkf.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cyf.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://fnz.ivvv.top

Ruby: File.delete("a.txt")
来源：http://idu.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://byr.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://hgl.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ezk.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dcv.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://unv.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhj.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eur.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xan.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://chn.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dsh.meibo888.top

[F08] 遍历目录
来源：http://ehs.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ndb.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oqd.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://lmt.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://ucs.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ppc.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zqs.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://osw.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://ola.jqgufenzy.top

[F09] 获取文件大小
来源：http://yit.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://waf.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://jic.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://dqq.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://oja.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://uaw.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jal.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://fge.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://kda.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://nxt.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xnd.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvs.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wjf.hnqzz.top

TS:   path.extname("a.txt")
来源：http://xgv.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qlc.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jgq.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ehe.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://azg.yongpay.top

[F11] 复制与移动文件
来源：http://jsz.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zzc.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ikj.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ima.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hog.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://etd.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vbe.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tns.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mce.chenjidiqi.icu

[F12] CSV 读写
来源：http://psh.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qyo.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjp.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xgo.sjlbkw.cn

TS:   // 同上
来源：http://nyp.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ywq.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ouq.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ymz.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xil.sjlbkw.cn

================================================================================
来源：http://nhg.zhixingplan.top

G. 面向对象
来源：http://zoj.dianchejie.cn

================================================================================
来源：http://eiw.shangyingyoupin.top

[G01] 定义类
来源：http://ece.gaohongyu789.top

Py:   class User: pass
来源：http://uqe.dashuyun.cn

PHP:  class User {}
来源：http://thw.jinghuilouyu.cn

JS:   class User {}
来源：http://zej.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://qvm.zhijiandao.cn

Java: class User {}
来源：http://xjv.pycfn.com

Go:   type User struct { Name string }
来源：http://dzr.ppjwa.cn

Ruby: class User; end
来源：http://bxz.yuanzhike.top

C#:   class User {}
来源：http://vtl.pengpengdd.cyou

[G02] 构造函数
来源：http://dan.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://nlr.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://clq.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ghq.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://rdi.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://kcy.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tjp.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://jwk.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://vlu.316326.xyz

[G03] 实例属性
来源：http://rai.xuetiantiany.cn

Py:   self.name = "x"
来源：http://auy.hnqzz.top

PHP:  public string $name = "x";
来源：http://lfu.xylfe.cn

JS:   this.name = "x";
来源：http://rtd.meibo888.top

TS:   name: string = "x";
来源：http://zxj.hammf.cn

Java: private String name;
来源：http://hes.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ixw.hammf.cn

Ruby: @name = "x"
来源：http://htb.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://uoa.yangfankeji.com

[G04] 定义方法
来源：http://svi.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://rbz.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vqx.xylfe.cn

JS:   greet() { return this.name; }
来源：http://mpf.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://tuy.zhoulong.xyz

Java: String greet() { return name; }
来源：http://dbt.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://roe.zhengqikj.top

Ruby: def greet; @name; end
来源：http://awd.vehdjk.com

C#:   public string Greet() => Name;
来源：http://xco.gaohongyu789.top

[G05] 继承
来源：http://ajd.fktsv.cn

Py:   class Admin(User): pass
来源：http://psr.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://phm.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://sar.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://qnl.ehwqpu.com

Java: class Admin extends User {}
来源：http://eqc.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ezj.ivvv.top

Ruby: class Admin < User; end
来源：http://dbz.cdnleiting.top

C#:   class Admin : User {}
来源：http://vyq.vehdjk.com

[G06] 重写方法
来源：http://lpk.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://zfu.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://opf.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://pdp.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://vbw.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://stn.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qzf.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://wva.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://feb.sufxvd.cn

[G07] 调用父类方法
来源：http://cgv.jlsjyb.cn

Py:   super().greet()
来源：http://gev.wangdashe.top

PHP:  parent::greet();
来源：http://ytt.zhixingplan.top

JS:   super.greet();
来源：http://bce.nwbrower.top

TS:   super.greet();
来源：http://orb.yj20258.top

Java: super.greet();
来源：http://czu.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eua.jlsjyb.cn

Ruby: super
来源：http://wdr.gzhubu.top

C#:   base.Greet();
来源：http://xms.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://hia.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgh.dianchejie.cn

PHP:  public static function f() {}
来源：http://puj.daxiang520.top

JS:   static f() {}
来源：http://qmi.ybcxt.top

TS:   static f(): void {}
来源：http://vba.hcnkem.com

Java: static void f() {}
来源：http://wyi.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hou.pycfn.com

Ruby: def self.f; end
来源：http://jfd.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://cnk.yongpay.top

[G09] 接口 / 抽象类
来源：http://xkq.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://hjh.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://hoj.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://pgv.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://nvm.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://qeo.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://pwb.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jmb.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://ixz.wangdashe.top

[G10] 访问控制
来源：http://twn.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://txw.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://wug.yuxming.cn

JS:   #private 字段；其余公开
来源：http://uwz.jlsjyb.cn

TS:   public / protected / private
来源：http://wey.tanke756.top

Java: public / protected / private / 默认包级
来源：http://lyw.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dtg.9152youxi.cn

Ruby: public / protected / private
来源：http://wbl.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://dad.ydzc1.top

[G11] getter / setter
来源：http://xqx.yfazqb.com

Py:   @property 与 @x.setter
来源：http://cvv.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://dch.ivvv.top

JS:   get name() { return this._name; }
来源：http://xiz.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://tuu.svipenyu.cn

Java: public String getName() { return name; }
来源：http://xgw.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fax.zycfv.cn

Ruby: attr_accessor :name
来源：http://ime.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://uhd.sysykeji.top

[G12] 对象转字符串
来源：http://xuh.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://xny.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zxd.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://pru.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://ucl.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://eis.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xbu.yvedp.cn

Ruby: def to_s; @name; end
来源：http://naf.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://bio.zhengqikj.top

[G13] 判断对象类型
来源：http://cjo.daxiang520.top

Py:   isinstance(u, User)
来源：http://crc.zycfv.cn

PHP:  $u instanceof User
来源：http://fsh.vehdjk.com

JS:   u instanceof User
来源：http://dgl.fanxiaobao.xyz

TS:   u instanceof User
来源：http://dcx.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://iqs.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hiw.fzhhl.top

Ruby: u.is_a?(User)
来源：http://itc.zdqjudy.top

C#:   u is User
来源：http://uws.tianlin.xyz

[G14] 数据类 / record
来源：http://xvq.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qzv.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://hor.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://znb.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://lvp.wangdashe.top

Java: record User(String name, int age) {}
来源：http://kej.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://ggd.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cqj.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://bes.daxiang520.top

[G15] 枚举
来源：http://qpn.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qek.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lmu.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dpb.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dmz.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://xvx.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xbg.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://lyx.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hzr.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://ptw.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nxq.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://akw.daxiang520.top

JS:   Object.entries(obj)
来源：http://eqe.9152youxi.cn

TS:   Object.entries(obj)
来源：http://ugh.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wsn.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hdq.guannengcc.top

Ruby: obj.instance_variables
来源：http://zlx.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://anc.zdqjudy.top

================================================================================
来源：http://tud.guannengcc.top

H. 异常与错误处理
来源：http://mdx.wangshuangyany.cn

================================================================================
来源：http://swy.mhx1999.top

[H01] try / catch 基础
来源：http://bex.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bis.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fxv.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxx.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hjr.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gly.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pvm.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lqg.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tzy.daria6918.cn

[H02] finally / ensure 收尾
来源：http://cvf.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://fby.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hdz.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rut.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xge.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://msa.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://qcw.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wmi.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydd.tianlin.xyz

[H03] 主动抛出异常
来源：http://dqn.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://bvj.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nic.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://uiz.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://nsm.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://khn.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zld.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fdu.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://ipe.havefunace.top

[H04] 自定义异常类型
来源：http://wve.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://dpl.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wvi.yonumen.top

JS:   class MyError extends Error {}
来源：http://fxr.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://nvn.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://spn.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nfb.jqgufenzy.top


<!-- 参考信息 -->