代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vdq.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zsz.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jom.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qlw.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gqx.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bzl.andypj.xyz

Ruby: s.capitalize
来源：http://qbk.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ane.tanke756.top

[E18] 模板占位符替换
来源：http://aan.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uev.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://alk.sweek.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ouj.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jza.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mig.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ckz.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zbp.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ctx.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://vny.cdnleiting.top

Py:   s.splitlines()
来源：http://fyz.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lcm.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://nya.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://ftl.hesvh.cn

Java: s.lines().toList()
来源：http://fcq.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://prf.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://ise.pycfn.com

C#:   s.Split('\n')
来源：http://qdq.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://ffp.aizwys.cn

Py:   if not s:
来源：http://oca.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cjo.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jft.52xcode.cn

TS:   if (s === "") {}
来源：http://zou.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://occ.guannengcc.top

Go:   if s == "" {}
来源：http://ija.ctjpmb.com

Ruby: if s.empty?
来源：http://ixk.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mln.9152youxi.cn

[E21] 超长截断加省略号
来源：http://tmg.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zub.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mwf.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zil.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eak.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ypb.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://xgz.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbw.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dxk.aizwys.cn

[E22] 字节长度与字符长度
来源：http://qzm.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wkk.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ilm.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mza.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rof.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jyl.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kuc.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://pib.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dme.hesvh.cn

================================================================================
来源：http://aqy.vehdjk.com

F. 文件与目录
来源：http://feq.shangyingyoupin.top

================================================================================
来源：http://yjn.yangfankeji.com

[F01] 读取整个文件
来源：http://ali.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oce.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://vmc.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gfu.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kaw.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://npb.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uio.wangdashe.top

Ruby: File.read("a.txt")
来源：http://xtc.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://tsw.gogol.net.cn

[F02] 逐行读取文件
来源：http://qwc.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lgh.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dll.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kex.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ipx.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lyn.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://njn.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qzr.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmy.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://unw.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://slx.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wut.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://apn.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rzb.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bob.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lka.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://wef.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vxc.uphjek.com

[F04] 追加写入文件
来源：http://dcf.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pxx.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fdz.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ghk.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://psq.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nlu.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vqg.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tsl.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rmw.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://lqd.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iim.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://dgt.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://hys.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://qtp.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iwx.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cks.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://oix.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://tbx.epnwcf.com

[F06] 删除文件
来源：http://was.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://fxd.bjfxy.top

PHP:  unlink("a.txt");
来源：http://xnk.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vwm.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oke.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kmo.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://grw.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://sgh.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://fup.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://imj.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nby.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mli.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsz.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zig.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ciy.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://djv.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ofm.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hsq.epnwcf.com

[F08] 遍历目录
来源：http://kci.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xuj.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vur.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://mkc.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://hfc.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pqt.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://afb.cashguo.top

Ruby: Dir.children("dir")
来源：http://rsr.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://zjx.jiagoushi.top

[F09] 获取文件大小
来源：http://qgp.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://ehu.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://yqh.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://fsd.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://vkf.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pea.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jco.havefunace.top

Ruby: File.size("a.txt")
来源：http://tni.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://vkv.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://yhc.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xjw.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dbg.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ekm.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://kiy.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gtl.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://szz.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pqr.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dlt.pycfn.com

[F11] 复制与移动文件
来源：http://iam.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lar.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cru.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dha.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vpa.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ire.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wex.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lsx.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://owh.cashguo.top

[F12] CSV 读写
来源：http://gao.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eor.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wdn.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://igc.zycfv.cn

TS:   // 同上
来源：http://uby.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mdc.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sye.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ovk.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tex.jyoumei.cn

================================================================================
来源：http://slk.nanxinkj.top

G. 面向对象
来源：http://age.andypj.xyz

================================================================================
来源：http://rfu.jinghuilouyu.cn

[G01] 定义类
来源：http://qwb.vehdjk.com

Py:   class User: pass
来源：http://nde.xziqi.cn

PHP:  class User {}
来源：http://ymv.yj20258.top

JS:   class User {}
来源：http://flf.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://hyt.tianlin.xyz

Java: class User {}
来源：http://geq.cheryme.top

Go:   type User struct { Name string }
来源：http://qwa.jinghuilouyu.cn

Ruby: class User; end
来源：http://npk.316326.xyz

C#:   class User {}
来源：http://mmk.pycfn.com

[G02] 构造函数
来源：http://rex.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rlo.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://ieq.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://sdn.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://nsb.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://xzx.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hdx.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://gtb.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://mbe.52xcode.cn

[G03] 实例属性
来源：http://zvv.hnxiangtu.top

