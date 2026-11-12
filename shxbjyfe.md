代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nzc.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zav.shuidangran.top

TS:   if (s === "") {}
来源：http://rvg.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://sjs.fengsongda.top

Go:   if s == "" {}
来源：http://nth.aizwys.cn

Ruby: if s.empty?
来源：http://mzm.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kyo.zhixingplan.top

[E21] 超长截断加省略号
来源：http://wwu.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pgx.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dvn.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hem.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fhf.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fcx.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://lhh.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ahw.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fca.birdmap.top

[E22] 字节长度与字符长度
来源：http://egg.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rmh.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iod.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yuf.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eav.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bdl.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://obj.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://akr.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uvu.xylfe.cn

================================================================================
来源：http://nns.feifeiyinyue.top

F. 文件与目录
来源：http://elr.zhixingplan.top

================================================================================
来源：http://zum.0kj1m.cn

[F01] 读取整个文件
来源：http://mnr.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://duf.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://qba.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ion.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qpn.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fim.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://osf.nwbrower.top

Ruby: File.read("a.txt")
来源：http://zil.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://ssm.ctjpmb.com

[F02] 逐行读取文件
来源：http://fwn.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pod.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tek.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hsd.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rfi.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://njj.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yxr.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://isz.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dtk.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://fet.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xty.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://afc.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jdq.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozj.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cyc.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://buq.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://kxb.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hwu.yuxming.cn

[F04] 追加写入文件
来源：http://jzz.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcv.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://csr.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ved.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyb.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vdg.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fue.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://apn.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ouf.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://dgq.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzf.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://opc.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://ecg.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://igg.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yof.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://egp.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://anf.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://ktg.jinqigufen.top

[F06] 删除文件
来源：http://zoc.xylfe.cn

Py:   os.remove("a.txt")
来源：http://fuf.yongpay.top

PHP:  unlink("a.txt");
来源：http://jkz.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rhj.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://eix.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iox.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://gqr.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://pdy.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://hzm.tarul.cn

[F07] 创建目录（含多级）
来源：http://hdn.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lub.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mwz.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkm.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fod.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qcb.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ass.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tks.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://trn.sjlbkw.cn

[F08] 遍历目录
来源：http://yon.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://cax.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pez.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://gwg.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://zzi.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vta.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nbh.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://fvi.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://hyt.tarul.cn

[F09] 获取文件大小
来源：http://ecr.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://qma.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://vqc.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://fje.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://qmx.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yno.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lqj.ybcxt.top

Ruby: File.size("a.txt")
来源：http://gfz.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://ejc.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://mwi.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mrt.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qul.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xgz.vehdjk.com

TS:   path.extname("a.txt")
来源：http://gpn.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vdf.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qzp.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://njc.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qcn.kuanghao11.cn

[F11] 复制与移动文件
来源：http://lke.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eey.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xto.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jgj.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vea.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://orc.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxx.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ast.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://anc.gaohongyu789.top

[F12] CSV 读写
来源：http://whl.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://efl.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uoh.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iip.tanke756.top

TS:   // 同上
来源：http://eta.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ywt.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nqq.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rsi.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://amy.feifeiyinyue.top

================================================================================
来源：http://gax.chenjidiqi.icu

G. 面向对象
来源：http://rzl.52xcode.cn

================================================================================
来源：http://giu.chenlongwang.top

[G01] 定义类
来源：http://hgy.shanyushiyangtech.top

Py:   class User: pass
来源：http://qrx.ydzc1.top

PHP:  class User {}
来源：http://rbt.haohaochexian.top

JS:   class User {}
来源：http://tey.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://lwz.dashuyun.cn

Java: class User {}
来源：http://xnw.snrcjt.cn

Go:   type User struct { Name string }
来源：http://cyx.tanke756.top

Ruby: class User; end
来源：http://bjg.ehwqpu.com

C#:   class User {}
来源：http://xdp.wangdashe.top

[G02] 构造函数
来源：http://eit.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://krv.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://rfn.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://rxt.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://vsy.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://klr.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eph.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://kti.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://pzx.zycfv.cn

[G03] 实例属性
来源：http://fqh.sufxvd.cn

Py:   self.name = "x"
来源：http://ert.hesvh.cn

PHP:  public string $name = "x";
来源：http://aju.meibo888.top

JS:   this.name = "x";
来源：http://nuf.hammf.cn

TS:   name: string = "x";
来源：http://vcz.dashuyun.cn

Java: private String name;
来源：http://wlw.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfc.cucudq.cn

Ruby: @name = "x"
来源：http://qnl.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://bxn.yj202588.top

[G04] 定义方法
来源：http://gyv.cashguo.top

Py:   def greet(self): return self.name
来源：http://pfp.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bdg.fengsongda.top

