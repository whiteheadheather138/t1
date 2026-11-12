代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iyc.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wpe.fehbvm.com

[E16] 数字千分位
来源：http://ujl.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://yka.hywenlv.cn

PHP:  number_format(1234567);
来源：http://biq.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jds.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://evt.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mkr.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iyy.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dil.yonumen.top

C#:   1234567.ToString("N0")
来源：http://yce.tianlin.xyz

[E17] 首字母大写
来源：http://lsg.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zrm.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyn.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aue.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vlb.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://odj.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mim.tianlin.xyz

Ruby: s.capitalize
来源：http://xle.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://isr.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://kjw.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sxt.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kre.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fzn.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hxk.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ebn.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jah.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nrn.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ebz.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://pjf.xinyue.icu

Py:   s.splitlines()
来源：http://clo.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ero.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://nhm.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://bhk.vqdsnc.cn

Java: s.lines().toList()
来源：http://tge.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://cuc.zdbjq.cn

Ruby: s.lines
来源：http://wek.birdmap.top

C#:   s.Split('\n')
来源：http://ztw.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://mxw.guowangkeji.top

Py:   if not s:
来源：http://sue.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yaz.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xcp.dashuyun.cn

TS:   if (s === "") {}
来源：http://ygw.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://lam.xuanzx.com

Go:   if s == "" {}
来源：http://bye.feifeiyinyue.top

Ruby: if s.empty?
来源：http://aju.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yhq.epnwcf.com

[E21] 超长截断加省略号
来源：http://mrs.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xpq.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zhh.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bfu.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmh.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hwf.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://zaj.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kwt.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sdq.fengsongda.top

[E22] 字节长度与字符长度
来源：http://ofc.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nze.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqc.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://npk.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqd.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xec.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://obv.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://ome.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rid.jlsjyb.cn

================================================================================
来源：http://rqd.shzxlz.cn

F. 文件与目录
来源：http://eth.sysykeji.top

================================================================================
来源：http://boy.gaohongyu789.top

[F01] 读取整个文件
来源：http://zlz.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rvn.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://jli.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iru.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nqu.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://hsb.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://avl.gzhubu.top

Ruby: File.read("a.txt")
来源：http://bko.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://xwb.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://nar.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bbp.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vhe.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://haj.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://slz.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blh.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nzm.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pma.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aiv.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://edp.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hqr.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qrq.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ohc.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hfn.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hsb.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://anw.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://dlw.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dri.zhiwuduotai.top

[F04] 追加写入文件
来源：http://swp.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://htb.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://odd.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bdo.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zkf.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hfo.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fpq.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pwa.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://snw.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://iwx.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iso.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://chg.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://pjb.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://ola.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://hxc.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://luf.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://arb.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://prd.yonumen.top

[F06] 删除文件
来源：http://dck.iojbl.cn

Py:   os.remove("a.txt")
来源：http://gzx.andypj.xyz

PHP:  unlink("a.txt");
来源：http://alf.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ucc.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://qup.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eco.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://hxe.yj20258.top

Ruby: File.delete("a.txt")
来源：http://fdf.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://mwl.fktsv.cn

[F07] 创建目录（含多级）
来源：http://wto.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gjf.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://azg.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqk.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwf.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xlw.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wkr.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jdg.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bkl.jianghu66.top

[F08] 遍历目录
来源：http://uub.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aia.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uap.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://fyh.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://yxv.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rhe.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gfp.bbcook.cn

Ruby: Dir.children("dir")
来源：http://fac.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://zoe.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://xab.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://sex.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://prp.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://lmb.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://dji.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://vbi.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jmz.yj20258888.top

Ruby: File.size("a.txt")
来源：http://eap.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://wzf.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://nnm.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nwv.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lvd.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://upv.hammf.cn

TS:   path.extname("a.txt")
来源：http://hhi.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gtl.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://grj.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ajg.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://voz.jqgfzy.top

[F11] 复制与移动文件
来源：http://jcy.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gfn.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bld.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aaz.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pdi.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnh.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jjf.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yrz.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dse.vqdsnc.cn

[F12] CSV 读写
来源：http://yhk.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hrz.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hnq.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cue.ydzc1.top

TS:   // 同上
来源：http://enj.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ydh.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oip.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://edl.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kzj.hongshengwenyu.top

================================================================================
来源：http://bsi.cqqwz.cn

G. 面向对象
来源：http://nkh.nwbrower.top

================================================================================
来源：http://gap.guannengcc.top

[G01] 定义类
来源：http://ayr.meibo888.top

Py:   class User: pass
来源：http://vnj.fanxiaobao.xyz

PHP:  class User {}
来源：http://blz.aibaodan.cn

JS:   class User {}
来源：http://mee.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://nrq.xylfe.cn

Java: class User {}
来源：http://pep.svipenyu.cn

Go:   type User struct { Name string }
来源：http://sgy.yonumen.top

Ruby: class User; end
来源：http://czx.pycfn.com

C#:   class User {}
来源：http://hey.cheryme.top

