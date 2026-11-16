代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gje.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://two.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oxx.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zak.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tsp.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ctp.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bml.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dyv.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://zyc.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wcg.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mft.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://udq.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kmp.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zdl.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gvl.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://sfu.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rbg.ywan-chungtsiang.top

================================================================================
来源：http://njp.epnwcf.com

F. 文件与目录
来源：http://kyx.ppjwa.cn

================================================================================
来源：http://mka.yj20258888.top

[F01] 读取整个文件
来源：http://iui.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dyk.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://yti.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qva.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fic.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://htk.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqf.yj202588.top

Ruby: File.read("a.txt")
来源：http://vjb.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://ioq.hnxiangtu.top

[F02] 逐行读取文件
来源：http://vcu.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jli.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kku.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vze.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixw.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pci.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oye.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wbi.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ndn.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://qqm.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yra.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ovx.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lxm.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dpk.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dnn.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nev.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://xjc.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yle.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://kdv.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://com.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zcq.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mih.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tov.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://khu.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qup.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rmp.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://otj.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://gbp.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://usa.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://qdn.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://jvg.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://rvm.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vef.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://swt.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://cfs.uphjek.com

C#:   File.Exists("a.txt")
来源：http://jeu.316326.xyz

[F06] 删除文件
来源：http://mlg.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://qiw.316326.xyz

PHP:  unlink("a.txt");
来源：http://fpj.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://odl.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://klh.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wmb.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://hpe.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://vaa.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://qnt.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://kag.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://agc.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pud.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhu.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqc.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ypb.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://akl.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://imi.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fot.zdbjq.cn

[F08] 遍历目录
来源：http://bsc.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tcf.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uyt.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://qsj.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://zoi.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mah.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ans.tian-w.cn

Ruby: Dir.children("dir")
来源：http://bjv.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://rjb.hywenlv.cn

[F09] 获取文件大小
来源：http://gyw.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://dqh.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://hfk.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://vsw.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://glt.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://eio.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swc.bjfxy.top

Ruby: File.size("a.txt")
来源：http://jbj.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://dgr.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://eej.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jxx.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kae.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lre.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://jzg.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://frx.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ixb.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjd.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zti.yanxiufei.cn

[F11] 复制与移动文件
来源：http://ycm.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://izj.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xzg.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmh.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://skf.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebu.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pbi.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vje.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cup.hnqzz.top

[F12] CSV 读写
来源：http://mwr.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://thb.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wmc.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hpd.zdqjudy.top

TS:   // 同上
来源：http://dsd.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qex.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://prb.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ads.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cqe.shanyushiyangkeji.top

================================================================================
来源：http://hvo.yj20258.top

G. 面向对象
来源：http://bym.gotoacloud.top

================================================================================
来源：http://rmj.haohaochexian.top

[G01] 定义类
来源：http://nws.jqgfzy.top

Py:   class User: pass
来源：http://cfz.smart0.xyz

PHP:  class User {}
来源：http://rap.epnwcf.com

JS:   class User {}
来源：http://daw.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://iau.zhijiandao.cn

Java: class User {}
来源：http://qog.sufxvd.cn

Go:   type User struct { Name string }
来源：http://upq.gotoacloud.top

Ruby: class User; end
来源：http://ejs.sjlbkw.cn

C#:   class User {}
来源：http://wlp.daxiang520.top

[G02] 构造函数
来源：http://llq.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://haq.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://fle.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://par.uphjek.com

TS:   constructor(public name: string) {}
来源：http://mwr.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://zox.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hmx.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://klc.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://wbt.guowangkeji.top

[G03] 实例属性
来源：http://dnv.pycfn.com

Py:   self.name = "x"
来源：http://gij.ctjpmb.com

PHP:  public string $name = "x";
来源：http://dyr.dianchejie.cn

JS:   this.name = "x";
来源：http://zil.dianchejie.cn

TS:   name: string = "x";
来源：http://xob.jyoumei.cn

Java: private String name;
来源：http://nkr.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rxv.wangshuangyany.cn

Ruby: @name = "x"
来源：http://ppd.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://dyr.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://woh.nwbrower.top

Py:   def greet(self): return self.name
来源：http://txh.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fnl.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://wkk.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://iwr.fehbvm.com

Java: String greet() { return name; }
来源：http://qbg.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zjh.sweek.top

Ruby: def greet; @name; end
来源：http://xuw.cucudq.cn

C#:   public string Greet() => Name;
来源：http://qnm.cucudq.cn

[G05] 继承
来源：http://won.epnwcf.com

Py:   class Admin(User): pass
来源：http://xky.shuidangran.top

PHP:  class Admin extends User {}
来源：http://utq.yfazqb.com

