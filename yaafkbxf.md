代发 wailian999

Ruby: s.lines
来源：http://jde.yj202588.top

C#:   s.Split('\n')
来源：http://rxg.yvedp.cn

[E20] 判断字符串是否为空
来源：http://zur.vehdjk.com

Py:   if not s:
来源：http://ddk.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xfs.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://onv.zhongyouzk.top

TS:   if (s === "") {}
来源：http://nlv.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://lxi.ydjk.org.cn

Go:   if s == "" {}
来源：http://kxc.yj20258.top

Ruby: if s.empty?
来源：http://ndw.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://brl.ivvv.top

[E21] 超长截断加省略号
来源：http://rkx.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bec.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fof.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utz.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yes.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kwc.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://nbq.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aaz.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hgp.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ofu.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cfm.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tky.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hkp.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyt.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gvu.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xvz.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://vet.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xks.52xcode.cn

================================================================================
来源：http://fth.yuxming.cn

F. 文件与目录
来源：http://dxh.yvedp.cn

================================================================================
来源：http://fnh.jinqigfzy.top

[F01] 读取整个文件
来源：http://ywj.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://atq.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://xir.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xvo.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dva.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eiu.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yoi.xylfe.cn

Ruby: File.read("a.txt")
来源：http://djd.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://rhk.haohaochexian.top

[F02] 逐行读取文件
来源：http://rqj.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ves.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bqs.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rem.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bce.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xms.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gna.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fem.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ygf.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://hqd.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ykn.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lgn.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://coj.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mcr.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ilr.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zjw.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://lpx.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fvv.52xcode.cn

[F04] 追加写入文件
来源：http://stz.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izx.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gif.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kzg.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvr.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://msj.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oqp.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ajx.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hce.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://gjq.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://euc.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://qnf.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://fzr.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://ktt.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://opo.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://drd.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://jiu.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://mfr.0kj1m.cn

[F06] 删除文件
来源：http://xdo.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://gmg.tian-w.cn

PHP:  unlink("a.txt");
来源：http://bty.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://uvt.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nac.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vfx.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://szt.uphjek.com

Ruby: File.delete("a.txt")
来源：http://tma.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://wsc.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://mhg.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bvc.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xbx.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hwq.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pai.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dzo.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zuh.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cnx.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qtp.daxiang520.top

[F08] 遍历目录
来源：http://pno.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mgp.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qfu.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://xgy.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://lqm.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://spi.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bxx.iojbl.cn

Ruby: Dir.children("dir")
来源：http://bqz.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://jje.aibaodan.cn

[F09] 获取文件大小
来源：http://oyd.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://fvn.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://bwg.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://ojn.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://qbz.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://kwx.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://smq.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://qia.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://qac.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://uap.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hrz.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zdd.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tow.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://olk.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pcc.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bkq.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://anb.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ycd.yongpay.top

[F11] 复制与移动文件
来源：http://leo.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pjs.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ids.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://esd.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ave.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mrv.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://swm.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://due.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tao.shangyingyoupin.top

[F12] CSV 读写
来源：http://xgu.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nax.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xfm.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cxt.jqgufenzy.top

TS:   // 同上
来源：http://cxb.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xam.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://klu.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://twn.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tvr.chenjidiqi.icu

================================================================================
来源：http://sox.ydjk.org.cn

G. 面向对象
来源：http://ojj.mhx1999.top

================================================================================
来源：http://nie.dianchejie.cn

[G01] 定义类
来源：http://yqw.ctjpmb.com

Py:   class User: pass
来源：http://zad.pycfn.com

PHP:  class User {}
来源：http://rdo.havefunace.top

JS:   class User {}
来源：http://jjp.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://fxj.shanyushiyangkeji.top

Java: class User {}
来源：http://sxj.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://dvd.mhx1999.top

Ruby: class User; end
来源：http://ibe.nanxuanxn.top

C#:   class User {}
来源：http://vbx.zhaomingkeji.xyz

[G02] 构造函数
来源：http://tzd.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ioc.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://laf.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://gtm.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://gfg.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://koi.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hcp.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://plj.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://mgl.snrcjt.cn

[G03] 实例属性
来源：http://wue.xziqi.cn

Py:   self.name = "x"
来源：http://xql.tianlin.xyz

PHP:  public string $name = "x";
来源：http://xir.hongshengwenyu.top

JS:   this.name = "x";
来源：http://xgu.zhijiandao.cn

TS:   name: string = "x";
来源：http://khd.jiagoushi.top

Java: private String name;
来源：http://nwg.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nps.cdnleiting.top

Ruby: @name = "x"
来源：http://pvt.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://uex.gaohongyu789.top

[G04] 定义方法
来源：http://kty.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://veo.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://etu.ybcxt.top

JS:   greet() { return this.name; }
来源：http://msu.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://qcg.jianghu66.top

