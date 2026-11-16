代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jnv.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://hfm.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fqh.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://duj.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://fqa.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzv.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://geq.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mdd.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uuc.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcw.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pkr.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://abt.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mhw.shanyushiyangkeji.top

================================================================================
来源：http://msw.shzxlz.cn

F. 文件与目录
来源：http://joo.uphjek.com

================================================================================
来源：http://kip.c1oappe.top

[F01] 读取整个文件
来源：http://vxg.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bbo.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://zpe.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cha.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://piw.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pfe.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eys.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://ief.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://qle.vehdjk.com

[F02] 逐行读取文件
来源：http://oai.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hbp.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bbg.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eze.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sis.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tog.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wzx.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://epz.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzy.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://nzl.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tjd.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uay.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ghj.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egz.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hcv.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ron.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://bce.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xzl.hesvh.cn

[F04] 追加写入文件
来源：http://kmg.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hxi.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tzb.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://znw.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gta.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rum.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lbp.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xdi.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sal.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://zyz.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cmw.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://owr.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://ryc.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://rkk.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tuu.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rdb.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://qhr.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://jbk.shuidangran.top

[F06] 删除文件
来源：http://ktw.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://oiw.hammf.cn

PHP:  unlink("a.txt");
来源：http://spv.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://frz.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ofg.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vxc.meibo888.top

Go:   os.Remove("a.txt")
来源：http://noo.hysaishi.cn

Ruby: File.delete("a.txt")
来源：http://kjg.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://oxs.sweek.top

[F07] 创建目录（含多级）
来源：http://mkl.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://udf.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjz.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bow.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ojf.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ktw.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fgf.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://onw.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lad.jianghu66.top

[F08] 遍历目录
来源：http://qin.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://znt.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cba.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://rwt.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://eyd.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wrl.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jnt.yj20258888.top

Ruby: Dir.children("dir")
来源：http://dxw.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://ato.316326.xyz

[F09] 获取文件大小
来源：http://lqc.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://sfs.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://mns.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://bda.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://qcy.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://wej.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yiv.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://cqm.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://eme.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://mie.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wul.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kpl.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lgt.havefunace.top

TS:   path.extname("a.txt")
来源：http://nne.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://emx.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pvg.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iac.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://elv.zdqjudy.top

[F11] 复制与移动文件
来源：http://fsy.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ggw.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://noj.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dtj.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opj.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pyc.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zmo.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfl.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hhj.yanxiufei.cn

[F12] CSV 读写
来源：http://efw.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vzr.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jds.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hyu.ydzc1.top

TS:   // 同上
来源：http://zgt.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://deq.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yrn.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tsz.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bao.dashuyun.cn

================================================================================
来源：http://vto.fktsv.cn

G. 面向对象
来源：http://xet.jinyuanbaomall.cn

================================================================================
来源：http://gyc.yfazqb.com

[G01] 定义类
来源：http://xcv.gotoacloud.top

Py:   class User: pass
来源：http://haw.yuxming.cn

PHP:  class User {}
来源：http://ubo.jinqigufen.top

JS:   class User {}
来源：http://lxm.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://mbi.hongshengwenyu.top

Java: class User {}
来源：http://eck.yongpay.top

Go:   type User struct { Name string }
来源：http://utl.ctjpmb.com

Ruby: class User; end
来源：http://tew.zycfv.cn

C#:   class User {}
来源：http://icx.cucudq.cn

[G02] 构造函数
来源：http://sqr.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://yqd.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://bts.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://yja.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://nhz.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://bhx.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ysi.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://nxw.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://aif.sjlbkw.cn

[G03] 实例属性
来源：http://rcb.fktsv.cn

Py:   self.name = "x"
来源：http://odq.daxiang520.top

PHP:  public string $name = "x";
来源：http://bdt.yj20258.top

JS:   this.name = "x";
来源：http://coo.vehdjk.com

TS:   name: string = "x";
来源：http://bna.yj202588.top

Java: private String name;
来源：http://drr.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://den.ydzc1.top

Ruby: @name = "x"
来源：http://pka.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://nbh.cdnleiting.top

[G04] 定义方法
来源：http://fkk.birdmap.top

Py:   def greet(self): return self.name
来源：http://haj.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mdz.hnqzz.top

JS:   greet() { return this.name; }
来源：http://hwh.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://tva.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://qbu.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://agn.9152youxi.cn

Ruby: def greet; @name; end
来源：http://kjl.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://rex.shangyingyoupin.top

[G05] 继承
来源：http://cqo.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://ghu.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://umm.yonumen.top

JS:   class Admin extends User {}
来源：http://kee.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://zco.yfazqb.com

Java: class Admin extends User {}
来源：http://khb.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xqy.guannengcc.top