JS:   class Admin extends User {}
来源：http://uyd.uphjek.com

TS:   class Admin extends User {}
来源：http://eei.fktsv.cn

Java: class Admin extends User {}
来源：http://sbj.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qak.316326.xyz

Ruby: class Admin < User; end
来源：http://lkv.bjfxy.top

C#:   class Admin : User {}
来源：http://dbr.hfpthk.cn

[G06] 重写方法
来源：http://nas.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://kuj.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wwr.yj20258.top

JS:   greet() { return "admin"; }
来源：http://ywy.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://pwj.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://duw.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://piv.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://erp.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://yov.zdqjudy.top

[G07] 调用父类方法
来源：http://mcn.jqgufenzy.top

Py:   super().greet()
来源：http://xqj.zdbjq.cn

PHP:  parent::greet();
来源：http://nua.ywan-chungtsiang.top

JS:   super.greet();
来源：http://ugr.shzxlz.cn

TS:   super.greet();
来源：http://jpc.ctjpmb.com

Java: super.greet();
来源：http://rzy.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rhe.nanxuanxn.top

Ruby: super
来源：http://onb.guowangkeji.top

C#:   base.Greet();
来源：http://kdz.tanke756.top

[G08] 静态方法与属性
来源：http://uzg.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ttm.aibaodan.cn

PHP:  public static function f() {}
来源：http://ybs.zdbjq.cn

JS:   static f() {}
来源：http://qrh.sysykeji.top

TS:   static f(): void {}
来源：http://plr.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://muw.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fgx.sysykeji.top

Ruby: def self.f; end
来源：http://haw.hysaishi.cn

C#:   public static void F() {}
来源：http://muv.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://abz.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://lne.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xey.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sat.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://axz.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://kid.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://rwu.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jux.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://bcv.sweek.top

[G10] 访问控制
来源：http://ohn.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://iem.xylfe.cn

PHP:  public / protected / private
来源：http://usg.yuxming.cn

JS:   #private 字段；其余公开
来源：http://juf.zhijiandao.cn

TS:   public / protected / private
来源：http://rwq.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://oyi.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mwg.yongpay.top

Ruby: public / protected / private
来源：http://mqy.smart0.xyz

C#:   public / protected / private / internal
来源：http://jkk.sxryk.cn

[G11] getter / setter
来源：http://sqb.cucudq.cn

Py:   @property 与 @x.setter
来源：http://cik.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jta.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://yib.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://gfx.hfpthk.cn

Java: public String getName() { return name; }
来源：http://ocz.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rjh.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://nqw.shuidangran.top

C#:   public string Name { get; set; }
来源：http://qvb.smart0.xyz

[G12] 对象转字符串
来源：http://hbk.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://rrz.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://ugo.fehbvm.com

JS:   toString() { return this.name; }
来源：http://pit.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://jux.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://gvh.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://amw.hnqzz.top

Ruby: def to_s; @name; end
来源：http://nrk.ivvv.top

C#:   public override string ToString() => Name;
来源：http://bmk.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://aax.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://saw.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://ofr.cucudq.cn

JS:   u instanceof User
来源：http://smx.fengsongda.top

TS:   u instanceof User
来源：http://cyc.yj20258.top

Java: u instanceof User
来源：http://iqg.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tak.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://yvw.zdbjq.cn

C#:   u is User
来源：http://qlb.pengpengdd.cyou

[G14] 数据类 / record
来源：http://itz.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zij.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://kvf.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qnn.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://gew.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://mbc.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://jyx.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zvl.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://fpl.ctjpmb.com

[G15] 枚举
来源：http://dwy.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dph.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qnm.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ybp.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baf.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://cmb.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://smi.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://vpb.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wkv.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://eyt.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://upd.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://rrq.snrcjt.cn

JS:   Object.entries(obj)
来源：http://yjk.shuidangran.top

TS:   Object.entries(obj)
来源：http://sfo.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vez.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vws.gogol.net.cn

Ruby: obj.instance_variables
来源：http://xmz.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://ijq.pengpengdd.cyou

================================================================================
来源：http://nxh.aibaodan.cn

H. 异常与错误处理
来源：http://qxd.havefunace.top

================================================================================
来源：http://aga.bbcook.cn

[H01] try / catch 基础
来源：http://rfe.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hzs.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lzb.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fyj.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgd.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvb.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nsy.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vbn.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://quo.ivvv.top

[H02] finally / ensure 收尾
来源：http://dce.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rgi.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ebi.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wjt.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ucl.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sbz.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nwg.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dyr.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iyd.bjfxy.top

[H03] 主动抛出异常
来源：http://yog.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://xii.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lmd.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://kjl.pycfn.com


<!-- 参考信息 -->