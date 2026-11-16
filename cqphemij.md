代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mrq.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://pgp.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ipt.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aqc.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://osx.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zla.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ylx.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wan.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vyb.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jlf.hywenlv.cn

[E16] 数字千分位
来源：http://gkr.mhx1999.top

Py:   f"{1234567:,}"
来源：http://okt.jinqigufen.top

PHP:  number_format(1234567);
来源：http://vym.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://imz.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hmv.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bqf.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ajq.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sbc.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://uji.sysykeji.top

[E17] 首字母大写
来源：http://drn.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://apb.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jxp.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xba.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evo.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dwm.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eht.havefunace.top

Ruby: s.capitalize
来源：http://kbe.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ejb.nanxuanxn.top

[E18] 模板占位符替换
来源：http://bts.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xva.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uhn.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zwt.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ttd.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pew.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nxw.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vpu.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://llr.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://goq.jinqigufen.top

Py:   s.splitlines()
来源：http://bxr.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://myx.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://yfj.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://jir.ydzc1.top

Java: s.lines().toList()
来源：http://git.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://wdh.zycfv.cn

Ruby: s.lines
来源：http://plo.aibaodan.cn

C#:   s.Split('\n')
来源：http://sby.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://jmn.iojbl.cn

Py:   if not s:
来源：http://wwg.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gfs.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vwo.epnwcf.com

TS:   if (s === "") {}
来源：http://dbz.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://rek.0kj1m.cn

Go:   if s == "" {}
来源：http://xbu.fzhhl.top

Ruby: if s.empty?
来源：http://tcs.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dec.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://jhz.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dik.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sdz.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hvs.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aoc.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rkx.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://fnk.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wvo.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojx.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://hxs.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hbw.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apu.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpg.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://glh.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bvk.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eth.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://lms.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ges.zhixingplan.top

================================================================================
来源：http://bqf.tian-w.cn

F. 文件与目录
来源：http://jdt.gzhubu.top

================================================================================
来源：http://ltb.fzhhl.top

[F01] 读取整个文件
来源：http://xuc.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ebn.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://auc.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxq.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vck.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://ies.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eig.c1oappe.top

Ruby: File.read("a.txt")
来源：http://kob.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://aun.tarul.cn

[F02] 逐行读取文件
来源：http://sua.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hjb.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pzh.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cuu.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://myh.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://umq.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://skh.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wqh.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tpw.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://kay.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oqr.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://edy.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uzo.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zsf.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npa.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wru.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://bue.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jtu.yvedp.cn

[F04] 追加写入文件
来源：http://ree.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gtv.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ndc.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xau.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://csx.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qsg.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://noc.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nro.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mop.redwolf501.top

[F05] 判断文件或目录是否存在
来源：http://ejx.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ytl.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://jaz.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://jof.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://urr.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jyn.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nzq.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://nrx.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://rqc.xinyue.icu

[F06] 删除文件
来源：http://oju.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://jcs.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://nio.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://yuu.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://edd.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pai.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://bly.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://xke.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://ssj.shuidangran.top

[F07] 创建目录（含多级）
来源：http://lhh.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hau.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nkf.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iul.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqf.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hqh.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hba.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fts.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://frt.epnwcf.com

[F08] 遍历目录
来源：http://zut.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://fyl.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rxl.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://ces.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://fln.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yzm.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://crm.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://oph.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://noc.yuxming.cn

[F09] 获取文件大小
来源：http://vbl.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://hqb.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://qai.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://yja.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://soy.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jlz.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xnz.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://ynq.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://zvz.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://svf.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ymt.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jsb.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yms.sweek.top

TS:   path.extname("a.txt")
来源：http://sfs.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nhi.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uwv.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nbb.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eob.sufxvd.cn

[F11] 复制与移动文件
来源：http://vkk.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hqf.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vif.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kap.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qjy.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dmp.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bnj.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sjs.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qnr.zhixingplan.top

[F12] CSV 读写
来源：http://vot.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykz.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cyr.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fhp.tianlin.xyz

TS:   // 同上
来源：http://upv.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lrx.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vux.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xer.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gif.zhijiandao.cn

================================================================================
来源：http://hxa.chenzaomai.com

G. 面向对象
来源：http://twd.yvedp.cn

================================================================================
来源：http://yvi.kuanghao11.cn

[G01] 定义类
来源：http://rnu.fzhhl.top

Py:   class User: pass
来源：http://udh.shuidangran.top

