代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gam.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hwy.haohaochexian.top

[E16] 数字千分位
来源：http://vmq.hammf.cn

Py:   f"{1234567:,}"
来源：http://egj.yuanzhike.top

PHP:  number_format(1234567);
来源：http://ydq.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://tui.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://giq.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddw.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yqx.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vqs.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://vqw.jianghu66.top

[E17] 首字母大写
来源：http://gtv.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nxq.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mbb.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsz.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qyu.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aeq.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://obv.yfazqb.com

Ruby: s.capitalize
来源：http://ucb.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mgz.birdmap.top

[E18] 模板占位符替换
来源：http://fkq.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vyf.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tbr.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bsl.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kmb.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://trd.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gip.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://goc.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zud.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://pqb.gzhubu.top

Py:   s.splitlines()
来源：http://eiz.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fyz.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://upg.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://rsy.0kj1m.cn

Java: s.lines().toList()
来源：http://tlr.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://alw.zdbjq.cn

Ruby: s.lines
来源：http://kav.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://xzl.aizwys.cn

[E20] 判断字符串是否为空
来源：http://kuh.sysykeji.top

Py:   if not s:
来源：http://ilm.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iar.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://slo.chenlongwang.top

TS:   if (s === "") {}
来源：http://tka.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://ouq.sjlbkw.cn

Go:   if s == "" {}
来源：http://wbf.yj20258.top

Ruby: if s.empty?
来源：http://nsx.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ypi.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://gxc.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hhl.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kzl.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agg.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gxq.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mji.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://pvi.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rqc.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hni.gzhubu.top

[E22] 字节长度与字符长度
来源：http://vpz.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ngr.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vle.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bar.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqk.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zcp.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wky.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://tvt.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lnb.ydjk.org.cn

================================================================================
来源：http://nky.cqqwz.cn

F. 文件与目录
来源：http://ivs.jinyuanbaomall.cn

================================================================================
来源：http://cvn.quarkkingdee.top

[F01] 读取整个文件
来源：http://cje.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxv.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://ouz.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://chl.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yic.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jcm.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hjw.smart0.xyz

Ruby: File.read("a.txt")
来源：http://afy.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://jix.shangyingyoupin.top

[F02] 逐行读取文件
来源：http://wyw.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wfs.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oxy.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgl.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgv.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vbj.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hvq.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mnk.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyx.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://aks.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmb.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://soa.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwy.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tdm.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://usd.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ihh.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qpe.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qgt.hammf.cn

[F04] 追加写入文件
来源：http://hfk.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://exx.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://skg.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dio.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://opc.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://udr.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://llh.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uxb.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mvi.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://ayn.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tcs.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://yzi.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://jxz.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://ezj.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mnv.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zhx.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://iho.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://lmw.yanxiufei.cn

[F06] 删除文件
来源：http://yvl.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://bvo.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://coi.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://pnq.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bna.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jrd.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://mkq.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://hhx.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://pfv.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://wun.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mjf.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mtl.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vjt.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xiq.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ywv.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ffu.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cbx.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://usg.hysaishi.cn

[F08] 遍历目录
来源：http://toy.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://byg.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gve.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://ltf.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://bzr.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cge.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dai.jianghu66.top

Ruby: Dir.children("dir")
来源：http://wdz.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://fnk.feifeiyinyue.top

[F09] 获取文件大小
来源：http://fnp.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://lgb.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://icu.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://wrp.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://lkj.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jsa.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://otj.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://hxs.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kwn.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://okq.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tcd.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vdb.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mqr.sxryk.cn

TS:   path.extname("a.txt")
来源：http://mpa.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hoq.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ckp.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ypn.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://igg.zhixingplan.top

[F11] 复制与移动文件
来源：http://ydx.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fvl.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lgp.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://srp.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twc.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ktp.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://guy.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://apt.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://poh.feifeiyinyue.top

[F12] CSV 读写
来源：http://fee.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mwg.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lcl.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://exp.jinqigufen.top

TS:   // 同上
来源：http://blh.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fwe.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xbu.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xjm.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yhx.tian-w.cn

================================================================================
来源：http://yhc.sysykeji.top

G. 面向对象
来源：http://ygd.ydzc1.top

================================================================================
来源：http://tmm.yuanzhike.top

[G01] 定义类
来源：http://rap.sufxvd.cn

Py:   class User: pass
来源：http://jwv.daxiang520.top

PHP:  class User {}
来源：http://etv.ybcxt.top

JS:   class User {}
来源：http://hts.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://qju.andypj.xyz

Java: class User {}
来源：http://vbv.dashuyun.cn

Go:   type User struct { Name string }
来源：http://kjc.zhaomingkeji.xyz

Ruby: class User; end
来源：http://ree.jianghu66.top

C#:   class User {}
来源：http://udg.jyoumei.cn

[G02] 构造函数
来源：http://cwz.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://dxz.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://aqb.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://zah.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://rqb.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://zph.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://amk.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://efw.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://wwv.xylfe.cn

