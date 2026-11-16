代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ysb.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://umm.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vdt.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qzf.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zyz.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nva.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zky.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pgb.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rpw.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uso.xylfe.cn

[E16] 数字千分位
来源：http://loj.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://zmr.yueranfly.top

PHP:  number_format(1234567);
来源：http://ghf.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zoh.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mcw.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wwr.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zdn.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xyj.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://qrb.epnwcf.com

[E17] 首字母大写
来源：http://kcg.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kui.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kyg.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpc.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgr.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qkz.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rok.zhoulong.xyz

Ruby: s.capitalize
来源：http://otu.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uyj.yj20258888.top

[E18] 模板占位符替换
来源：http://gsf.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggk.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zuu.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yxu.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://upm.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jiq.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://asi.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hsg.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ydp.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://xkb.hnqzz.top

Py:   s.splitlines()
来源：http://uas.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jrp.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://urk.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://nwa.xuanzx.com

Java: s.lines().toList()
来源：http://tbl.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://zbg.yuanzhike.top

Ruby: s.lines
来源：http://ozq.fehbvm.com

C#:   s.Split('\n')
来源：http://vpw.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://pcw.yueranfly.top

Py:   if not s:
来源：http://xgc.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://glv.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hxt.yfazqb.com

TS:   if (s === "") {}
来源：http://szi.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://zpt.cucudq.cn

Go:   if s == "" {}
来源：http://uba.vqdsnc.cn

Ruby: if s.empty?
来源：http://daq.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tpn.epnwcf.com

[E21] 超长截断加省略号
来源：http://sgi.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://och.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vke.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztk.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zft.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xpp.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://vzr.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mqb.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ouo.xylfe.cn

[E22] 字节长度与字符长度
来源：http://jqs.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ieo.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rso.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://otm.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ost.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mcz.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gwv.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://gwc.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jkb.jianghu66.top

================================================================================
来源：http://bis.wangshuangyany.cn

F. 文件与目录
来源：http://web.nanxuanxn.top

================================================================================
来源：http://smt.fehbvm.com

[F01] 读取整个文件
来源：http://mvn.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mej.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://opv.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://szu.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qzt.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hrw.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jbu.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://iec.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://xcu.sysykeji.top

[F02] 逐行读取文件
来源：http://mue.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xlm.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://plu.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bin.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tni.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gbq.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oyg.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cls.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kyq.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://mmb.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yol.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://uli.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hga.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bvc.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rte.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://urx.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://cji.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bun.zhixingplan.top

[F04] 追加写入文件
来源：http://bcv.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ema.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iwk.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrj.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tqv.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lit.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jqo.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sdx.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dae.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://nrd.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://til.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://hyk.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://bpb.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://ywk.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ucv.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kun.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://wam.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://kkd.cdnleiting.top

[F06] 删除文件
来源：http://gie.cheryme.top

Py:   os.remove("a.txt")
来源：http://etd.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://ncs.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://ach.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://qiy.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eeo.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://eim.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://odg.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://nbc.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://fhz.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wun.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ynp.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nok.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kxm.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jdj.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfg.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mrd.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cib.zhengqikj.top

[F08] 遍历目录
来源：http://shw.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ryk.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gnw.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://zmk.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://fjo.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vrg.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qpq.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://jws.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://qlk.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://wkk.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://vhi.fktsv.cn

PHP:  filesize("a.txt");
来源：http://nid.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://teq.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://hcu.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hcb.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyr.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://xvl.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://udz.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://nku.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jzs.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gzf.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kdj.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://ror.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dqc.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://src.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fzs.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dod.fktsv.cn

[F11] 复制与移动文件
来源：http://csg.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jxh.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hnr.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdg.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrp.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jme.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ald.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://onc.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://goe.zhiwuduotai.top

[F12] CSV 读写
来源：http://gne.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://atp.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qtc.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qeq.ybcxt.top

TS:   // 同上
来源：http://mge.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ovd.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://whc.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sqf.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sdd.yangfankeji.com

================================================================================
来源：http://nyz.feifeiyinyue.top

G. 面向对象
来源：http://tkk.yueranfly.top

================================================================================
来源：http://iey.hongshengwenyu.top

[G01] 定义类
来源：http://qhb.yueranfly.top

Py:   class User: pass
来源：http://qok.guowangkeji.top

PHP:  class User {}
来源：http://ppm.yongpay.top

JS:   class User {}
来源：http://rwc.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://lge.hywenlv.cn

Java: class User {}
来源：http://hoh.hfpthk.cn