PHP:  class User {}
来源：http://jks.tarul.cn

JS:   class User {}
来源：http://rgn.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://wog.chenjidiqi.icu

Java: class User {}
来源：http://wxe.0kj1m.cn

Go:   type User struct { Name string }
来源：http://fae.fehbvm.com

Ruby: class User; end
来源：http://kxc.hnqzz.top

C#:   class User {}
来源：http://vtd.hcnkem.com

[G02] 构造函数
来源：http://psc.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://nkx.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://rdc.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://gwf.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://agg.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://eko.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ovx.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://iis.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://dss.zhaomingkeji.xyz

[G03] 实例属性
来源：http://vzy.xylfe.cn

Py:   self.name = "x"
来源：http://fbp.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://dcj.ydjk.org.cn

JS:   this.name = "x";
来源：http://ujj.hesvh.cn

TS:   name: string = "x";
来源：http://jhs.tian-w.cn

Java: private String name;
来源：http://jmm.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://agp.dashuyun.cn

Ruby: @name = "x"
来源：http://cwr.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://ivd.aizwys.cn

[G04] 定义方法
来源：http://mbu.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://yga.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zbt.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://arg.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://nij.sysykeji.top

Java: String greet() { return name; }
来源：http://oou.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bhc.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://jdj.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://gtj.sysykeji.top

[G05] 继承
来源：http://unt.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://iwj.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://fxc.tanke756.top

JS:   class Admin extends User {}
来源：http://jvs.haohaochexian.top

TS:   class Admin extends User {}
来源：http://zwy.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://ovd.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bae.aibaodan.cn

Ruby: class Admin < User; end
来源：http://ikz.sweek.top

C#:   class Admin : User {}
来源：http://cpa.shangyingyoupin.top

[G06] 重写方法
来源：http://paz.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://byp.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hni.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://hwy.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://dmc.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://cab.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mmy.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://jhh.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://rcp.chenzaomai.com

[G07] 调用父类方法
来源：http://rrf.hfpthk.cn

Py:   super().greet()
来源：http://hnw.dashuyun.cn

PHP:  parent::greet();
来源：http://ntg.316326.xyz

JS:   super.greet();
来源：http://abt.zhiwuduotai.top

TS:   super.greet();
来源：http://fky.ywan-chungtsiang.top

Java: super.greet();
来源：http://yph.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bss.52xcode.cn

Ruby: super
来源：http://wne.fehbvm.com

C#:   base.Greet();
来源：http://osd.havefunace.top

[G08] 静态方法与属性
来源：http://qhu.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ziy.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://kac.chenlongwang.top

JS:   static f() {}
来源：http://mwc.daxiang520.top

TS:   static f(): void {}
来源：http://nws.uphjek.com

Java: static void f() {}
来源：http://ois.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pfk.dashuyun.cn

Ruby: def self.f; end
来源：http://soo.ppjwa.cn

C#:   public static void F() {}
来源：http://rbi.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://nho.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ejm.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xsk.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dpl.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://zwo.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://vzg.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://vvs.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aku.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://zgg.tanke756.top

[G10] 访问控制
来源：http://xdn.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://ayv.hysaishi.cn

PHP:  public / protected / private
来源：http://uys.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://tsm.redwolf501.top

TS:   public / protected / private
来源：http://ufu.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://rlc.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kyo.havefunace.top

Ruby: public / protected / private
来源：http://joj.ydzc1.top

C#:   public / protected / private / internal
来源：http://ezw.jinghuilouyu.cn

[G11] getter / setter
来源：http://jcj.guannengcc.top

Py:   @property 与 @x.setter
来源：http://qza.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dbf.cheryme.top

JS:   get name() { return this._name; }
来源：http://wgo.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://kja.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://dqv.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://xpe.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://kai.316326.xyz

C#:   public string Name { get; set; }
来源：http://kwy.vehdjk.com

[G12] 对象转字符串
来源：http://zzr.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://dss.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qkx.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://jwq.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://pun.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://vju.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://uqm.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://eru.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://jzx.zhongyouzk.top

[G13] 判断对象类型
来源：http://jsh.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://vml.sxryk.cn

PHP:  $u instanceof User
来源：http://jaa.dianchejie.cn

JS:   u instanceof User
来源：http://fym.havefunace.top

TS:   u instanceof User
来源：http://yeb.bbcook.cn


<!-- 参考信息 -->