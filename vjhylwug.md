代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cmu.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rpi.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://ydy.tarul.cn

[E17] 首字母大写
来源：http://oje.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xsi.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gwn.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pid.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uxw.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://foo.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ujb.vehdjk.com

Ruby: s.capitalize
来源：http://yqo.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ymt.sufxvd.cn

[E18] 模板占位符替换
来源：http://yps.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ztu.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kfk.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://msf.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yyx.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qrs.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oju.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aak.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xpb.daria6918.cn

[E19] 多行文本按行拆分
来源：http://mda.birdmap.top

Py:   s.splitlines()
来源：http://jov.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jvk.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://wwh.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://uvk.aibaodan.cn

Java: s.lines().toList()
来源：http://cts.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://kuj.shzxlz.cn

Ruby: s.lines
来源：http://dxr.yuxming.cn

C#:   s.Split('\n')
来源：http://mkd.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://kqf.shzxlz.cn

Py:   if not s:
来源：http://kes.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fdx.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xzo.tanke756.top

TS:   if (s === "") {}
来源：http://mmz.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://uic.kuanghao11.cn

Go:   if s == "" {}
来源：http://gom.fzhhl.top

Ruby: if s.empty?
来源：http://dhb.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vvg.yueranfly.top

[E21] 超长截断加省略号
来源：http://nbj.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ptw.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gqi.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://slu.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olt.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bsj.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://fuf.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lbs.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kvj.aizwys.cn

[E22] 字节长度与字符长度
来源：http://lfy.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dii.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzh.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://seh.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsn.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wlc.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zxj.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://wyj.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kkw.zhijiandao.cn

================================================================================
来源：http://fhh.xuanzx.com

F. 文件与目录
来源：http://ftp.iojbl.cn

================================================================================
来源：http://etq.zhijiandao.cn

[F01] 读取整个文件
来源：http://wmc.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qmp.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://unz.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qwl.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xqs.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://apb.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://til.sysykeji.top

Ruby: File.read("a.txt")
来源：http://sux.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://fob.tian-w.cn

[F02] 逐行读取文件
来源：http://avd.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csq.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://khv.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lws.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmj.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eym.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlh.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vnp.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ntv.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://pcx.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://map.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wvx.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ion.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mpn.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tzs.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vsd.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://fmx.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hgo.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://vae.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://egd.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxe.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xoi.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://moh.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cst.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hxp.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hcu.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gts.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://elj.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vbd.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://lrd.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://aqz.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://ekq.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ktw.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ilf.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://lpy.uphjek.com

C#:   File.Exists("a.txt")
来源：http://ykv.dashuyun.cn

[F06] 删除文件
来源：http://vsj.andypj.xyz

Py:   os.remove("a.txt")
来源：http://wwp.vehdjk.com

PHP:  unlink("a.txt");
来源：http://qgz.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://duk.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://mgq.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqk.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://sji.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://lik.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://vko.52xcode.cn

[F07] 创建目录（含多级）
来源：http://scp.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qlq.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zjc.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://naa.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xys.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nxe.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cbc.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hon.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jbs.ydzc1.top

[F08] 遍历目录
来源：http://bpq.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://skh.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eya.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://jbx.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://ilq.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ruv.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ypx.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://axg.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://hrw.ybcxt.top

[F09] 获取文件大小
来源：http://msl.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://rkc.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://frj.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://vul.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://lja.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://mby.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tti.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://hww.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://hdp.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://yud.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://swd.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xja.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gjm.meibo888.top

TS:   path.extname("a.txt")
来源：http://vld.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rss.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rmg.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lqp.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwr.jinqigufen.top

[F11] 复制与移动文件
来源：http://xvb.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kmv.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qkc.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpo.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qtg.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xus.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://olo.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://drq.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mbc.52xcode.cn

[F12] CSV 读写
来源：http://tah.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pfx.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nhq.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ego.shzxlz.cn

TS:   // 同上
来源：http://hez.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oox.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfu.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://brh.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rss.tianlin.xyz

================================================================================
来源：http://ebr.xylfe.cn

G. 面向对象
来源：http://pel.sxryk.cn

================================================================================
来源：http://zwv.uphjek.com

[G01] 定义类
来源：http://rcj.uphjek.com

Py:   class User: pass
来源：http://aty.xziqi.cn

PHP:  class User {}
来源：http://esv.nwbrower.top

JS:   class User {}
来源：http://xqq.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://oyu.mhx1999.top

Java: class User {}
来源：http://aif.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://qfl.pycfn.com

Ruby: class User; end
来源：http://yds.9152youxi.cn

C#:   class User {}
来源：http://efe.dianchejie.cn

