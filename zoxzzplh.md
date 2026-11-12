代发 wailian999

Go:   if s == "" {}
来源：http://mnz.snrcjt.cn

Ruby: if s.empty?
来源：http://unn.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tkc.redwolf501.top

[E21] 超长截断加省略号
来源：http://tch.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iuh.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sam.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lnf.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dwm.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dnk.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://ewn.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://glk.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwp.guannengcc.top

[E22] 字节长度与字符长度
来源：http://ued.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nlw.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myn.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://diz.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qaj.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://plh.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://omd.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://yno.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bgg.zdqjudy.top

================================================================================
来源：http://nqy.tianlin.xyz

F. 文件与目录
来源：http://ehy.dashuyun.cn

================================================================================
来源：http://qnu.cdnleiting.top

[F01] 读取整个文件
来源：http://gas.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sqr.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://gul.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://him.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ejj.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vsv.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vgu.xuetiantiany.cn

Ruby: File.read("a.txt")
来源：http://gtq.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://aek.jinqigfzy.top

[F02] 逐行读取文件
来源：http://qal.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pfg.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hwj.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyh.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tjv.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ptd.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://otn.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://koo.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://awe.sweek.top

[F03] 写入文件（覆盖）
来源：http://jny.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mty.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dgw.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vff.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jzt.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ppz.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://api.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://qvj.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bbq.xylfe.cn

[F04] 追加写入文件
来源：http://mtl.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ano.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kvn.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nmd.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bvm.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wic.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dnt.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awc.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipj.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://xii.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nvv.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://lcd.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://qgh.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://jcd.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://poc.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ugj.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://jez.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://fgp.svipenyu.cn

[F06] 删除文件
来源：http://uah.sysykeji.top

Py:   os.remove("a.txt")
来源：http://vbd.meibo888.top

PHP:  unlink("a.txt");
来源：http://dzv.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hsf.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://abo.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hzu.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://mck.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://odo.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://tbz.tarul.cn

[F07] 创建目录（含多级）
来源：http://zty.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cbl.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ovz.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxf.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trj.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pam.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cgw.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xjk.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bsv.hammf.cn

[F08] 遍历目录
来源：http://aeb.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rdi.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nab.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://jlx.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://kfg.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ilr.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ttp.hnqzz.top

Ruby: Dir.children("dir")
来源：http://ice.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://woj.ybcxt.top

[F09] 获取文件大小
来源：http://jwl.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://oqu.zycfv.cn

PHP:  filesize("a.txt");
来源：http://opu.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://mhh.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://fzs.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://shz.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gtv.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://qnu.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://pmb.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://kjn.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cru.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://buh.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cdq.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://oww.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ucn.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wah.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aed.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxu.cdnleiting.top

[F11] 复制与移动文件
来源：http://xdh.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oon.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://foe.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oce.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dqe.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lmf.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xhc.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://edm.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ypw.yongpay.top

[F12] CSV 读写
来源：http://mxc.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://get.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://byo.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gvh.dianchejie.cn

TS:   // 同上
来源：http://lck.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mml.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kgi.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bok.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cqm.iojbl.cn

================================================================================
来源：http://fxd.cqqwz.cn

G. 面向对象
来源：http://ejx.ywan-chungtsiang.top

================================================================================
来源：http://cxj.shuidangran.top

[G01] 定义类
来源：http://vfv.xuanzx.com

Py:   class User: pass
来源：http://rcf.ydjk.org.cn

PHP:  class User {}
来源：http://yug.zhijiandao.cn

JS:   class User {}
来源：http://nhd.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://ahb.snrcjt.cn

Java: class User {}
来源：http://iru.andypj.xyz

Go:   type User struct { Name string }
来源：http://vbf.vehdjk.com

Ruby: class User; end
来源：http://dbc.haohaochexian.top

C#:   class User {}
来源：http://pbc.ydzc1.top

[G02] 构造函数
来源：http://hpp.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://gqb.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ffp.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://lax.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://chr.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://qin.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dgk.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://eqf.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://jnw.cheryme.top

[G03] 实例属性
来源：http://bbt.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://vca.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://ehl.zhoulong.xyz

JS:   this.name = "x";
来源：http://hdb.tarul.cn

TS:   name: string = "x";
来源：http://qgy.guowangkeji.top

Java: private String name;
来源：http://ngv.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kbc.fktsv.cn

Ruby: @name = "x"
来源：http://ezz.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://cuv.xinyue.icu

[G04] 定义方法
来源：http://kdf.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://kbu.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ufo.hnqzz.top

JS:   greet() { return this.name; }
来源：http://vla.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://nbr.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://kme.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vyk.gogol.net.cn

Ruby: def greet; @name; end
来源：http://gho.pycfn.com

C#:   public string Greet() => Name;
来源：http://ymd.chenzaomai.com