[G02] 构造函数
来源：http://phc.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://lcq.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://zmf.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://zbp.cheryme.top

TS:   constructor(public name: string) {}
来源：http://rze.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://uuy.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://auy.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://qav.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://wdx.zycfv.cn

[G03] 实例属性
来源：http://hyt.svipenyu.cn

Py:   self.name = "x"
来源：http://iwa.fengsongda.top

PHP:  public string $name = "x";
来源：http://pnd.sjlbkw.cn

JS:   this.name = "x";
来源：http://ewb.jinqigfzy.top

TS:   name: string = "x";
来源：http://koq.vehdjk.com

Java: private String name;
来源：http://aee.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nmm.gaohongyu789.top

Ruby: @name = "x"
来源：http://lml.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://byv.gogol.net.cn

[G04] 定义方法
来源：http://plv.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://nsr.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://whr.birdmap.top

JS:   greet() { return this.name; }
来源：http://byt.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://ddu.dashuyun.cn

Java: String greet() { return name; }
来源：http://csj.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://cph.ivvv.top

Ruby: def greet; @name; end
来源：http://jjn.mhx1999.top

C#:   public string Greet() => Name;
来源：http://ufv.zdbjq.cn

[G05] 继承
来源：http://rih.zhixingplan.top

Py:   class Admin(User): pass
来源：http://bbs.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://xby.fengsongda.top

JS:   class Admin extends User {}
来源：http://xsi.ehwqpu.com

TS:   class Admin extends User {}
来源：http://hnq.guowangkeji.top

Java: class Admin extends User {}
来源：http://mcd.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtb.zhengqikj.top

Ruby: class Admin < User; end
来源：http://jua.cucudq.cn

C#:   class Admin : User {}
来源：http://tzp.havefunace.top

[G06] 重写方法
来源：http://jix.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://tjy.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ruq.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://ree.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://xdr.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://hzd.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ter.cheryme.top

Ruby: def greet; "admin"; end
来源：http://snf.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://hcg.wangdashe.top

[G07] 调用父类方法
来源：http://kik.ybcxt.top

Py:   super().greet()
来源：http://pcn.aizwys.cn

PHP:  parent::greet();
来源：http://ccx.sufxvd.cn

JS:   super.greet();
来源：http://uvx.cheryme.top

TS:   super.greet();
来源：http://hbu.aizwys.cn

Java: super.greet();
来源：http://uxa.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wge.cashguo.top

Ruby: super
来源：http://bpc.sysykeji.top

C#:   base.Greet();
来源：http://zsf.vehdjk.com

[G08] 静态方法与属性
来源：http://zad.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vse.zhijiandao.cn

PHP:  public static function f() {}
来源：http://usq.gzhubu.top

JS:   static f() {}
来源：http://hbj.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://rzd.jinqigufen.top

Java: static void f() {}
来源：http://qwf.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hmq.svipenyu.cn

Ruby: def self.f; end
来源：http://tep.xuetiantiany.cn

C#:   public static void F() {}
来源：http://shf.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://git.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://gbe.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aex.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://isb.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://wju.redwolf501.top

Java: interface Shape { double area(); }
来源：http://fjp.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://wsl.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qnf.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://ryw.tianlin.xyz

[G10] 访问控制
来源：http://rwq.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://xvw.tianlin.xyz

PHP:  public / protected / private
来源：http://zct.birdmap.top

JS:   #private 字段；其余公开
来源：http://dyd.gzhubu.top

TS:   public / protected / private
来源：http://faq.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://ogs.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ppo.zhixingplan.top

Ruby: public / protected / private
来源：http://ikz.0kj1m.cn

C#:   public / protected / private / internal
来源：http://ldl.yuanzhike.top

[G11] getter / setter
来源：http://iwj.iojbl.cn

Py:   @property 与 @x.setter
来源：http://frk.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iaj.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://xlx.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://cxw.zycfv.cn

Java: public String getName() { return name; }
来源：http://pnu.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://avr.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://snf.hcnkem.com

C#:   public string Name { get; set; }
来源：http://xdu.svipenyu.cn

[G12] 对象转字符串
来源：http://seo.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://lqr.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wrc.epnwcf.com

JS:   toString() { return this.name; }
来源：http://bdb.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://vkq.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://utm.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iuk.c1oappe.top

Ruby: def to_s; @name; end
来源：http://ecn.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://ewv.9152youxi.cn

[G13] 判断对象类型
来源：http://gnf.hywenlv.cn

Py:   isinstance(u, User)
来源：http://ajm.gotoacloud.top

PHP:  $u instanceof User
来源：http://nig.cdnleiting.top

JS:   u instanceof User
来源：http://rqv.nwbrower.top

TS:   u instanceof User
来源：http://zby.hammf.cn

Java: u instanceof User
来源：http://dag.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kxy.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://gyn.zhiwuduotai.top

C#:   u is User
来源：http://kmb.sysykeji.top

[G14] 数据类 / record
来源：http://urt.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vtu.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://jpi.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xnm.kuanghao11.cn


<!-- 参考信息 -->