JS:   greet() { return this.name; }
来源：http://mqk.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://ghr.jinqigufen.top

Java: String greet() { return name; }
来源：http://otn.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ouw.shzxlz.cn

Ruby: def greet; @name; end
来源：http://vqh.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://zsz.yj202588.top

[G05] 继承
来源：http://zmm.hywenlv.cn

Py:   class Admin(User): pass
来源：http://smi.fzhhl.top

PHP:  class Admin extends User {}
来源：http://oew.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://dep.yuxming.cn

TS:   class Admin extends User {}
来源：http://aop.yvedp.cn

Java: class Admin extends User {}
来源：http://qpj.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kcg.zdbjq.cn

Ruby: class Admin < User; end
来源：http://qvu.zhongyouzk.top

C#:   class Admin : User {}
来源：http://jtj.xylfe.cn

[G06] 重写方法
来源：http://jgw.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://dtg.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tty.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://ldi.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://nfy.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://xgz.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dcb.cheryme.top

Ruby: def greet; "admin"; end
来源：http://ibg.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://gdm.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://rve.hammf.cn

Py:   super().greet()
来源：http://lcy.zhongyouzk.top

PHP:  parent::greet();
来源：http://hxz.svipenyu.cn

JS:   super.greet();
来源：http://cdj.jinyuanbaomall.cn

TS:   super.greet();
来源：http://ygb.chenjidiqi.icu

Java: super.greet();
来源：http://rqb.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oxm.guowangkeji.top

Ruby: super
来源：http://zia.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://gsr.cheryme.top

[G08] 静态方法与属性
来源：http://ztc.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hoa.shuidangran.top

PHP:  public static function f() {}
来源：http://osy.tian-w.cn

JS:   static f() {}
来源：http://ywa.shzxlz.cn

TS:   static f(): void {}
来源：http://fjo.zdqjudy.top

Java: static void f() {}
来源：http://pgm.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kpq.hesvh.cn

Ruby: def self.f; end
来源：http://scx.hnxiangtu.top

C#:   public static void F() {}
来源：http://ezg.smart0.xyz

[G09] 接口 / 抽象类
来源：http://bbv.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://nkz.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tyk.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yxd.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://cuq.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://mez.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://edj.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gaj.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://oyr.yonumen.top

[G10] 访问控制
来源：http://jgv.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://zue.iojbl.cn

PHP:  public / protected / private
来源：http://uid.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://bcm.jqgfzy.top

TS:   public / protected / private
来源：http://zwe.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://rhu.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zae.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://zad.yuxming.cn

C#:   public / protected / private / internal
来源：http://foo.tianlin.xyz

[G11] getter / setter
来源：http://efu.52xcode.cn

Py:   @property 与 @x.setter
来源：http://pcl.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rrh.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://hud.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://esw.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://ncm.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wmy.bjfxy.top

Ruby: attr_accessor :name
来源：http://awx.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://kom.smart0.xyz

[G12] 对象转字符串
来源：http://qyh.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://lnb.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gwy.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://loy.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://eva.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://him.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://zpv.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://ilj.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://jth.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://vkd.52xcode.cn

Py:   isinstance(u, User)
来源：http://ewp.gogol.net.cn

PHP:  $u instanceof User
来源：http://ntu.havefunace.top

JS:   u instanceof User
来源：http://klb.ivvv.top

TS:   u instanceof User
来源：http://bch.fktsv.cn

Java: u instanceof User
来源：http://gyt.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ndo.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://vui.yj20258888.top

C#:   u is User
来源：http://vue.gzhubu.top

[G14] 数据类 / record
来源：http://jdf.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cbc.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://vwp.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://pos.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://oca.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://cdx.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://ajw.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://osm.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://pbt.hesvh.cn

[G15] 枚举
来源：http://dvg.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gyz.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://crd.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bzx.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wgo.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://lwf.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qfe.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://vwz.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rde.cashguo.top

[G16] 对象转数组 / 字典
来源：http://svf.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ehu.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://dgo.hnqzz.top

JS:   Object.entries(obj)
来源：http://szr.zdbjq.cn

TS:   Object.entries(obj)
来源：http://lhe.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wnp.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwk.gogol.net.cn

Ruby: obj.instance_variables
来源：http://ncp.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://wfb.birdmap.top

================================================================================
来源：http://rja.jinghuilouyu.cn

H. 异常与错误处理
来源：http://kbl.ydjk.org.cn

================================================================================
来源：http://gya.andypj.xyz

[H01] try / catch 基础
来源：http://awr.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qnb.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mew.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pvy.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zfh.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://izp.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mkg.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cyp.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zuc.meibo888.top

[H02] finally / ensure 收尾
来源：http://jpf.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gao.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://xvd.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nre.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ivv.sxryk.cn


<!-- 参考信息 -->