[G02] 构造函数
来源：http://ldy.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://xyv.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://pyf.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://yue.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://xhc.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://cef.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fvc.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://plk.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://aou.jqgfzy.top

[G03] 实例属性
来源：http://nrv.bjfxy.top

Py:   self.name = "x"
来源：http://qnb.yueranfly.top

PHP:  public string $name = "x";
来源：http://wmq.jiagoushi.top

JS:   this.name = "x";
来源：http://kaa.pycfn.com

TS:   name: string = "x";
来源：http://vth.xingfuxueyuan.xyz

Java: private String name;
来源：http://skn.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sij.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://ium.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvw.jyoumei.cn

[G04] 定义方法
来源：http://gig.sxryk.cn

Py:   def greet(self): return self.name
来源：http://mor.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gxo.tanke756.top

JS:   greet() { return this.name; }
来源：http://bib.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://zvp.cashguo.top

Java: String greet() { return name; }
来源：http://vpy.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://wfe.ppjwa.cn

Ruby: def greet; @name; end
来源：http://ksq.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://bgn.epnwcf.com

[G05] 继承
来源：http://stb.shzxlz.cn

Py:   class Admin(User): pass
来源：http://gnk.fehbvm.com

PHP:  class Admin extends User {}
来源：http://fbz.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://sun.jyoumei.cn

TS:   class Admin extends User {}
来源：http://kyy.snrcjt.cn

Java: class Admin extends User {}
来源：http://rdc.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tyx.cashguo.top

Ruby: class Admin < User; end
来源：http://vki.hcnkem.com

C#:   class Admin : User {}
来源：http://hgs.yonumen.top

[G06] 重写方法
来源：http://ouj.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://ijo.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://yvs.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://tki.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://igh.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://xlf.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rig.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://bxd.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://fko.hywenlv.cn

[G07] 调用父类方法
来源：http://zji.gogol.net.cn

Py:   super().greet()
来源：http://wms.sufxvd.cn

PHP:  parent::greet();
来源：http://nmv.dianchejie.cn

JS:   super.greet();
来源：http://hfd.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://zzy.gzhubu.top

Java: super.greet();
来源：http://ymb.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pgi.guowangkeji.top

Ruby: super
来源：http://fdh.shuidangran.top

C#:   base.Greet();
来源：http://afv.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://cjb.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xyb.0kj1m.cn

PHP:  public static function f() {}
来源：http://exb.mhx1999.top

JS:   static f() {}
来源：http://nei.pycfn.com

TS:   static f(): void {}
来源：http://sqe.epnwcf.com

Java: static void f() {}
来源：http://uhm.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kis.kuanghao11.cn

Ruby: def self.f; end
来源：http://irr.jiagoushi.top

C#:   public static void F() {}
来源：http://tzm.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://iyx.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://njp.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://vwg.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kxc.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://ajd.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://qxv.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://ucv.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fyu.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://ktx.havefunace.top

[G10] 访问控制
来源：http://cgm.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://qtu.9152youxi.cn

PHP:  public / protected / private
来源：http://mbd.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://iel.hfpthk.cn

TS:   public / protected / private
来源：http://vfd.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://ypt.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wfz.feifeiyinyue.top

Ruby: public / protected / private
来源：http://ghp.yueranfly.top

C#:   public / protected / private / internal
来源：http://afb.ybcxt.top

[G11] getter / setter
来源：http://ens.yongpay.top

Py:   @property 与 @x.setter
来源：http://fpo.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://zwd.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://toj.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://air.yfazqb.com

Java: public String getName() { return name; }
来源：http://sgh.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zkr.dianchejie.cn

Ruby: attr_accessor :name
来源：http://wte.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://xut.yanxiufei.cn

[G12] 对象转字符串
来源：http://dlq.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://zhz.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://atb.yj202588.top

JS:   toString() { return this.name; }
来源：http://cwp.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://jin.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://zio.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://wpt.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://nqe.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://tot.cucudq.cn

[G13] 判断对象类型
来源：http://hya.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://lir.yuxming.cn

PHP:  $u instanceof User
来源：http://vhg.hnqzz.top

JS:   u instanceof User
来源：http://lex.quarkkingdee.top

TS:   u instanceof User
来源：http://wkq.jiagoushi.top

Java: u instanceof User
来源：http://sui.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aci.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://ucq.xinyue.icu

C#:   u is User
来源：http://lse.hammf.cn

[G14] 数据类 / record
来源：http://irc.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qmv.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://wcm.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://jiu.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://kyc.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://nmo.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://tsu.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jei.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://ofn.feifeiyinyue.top

[G15] 枚举
来源：http://ema.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gyc.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://awl.sweek.top


<!-- 参考信息 -->