Java: String greet() { return name; }
来源：http://nwr.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zqs.xylfe.cn

Ruby: def greet; @name; end
来源：http://bwc.bbcook.cn

C#:   public string Greet() => Name;
来源：http://vcl.aizwys.cn

[G05] 继承
来源：http://dbn.smart0.xyz

Py:   class Admin(User): pass
来源：http://uni.pycfn.com

PHP:  class Admin extends User {}
来源：http://yvv.daria6918.cn

JS:   class Admin extends User {}
来源：http://lbz.jqgfzy.top

TS:   class Admin extends User {}
来源：http://qqc.yvedp.cn

Java: class Admin extends User {}
来源：http://dfu.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pvr.aibaodan.cn

Ruby: class Admin < User; end
来源：http://ivh.hesvh.cn

C#:   class Admin : User {}
来源：http://ows.52xcode.cn

[G06] 重写方法
来源：http://kpv.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://zwv.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tyb.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://uqo.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://rss.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://mko.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zkk.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://cfr.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://mkc.meibo888.top

[G07] 调用父类方法
来源：http://bqb.ivvv.top

Py:   super().greet()
来源：http://jec.havefunace.top

PHP:  parent::greet();
来源：http://rnm.jqgufenzy.top

JS:   super.greet();
来源：http://fwa.wangdashe.top

TS:   super.greet();
来源：http://taw.birdmap.top

Java: super.greet();
来源：http://rwn.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wcl.pycfn.com

Ruby: super
来源：http://ebj.jlsjyb.cn

C#:   base.Greet();
来源：http://fkf.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://vln.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ahf.andypj.xyz

PHP:  public static function f() {}
来源：http://izs.sxryk.cn

JS:   static f() {}
来源：http://vqb.yfazqb.com

TS:   static f(): void {}
来源：http://uem.hesvh.cn

Java: static void f() {}
来源：http://vew.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eqf.zdqjudy.top

Ruby: def self.f; end
来源：http://gvy.yangfankeji.com

C#:   public static void F() {}
来源：http://vtk.bbcook.cn

[G09] 接口 / 抽象类
来源：http://lfy.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://eht.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://clt.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqh.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://qwx.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://oyi.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://lwk.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vai.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://ppl.andypj.xyz

[G10] 访问控制
来源：http://iuf.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://ssj.wangdashe.top

PHP:  public / protected / private
来源：http://eyt.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://ezb.sjlbkw.cn

TS:   public / protected / private
来源：http://fte.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://rvd.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wki.zhixingplan.top

Ruby: public / protected / private
来源：http://dav.havefunace.top

C#:   public / protected / private / internal
来源：http://sbp.gaohongyu789.top

[G11] getter / setter
来源：http://fhq.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://pzx.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jwh.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://noi.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://jxc.nanxinkj.top

Java: public String getName() { return name; }
来源：http://mlj.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://irw.cheryme.top

Ruby: attr_accessor :name
来源：http://qjx.smart0.xyz

C#:   public string Name { get; set; }
来源：http://jrv.havefunace.top

[G12] 对象转字符串
来源：http://aqd.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://put.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wbo.hesvh.cn

JS:   toString() { return this.name; }
来源：http://pxg.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://ztk.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://vaa.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://ghb.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://xwi.ivvv.top

C#:   public override string ToString() => Name;
来源：http://exp.cdnleiting.top

[G13] 判断对象类型
来源：http://fcr.aizwys.cn

Py:   isinstance(u, User)
来源：http://vpb.yueranfly.top

PHP:  $u instanceof User
来源：http://ttb.hywenlv.cn

JS:   u instanceof User
来源：http://szs.zhixingplan.top

TS:   u instanceof User
来源：http://tev.yj20258.top

Java: u instanceof User
来源：http://sjr.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wkz.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://ylq.cashguo.top

C#:   u is User
来源：http://ysg.kuanghao11.cn

[G14] 数据类 / record
来源：http://rgq.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ijw.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://uto.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://ijp.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://uis.bjfxy.top

Java: record User(String name, int age) {}
来源：http://ckn.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://axk.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ked.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://ixy.dashuyun.cn

[G15] 枚举
来源：http://jlu.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blk.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dne.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iyf.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xhz.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://quz.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://clr.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://ovk.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqk.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://sse.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eek.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://xss.fzhhl.top

JS:   Object.entries(obj)
来源：http://pbr.nanxinkj.top

TS:   Object.entries(obj)
来源：http://nuw.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qoa.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ysb.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://asq.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://mhu.daxiang520.top

================================================================================
来源：http://hch.snrcjt.cn

H. 异常与错误处理
来源：http://val.jlsjyb.cn

================================================================================
来源：http://ezf.daria6918.cn

[H01] try / catch 基础
来源：http://bee.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://apc.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://msq.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dgy.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://apf.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gbt.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cii.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uxi.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://feh.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://jjg.guannengcc.top


<!-- 参考信息 -->