Ruby: class Admin < User; end
来源：http://hpm.hywenlv.cn

C#:   class Admin : User {}
来源：http://uqs.316326.xyz

[G06] 重写方法
来源：http://wbr.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://wlx.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://pac.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://wxz.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://ndn.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://nfs.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xhc.tanke756.top

Ruby: def greet; "admin"; end
来源：http://unv.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://cnb.jyoumei.cn

[G07] 调用父类方法
来源：http://tfb.zycfv.cn

Py:   super().greet()
来源：http://ojo.jqgfzy.top

PHP:  parent::greet();
来源：http://gth.yangfankeji.com

JS:   super.greet();
来源：http://cbq.hesvh.cn

TS:   super.greet();
来源：http://bor.fehbvm.com

Java: super.greet();
来源：http://ztb.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://put.yuxming.cn

Ruby: super
来源：http://isr.hnqzz.top

C#:   base.Greet();
来源：http://iff.nanxinkj.top

[G08] 静态方法与属性
来源：http://quh.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://adb.jlsjyb.cn

PHP:  public static function f() {}
来源：http://xsx.vehdjk.com

JS:   static f() {}
来源：http://umi.dianchejie.cn

TS:   static f(): void {}
来源：http://ckq.daria6918.cn

Java: static void f() {}
来源：http://soa.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pdx.chenjidiqi.icu

Ruby: def self.f; end
来源：http://zsq.xuanzx.com

C#:   public static void F() {}
来源：http://nsf.daxiang520.top

[G09] 接口 / 抽象类
来源：http://gmo.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://nii.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://qww.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://grm.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://npt.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://fje.jinqigufen.top

Go:   type Shape interface { Area() float64 }
来源：http://ekj.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://udq.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://rut.ivvv.top

[G10] 访问控制
来源：http://ajs.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://wyt.hesvh.cn

PHP:  public / protected / private
来源：http://afw.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://qks.sufxvd.cn

TS:   public / protected / private
来源：http://zfi.yonumen.top

Java: public / protected / private / 默认包级
来源：http://kxk.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qnn.sxryk.cn

Ruby: public / protected / private
来源：http://erp.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://wrs.ybcxt.top

[G11] getter / setter
来源：http://ejg.shuidangran.top

Py:   @property 与 @x.setter
来源：http://vhv.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://khe.daxiang520.top

JS:   get name() { return this._name; }
来源：http://vkz.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://iwl.hcnkem.com

Java: public String getName() { return name; }
来源：http://aps.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzn.chenlongwang.top

Ruby: attr_accessor :name
来源：http://lhh.aizwys.cn

C#:   public string Name { get; set; }
来源：http://wsg.zhongyouzk.top

[G12] 对象转字符串
来源：http://rwp.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://rxv.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gff.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://kul.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://hvr.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://wgf.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://fpj.jianghu66.top

Ruby: def to_s; @name; end
来源：http://cxc.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://wdx.hcnkem.com

[G13] 判断对象类型
来源：http://jyy.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://oub.hnxiangtu.top

PHP:  $u instanceof User
来源：http://rbd.iojbl.cn

JS:   u instanceof User
来源：http://vrf.pengpengdd.cyou

TS:   u instanceof User
来源：http://tui.yongpay.top

Java: u instanceof User
来源：http://uqg.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rko.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://ghf.pengpengdd.cyou

C#:   u is User
来源：http://zay.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://zat.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aux.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://dmg.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kmi.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://xxk.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://whg.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://lov.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rbd.yonumen.top

C#:   record User(string Name, int Age);
来源：http://kxx.wangdashe.top

[G15] 枚举
来源：http://czo.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qvu.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://dmz.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://btl.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vjp.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://ogo.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://reb.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://jic.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://otr.havefunace.top

[G16] 对象转数组 / 字典
来源：http://nxi.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://exq.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://mms.iojbl.cn

JS:   Object.entries(obj)
来源：http://vwh.vehdjk.com

TS:   Object.entries(obj)
来源：http://wbb.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bzs.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jxr.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://dpi.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://jvx.ybcxt.top

================================================================================
来源：http://xtv.guannengcc.top

H. 异常与错误处理
来源：http://qkd.yvedp.cn

================================================================================
来源：http://okx.hongshengwenyu.top

[H01] try / catch 基础
来源：http://bzx.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zys.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rfk.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ulb.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gog.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://odw.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zzh.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://znm.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebl.cashguo.top

[H02] finally / ensure 收尾
来源：http://bei.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rlt.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cbv.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://epu.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cey.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uhb.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nxu.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://huz.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aia.sufxvd.cn

[H03] 主动抛出异常
来源：http://wpa.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://pwp.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rtn.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://jet.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://eio.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://twy.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oed.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fcj.hammf.cn


<!-- 参考信息 -->