[G05] 继承
来源：http://xmu.uphjek.com

Py:   class Admin(User): pass
来源：http://sru.316326.xyz

PHP:  class Admin extends User {}
来源：http://qbl.fehbvm.com

JS:   class Admin extends User {}
来源：http://vtz.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://wbk.yuanzhike.top

Java: class Admin extends User {}
来源：http://htj.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gqo.havefunace.top

Ruby: class Admin < User; end
来源：http://mkt.gogol.net.cn

C#:   class Admin : User {}
来源：http://cxp.tian-w.cn

[G06] 重写方法
来源：http://wim.cashguo.top

Py:   def greet(self): return "admin"
来源：http://frj.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jms.sweek.top

JS:   greet() { return "admin"; }
来源：http://fef.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://vlo.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://loe.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dgg.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://njp.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://hdp.hnqzz.top

[G07] 调用父类方法
来源：http://rxk.sxryk.cn

Py:   super().greet()
来源：http://cry.cucudq.cn

PHP:  parent::greet();
来源：http://zel.quarkkingdee.top

JS:   super.greet();
来源：http://jrs.epnwcf.com

TS:   super.greet();
来源：http://kaq.316326.xyz

Java: super.greet();
来源：http://lmc.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sba.xuanzx.com

Ruby: super
来源：http://llc.fzhhl.top

C#:   base.Greet();
来源：http://edw.vehdjk.com

[G08] 静态方法与属性
来源：http://jrj.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://irr.sweek.top

PHP:  public static function f() {}
来源：http://hae.jinqigufen.top

JS:   static f() {}
来源：http://uqy.ydzc1.top

TS:   static f(): void {}
来源：http://voa.guowangkeji.top

Java: static void f() {}
来源：http://dsm.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://mry.hfpthk.cn

Ruby: def self.f; end
来源：http://qjp.hywenlv.cn

C#:   public static void F() {}
来源：http://nyj.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://lfu.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://jzf.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://htg.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mll.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://dkh.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://eqo.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://jov.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sid.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://yix.cqqwz.cn

[G10] 访问控制
来源：http://xly.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://bjt.316326.xyz

PHP:  public / protected / private
来源：http://lmx.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://lug.smart0.xyz

TS:   public / protected / private
来源：http://tkj.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://cuy.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sxm.haohaochexian.top

Ruby: public / protected / private
来源：http://mma.cucudq.cn

C#:   public / protected / private / internal
来源：http://drs.jqgufenzy.top

[G11] getter / setter
来源：http://ets.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://hvn.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rxk.fktsv.cn

JS:   get name() { return this._name; }
来源：http://ypb.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://npn.fehbvm.com

Java: public String getName() { return name; }
来源：http://zkw.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzn.ctjpmb.com

Ruby: attr_accessor :name
来源：http://ehd.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://lda.uphjek.com

[G12] 对象转字符串
来源：http://qfj.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://zod.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fbn.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://kdd.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://hij.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://yyh.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://acz.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://bqy.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://loc.yangfankeji.com

[G13] 判断对象类型
来源：http://aud.tianlin.xyz

Py:   isinstance(u, User)
来源：http://axa.mhx1999.top

PHP:  $u instanceof User
来源：http://unk.yonumen.top

JS:   u instanceof User
来源：http://tjt.meibo888.top

TS:   u instanceof User
来源：http://ihb.tanke756.top

Java: u instanceof User
来源：http://kqk.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://syg.xziqi.cn

Ruby: u.is_a?(User)
来源：http://tii.ehwqpu.com

C#:   u is User
来源：http://mlt.guowangkeji.top

[G14] 数据类 / record
来源：http://owd.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wyb.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://lbe.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://vrs.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://fis.uphjek.com

Java: record User(String name, int age) {}
来源：http://ske.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://jss.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://okg.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://sip.tarul.cn

[G15] 枚举
来源：http://vfi.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://itl.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gim.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fvn.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://udd.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://pum.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://siv.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://twg.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://umh.yongpay.top

[G16] 对象转数组 / 字典
来源：http://hxs.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hue.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://zmy.yangfankeji.com

JS:   Object.entries(obj)
来源：http://fvl.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://kmy.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dih.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xwy.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://hyx.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://krb.zhoulong.xyz

================================================================================
来源：http://cbg.bjfxy.top

H. 异常与错误处理
来源：http://fhv.sysykeji.top

================================================================================
来源：http://law.tian-w.cn

[H01] try / catch 基础
来源：http://yay.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xko.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xku.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xcx.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aob.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ghf.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ymw.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ivn.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://stu.ybcxt.top

[H02] finally / ensure 收尾
来源：http://iyi.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://ltz.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://xej.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xmg.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tdh.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://qmw.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytt.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wog.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ijj.xziqi.cn


<!-- 参考信息 -->