Go:   type User struct { Name string }
来源：http://exh.hongshengwenyu.top

Ruby: class User; end
来源：http://apa.zdqjudy.top

C#:   class User {}
来源：http://vvc.xziqi.cn

[G02] 构造函数
来源：http://wab.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://xic.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://egc.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://xkn.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://sxd.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://iez.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://elq.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://zhl.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://hyq.yfazqb.com

[G03] 实例属性
来源：http://hrz.jinqigufen.top

Py:   self.name = "x"
来源：http://sjt.daria6918.cn

PHP:  public string $name = "x";
来源：http://wyc.xuetiantiany.cn

JS:   this.name = "x";
来源：http://xtw.yangfankeji.com

TS:   name: string = "x";
来源：http://oqm.yanxiufei.cn

Java: private String name;
来源：http://vkt.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lgj.hnxiangtu.top

Ruby: @name = "x"
来源：http://hgc.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://wpi.jqgufenzy.top

[G04] 定义方法
来源：http://pfl.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://gsl.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gbi.xuanzx.com

JS:   greet() { return this.name; }
来源：http://bka.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://tig.jqgfzy.top

Java: String greet() { return name; }
来源：http://djd.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wwd.yj20258888.top

Ruby: def greet; @name; end
来源：http://ttl.xinyue.icu

C#:   public string Greet() => Name;
来源：http://flv.birdmap.top

[G05] 继承
来源：http://apl.xylfe.cn

Py:   class Admin(User): pass
来源：http://xqa.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://vbe.jyoumei.cn

JS:   class Admin extends User {}
来源：http://ifh.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://ltp.tanke756.top

Java: class Admin extends User {}
来源：http://sei.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jdp.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://git.yuanzhike.top

C#:   class Admin : User {}
来源：http://zxx.hesvh.cn

[G06] 重写方法
来源：http://xwj.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://qdb.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ggm.zdqjudy.top

JS:   greet() { return "admin"; }
来源：http://sny.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://zaz.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://ehf.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iuj.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://wwy.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://apf.bjfxy.top

[G07] 调用父类方法
来源：http://syq.ppjwa.cn

Py:   super().greet()
来源：http://wfw.cashguo.top

PHP:  parent::greet();
来源：http://kfw.cqqwz.cn

JS:   super.greet();
来源：http://oix.ctjpmb.com

TS:   super.greet();
来源：http://ely.zhijiandao.cn

Java: super.greet();
来源：http://gkm.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qic.redwolf501.top

Ruby: super
来源：http://sxv.yj20258888.top

C#:   base.Greet();
来源：http://ful.gaohongyu789.top

[G08] 静态方法与属性
来源：http://awp.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjl.sweek.top

PHP:  public static function f() {}
来源：http://kyd.jinqigufen.top

JS:   static f() {}
来源：http://ggm.havefunace.top

TS:   static f(): void {}
来源：http://ula.hammf.cn

Java: static void f() {}
来源：http://cdd.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ejn.yj202588.top

Ruby: def self.f; end
来源：http://hzr.yangfankeji.com

C#:   public static void F() {}
来源：http://olz.andypj.xyz

[G09] 接口 / 抽象类
来源：http://utl.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://cxz.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://xbz.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gba.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://ryj.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://dic.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://jnc.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lgp.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://sue.tanke756.top

[G10] 访问控制
来源：http://zph.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://tmy.0kj1m.cn

PHP:  public / protected / private
来源：http://emr.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://pia.daxiang520.top

TS:   public / protected / private
来源：http://jvu.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://mlz.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fby.hywenlv.cn

Ruby: public / protected / private
来源：http://mzt.mhx1999.top

C#:   public / protected / private / internal
来源：http://gjn.shangyingyoupin.top

[G11] getter / setter
来源：http://hea.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://hof.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qns.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://ekm.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://oya.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://wze.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sws.bjfxy.top

Ruby: attr_accessor :name
来源：http://ytw.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://osp.ehwqpu.com

[G12] 对象转字符串
来源：http://rxt.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://obh.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xyo.daria6918.cn

JS:   toString() { return this.name; }
来源：http://gkb.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://ibq.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://ujb.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nas.nwbrower.top

Ruby: def to_s; @name; end
来源：http://qip.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://yfz.andypj.xyz

[G13] 判断对象类型
来源：http://udl.tarul.cn

Py:   isinstance(u, User)
来源：http://ohb.yj20258.top

PHP:  $u instanceof User
来源：http://qsz.hywenlv.cn

JS:   u instanceof User
来源：http://ylx.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://hni.sxryk.cn


<!-- 参考信息 -->