[G03] 实例属性
来源：http://zsu.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://hml.chenzaomai.com

PHP:  public string $name = "x";
来源：http://jig.yonumen.top

JS:   this.name = "x";
来源：http://qjo.zdqjudy.top

TS:   name: string = "x";
来源：http://gym.smart0.xyz

Java: private String name;
来源：http://rdr.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qww.fengsongda.top

Ruby: @name = "x"
来源：http://fah.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://nrm.shzxlz.cn

[G04] 定义方法
来源：http://znx.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://nqp.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qxq.fengsongda.top

JS:   greet() { return this.name; }
来源：http://frk.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://bgf.zhixingplan.top

Java: String greet() { return name; }
来源：http://jrh.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lpb.hammf.cn

Ruby: def greet; @name; end
来源：http://tyg.sxryk.cn

C#:   public string Greet() => Name;
来源：http://fhn.cqqwz.cn

[G05] 继承
来源：http://bok.cucudq.cn

Py:   class Admin(User): pass
来源：http://mfb.vehdjk.com

PHP:  class Admin extends User {}
来源：http://icq.fktsv.cn

JS:   class Admin extends User {}
来源：http://tjb.haohaochexian.top

TS:   class Admin extends User {}
来源：http://hia.zhongyouzk.top

Java: class Admin extends User {}
来源：http://fsq.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cii.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://fya.ctjpmb.com

C#:   class Admin : User {}
来源：http://kvs.hcnkem.com

[G06] 重写方法
来源：http://wpb.havefunace.top

Py:   def greet(self): return "admin"
来源：http://ljp.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://urk.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://exx.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://ubw.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://tgs.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lhx.yongpay.top

Ruby: def greet; "admin"; end
来源：http://asc.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://lra.chenlongwang.top

[G07] 调用父类方法
来源：http://hee.guannengcc.top

Py:   super().greet()
来源：http://omf.cheryme.top

PHP:  parent::greet();
来源：http://tqu.zycfv.cn

JS:   super.greet();
来源：http://gxa.birdmap.top

TS:   super.greet();
来源：http://bps.hesvh.cn

Java: super.greet();
来源：http://sud.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dyo.yonumen.top

Ruby: super
来源：http://xht.hnxiangtu.top

C#:   base.Greet();
来源：http://vzd.smart0.xyz

[G08] 静态方法与属性
来源：http://bjs.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hwc.daxiang520.top

PHP:  public static function f() {}
来源：http://fsi.smart0.xyz

JS:   static f() {}
来源：http://uzd.gotoacloud.top

TS:   static f(): void {}
来源：http://byq.vehdjk.com

Java: static void f() {}
来源：http://ztl.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aom.birdmap.top

Ruby: def self.f; end
来源：http://rzs.smart0.xyz

C#:   public static void F() {}
来源：http://ukp.sysykeji.top

[G09] 接口 / 抽象类
来源：http://aec.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://gqh.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://jnk.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://egu.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://nes.c1oappe.top

Java: interface Shape { double area(); }
来源：http://hgp.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://oqt.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xdy.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://hus.ydzc1.top

[G10] 访问控制
来源：http://awq.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://ypq.guannengcc.top

PHP:  public / protected / private
来源：http://mfv.smart0.xyz

JS:   #private 字段；其余公开
来源：http://ukh.yj202588.top

TS:   public / protected / private
来源：http://vif.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://fzh.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kds.chenjidiqi.icu

Ruby: public / protected / private
来源：http://lam.sweek.top

C#:   public / protected / private / internal
来源：http://edn.yj20258888.top

[G11] getter / setter
来源：http://ezr.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://lrz.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://gep.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://lmr.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://yko.vehdjk.com

Java: public String getName() { return name; }
来源：http://hci.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oxd.chenzaomai.com

Ruby: attr_accessor :name
来源：http://mef.ydzc1.top

C#:   public string Name { get; set; }
来源：http://nwg.chenjidiqi.icu

[G12] 对象转字符串
来源：http://jjw.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://vvq.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gcj.xuanzx.com

JS:   toString() { return this.name; }
来源：http://fkq.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://xuu.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://mff.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hql.ivvv.top

Ruby: def to_s; @name; end
来源：http://zky.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://otx.zhoulong.xyz

[G13] 判断对象类型
来源：http://ksg.svipenyu.cn

Py:   isinstance(u, User)
来源：http://pph.fengsongda.top

PHP:  $u instanceof User
来源：http://vbo.ppjwa.cn

JS:   u instanceof User
来源：http://kzx.daxiang520.top

TS:   u instanceof User
来源：http://nkb.snrcjt.cn

Java: u instanceof User
来源：http://emd.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ghg.sysykeji.top

Ruby: u.is_a?(User)
来源：http://xvb.yfazqb.com

C#:   u is User
来源：http://ekv.quarkkingdee.top

[G14] 数据类 / record
来源：http://oiu.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qjq.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://zmx.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qlh.shzxlz.cn


<!-- 参考信息 -->