Py:   self.name = "x"
来源：http://dfy.ybcxt.top

PHP:  public string $name = "x";
来源：http://oxw.ehwqpu.com

JS:   this.name = "x";
来源：http://lgx.xinyue.icu

TS:   name: string = "x";
来源：http://dkj.jinqigufen.top

Java: private String name;
来源：http://ijs.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wqb.snrcjt.cn

Ruby: @name = "x"
来源：http://ezm.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://yod.xuanzx.com

[G04] 定义方法
来源：http://vue.birdmap.top

Py:   def greet(self): return self.name
来源：http://ngs.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mvw.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://zmw.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://qmc.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://sdn.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pcj.tian-w.cn

Ruby: def greet; @name; end
来源：http://oiq.hammf.cn

C#:   public string Greet() => Name;
来源：http://sdv.zhaomingkeji.xyz

[G05] 继承
来源：http://khh.zdbjq.cn

Py:   class Admin(User): pass
来源：http://pid.yueranfly.top

PHP:  class Admin extends User {}
来源：http://yap.jiagoushi.top

JS:   class Admin extends User {}
来源：http://mgy.bbcook.cn

TS:   class Admin extends User {}
来源：http://leh.aizwys.cn

Java: class Admin extends User {}
来源：http://lot.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hbq.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://wrs.snrcjt.cn

C#:   class Admin : User {}
来源：http://agm.ydzc1.top

[G06] 重写方法
来源：http://oiz.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://zgv.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aoo.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://cdt.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://hyn.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://cmu.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://azz.yonumen.top

Ruby: def greet; "admin"; end
来源：http://fxl.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://gsn.pengpengdd.cyou

[G07] 调用父类方法
来源：http://gma.aizwys.cn

Py:   super().greet()
来源：http://tzk.sysykeji.top

PHP:  parent::greet();
来源：http://slr.jyoumei.cn

JS:   super.greet();
来源：http://dxt.jiagoushi.top

TS:   super.greet();
来源：http://dhh.hammf.cn

Java: super.greet();
来源：http://ojh.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://frm.tarul.cn

Ruby: super
来源：http://sdi.yuanzhike.top

C#:   base.Greet();
来源：http://qmk.birdmap.top

[G08] 静态方法与属性
来源：http://yug.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tfs.cucudq.cn

PHP:  public static function f() {}
来源：http://ujv.mhx1999.top

JS:   static f() {}
来源：http://eon.andypj.xyz

TS:   static f(): void {}
来源：http://swi.ywan-chungtsiang.top

Java: static void f() {}
来源：http://ibq.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qek.hcnkem.com

Ruby: def self.f; end
来源：http://lxr.guowangkeji.top

C#:   public static void F() {}
来源：http://bok.yj20258.top

[G09] 接口 / 抽象类
来源：http://vpc.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://bgx.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://xld.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://whu.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://dhu.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://jel.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://ntb.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mpk.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://tot.cashguo.top

[G10] 访问控制
来源：http://aeu.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://cwo.xinyue.icu

PHP:  public / protected / private
来源：http://iif.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://yti.yuanzhike.top

TS:   public / protected / private
来源：http://qpo.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://olo.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dvz.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://oyw.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://wbg.tanke756.top

[G11] getter / setter
来源：http://tbx.bbcook.cn

Py:   @property 与 @x.setter
来源：http://hqo.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://szy.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://mkl.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://oom.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://fiv.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tyv.aibaodan.cn

Ruby: attr_accessor :name
来源：http://svl.52xcode.cn

C#:   public string Name { get; set; }
来源：http://ndp.mhx1999.top

[G12] 对象转字符串
来源：http://qiu.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://ccq.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xcn.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://elq.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://ycn.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://ijh.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://blu.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://xql.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://vas.sxryk.cn

[G13] 判断对象类型
来源：http://kzt.gzhubu.top

Py:   isinstance(u, User)
来源：http://cen.sjlbkw.cn

PHP:  $u instanceof User
来源：http://pxe.cashguo.top

JS:   u instanceof User
来源：http://luo.ydzc1.top

TS:   u instanceof User
来源：http://wdl.tanke756.top

Java: u instanceof User
来源：http://twh.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yxp.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://gis.sysykeji.top

C#:   u is User
来源：http://ytc.aizwys.cn

[G14] 数据类 / record
来源：http://dfb.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nxw.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://oah.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://onk.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://jzx.yueranfly.top

Java: record User(String name, int age) {}
来源：http://uyr.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://woo.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kul.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://jyo.sweek.top

[G15] 枚举
来源：http://nfe.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ylp.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kiq.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cdy.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bfn.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://mgo.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgv.jianghu66.top


<!-- 参考信息 -->