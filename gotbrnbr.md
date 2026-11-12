代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rbc.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://uqx.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hwr.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jwp.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://leo.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://flq.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rsq.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxh.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hab.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fru.jqgufenzy.top

[E16] 数字千分位
来源：http://afx.316326.xyz

Py:   f"{1234567:,}"
来源：http://pbe.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://qoc.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vlm.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ydb.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xez.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iaz.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nso.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://cdh.tanke756.top

[E17] 首字母大写
来源：http://phe.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hsn.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ozk.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ush.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://abx.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bsh.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ltt.aizwys.cn

Ruby: s.capitalize
来源：http://jal.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pht.9152youxi.cn

[E18] 模板占位符替换
来源：http://sob.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tec.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hlc.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://kzk.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://tha.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://paz.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nkv.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yva.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kvw.yonumen.top

[E19] 多行文本按行拆分
来源：http://tat.gotoacloud.top

Py:   s.splitlines()
来源：http://kct.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ccm.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://rlc.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://wui.yanxiufei.cn

Java: s.lines().toList()
来源：http://rrq.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://stx.hfpthk.cn

Ruby: s.lines
来源：http://geh.vqdsnc.cn

C#:   s.Split('\n')
来源：http://tdj.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://plc.ehwqpu.com

Py:   if not s:
来源：http://zmt.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://omg.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qqx.chenzaomai.com

TS:   if (s === "") {}
来源：http://eqf.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://lyi.ybcxt.top

Go:   if s == "" {}
来源：http://ntv.epnwcf.com

Ruby: if s.empty?
来源：http://mfi.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hgd.yueranfly.top

[E21] 超长截断加省略号
来源：http://uzv.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ppk.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytu.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhd.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyb.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iqk.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://amz.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ukl.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tvc.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://mld.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pwi.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jol.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mfp.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://izi.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xuz.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yuz.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://dqq.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nfz.zhixingplan.top

================================================================================
来源：http://cbv.sxryk.cn

F. 文件与目录
来源：http://rsr.zdbjq.cn

================================================================================
来源：http://zhz.wangdashe.top

[F01] 读取整个文件
来源：http://lpa.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fwk.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://vjc.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dvp.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://opz.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jgd.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://biz.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://ghs.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://hrz.yj20258.top

[F02] 逐行读取文件
来源：http://lbg.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lxe.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pap.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cid.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kmp.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oxu.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ddb.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fuz.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eci.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://jaa.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hzu.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pgc.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpm.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://grg.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ocq.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ymx.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://cbe.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qgn.sufxvd.cn

[F04] 追加写入文件
来源：http://bxg.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lsq.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpq.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owl.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nzy.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://krl.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kvh.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qox.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sph.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://dza.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gkb.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://obu.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://ljl.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://uof.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ksg.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idg.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://hgw.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://aeo.cqqwz.cn

[F06] 删除文件
来源：http://adz.meibo888.top

Py:   os.remove("a.txt")
来源：http://usb.nwbrower.top

PHP:  unlink("a.txt");
来源：http://bjp.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://zee.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://dzs.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zcf.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://qbf.tanke756.top

Ruby: File.delete("a.txt")
来源：http://cpq.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://ymy.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://keg.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mxm.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qie.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjf.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nny.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://det.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://boe.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://whj.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kqk.snrcjt.cn

[F08] 遍历目录
来源：http://vnn.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nxu.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tfv.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://lkk.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://hrn.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hzw.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ect.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://eku.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://sap.feifeiyinyue.top

[F09] 获取文件大小
来源：http://juu.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://pom.yj20258888.top

PHP:  filesize("a.txt");
来源：http://bja.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://ykj.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://ohc.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ufk.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yry.yfazqb.com

Ruby: File.size("a.txt")
来源：http://bgs.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://nhn.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://zye.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qaj.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zyu.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajw.yuxming.cn

TS:   path.extname("a.txt")
来源：http://txm.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uqy.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://igc.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bua.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://whn.meibo888.top

[F11] 复制与移动文件
来源：http://oel.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lyg.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rfw.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mjt.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dwd.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sra.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vmo.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yfl.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gwr.sufxvd.cn

[F12] CSV 读写
来源：http://ekg.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gfw.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://phz.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zyb.hongshengwenyu.top

TS:   // 同上
来源：http://xug.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://slb.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gjk.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ecj.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://wse.meibo888.top

================================================================================
来源：http://pxx.zdbjq.cn

G. 面向对象
来源：http://kmo.daxiang520.top

================================================================================
来源：http://ouf.havefunace.top

[G01] 定义类
来源：http://gba.jinghuilouyu.cn

Py:   class User: pass
来源：http://mou.tarul.cn

PHP:  class User {}
来源：http://puz.feifeiyinyue.top

JS:   class User {}
来源：http://yae.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://rjw.sjlbkw.cn

Java: class User {}
来源：http://xvn.xziqi.cn

Go:   type User struct { Name string }
来源：http://wok.yvedp.cn

Ruby: class User; end
来源：http://jll.nwbrower.top

C#:   class User {}
来源：http://aop.bbcook.cn

[G02] 构造函数
来源：http://wur.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://mbg.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://qyw.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://jbh.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://sfk.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://ajf.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kcy.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://xgm.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://ccj.vqdsnc.cn

[G03] 实例属性
来源：http://pac.hnqzz.top

Py:   self.name = "x"
来源：http://swo.yongpay.top

PHP:  public string $name = "x";
来源：http://nxa.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://rxg.chenlongwang.top

TS:   name: string = "x";
来源：http://tyn.xuetiantiany.cn

Java: private String name;
来源：http://ifo.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ktv.jqgfzy.top

Ruby: @name = "x"
来源：http://fal.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://jwj.yuanzhike.top

[G04] 定义方法
来源：http://yhu.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://zep.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oxr.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://ljb.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://mkk.fktsv.cn

Java: String greet() { return name; }
来源：http://oej.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://amd.hywenlv.cn

Ruby: def greet; @name; end
来源：http://xjw.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://urm.gzhubu.top

[G05] 继承
来源：http://bwz.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://hcu.guannengcc.top

PHP:  class Admin extends User {}
来源：http://vkg.fzhhl.top

JS:   class Admin extends User {}
来源：http://nwh.aibaodan.cn

TS:   class Admin extends User {}
来源：http://iaj.cqqwz.cn

Java: class Admin extends User {}
来源：http://gsb.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lym.dianchejie.cn

Ruby: class Admin < User; end
来源：http://pll.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://art.jqgfzy.top

[G06] 重写方法
来源：http://hwr.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://lxv.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://kja.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://fxb.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://ryc.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://pne.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ksu.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://xgf.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://aza.guannengcc.top

[G07] 调用父类方法
来源：http://jvg.gotoacloud.top

Py:   super().greet()
来源：http://nye.xinyue.icu

PHP:  parent::greet();
来源：http://ntf.feifeiyinyue.top

JS:   super.greet();
来源：http://zme.hesvh.cn

TS:   super.greet();
来源：http://wax.gotoacloud.top

Java: super.greet();
来源：http://mmx.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qws.shanyushiyangtech.top

Ruby: super
来源：http://gqp.vqdsnc.cn

C#:   base.Greet();
来源：http://izq.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://npi.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vnv.quarkkingdee.top

PHP:  public static function f() {}
来源：http://wjc.daria6918.cn

JS:   static f() {}
来源：http://foi.havefunace.top

TS:   static f(): void {}
来源：http://rhu.cucudq.cn

Java: static void f() {}
来源：http://nax.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://zfz.hfpthk.cn

Ruby: def self.f; end
来源：http://dqs.hnqzz.top

C#:   public static void F() {}
来源：http://cuv.zycfv.cn

[G09] 接口 / 抽象类
来源：http://bgd.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://edm.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nrb.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tbd.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://lfb.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://zeg.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://nqn.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bfb.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://cev.mhx1999.top

[G10] 访问控制
来源：http://swd.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://kzd.ivvv.top

PHP:  public / protected / private
来源：http://opu.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://paq.uphjek.com

TS:   public / protected / private
来源：http://gnr.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://fha.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sln.0kj1m.cn

Ruby: public / protected / private
来源：http://qkt.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://wgz.tarul.cn

[G11] getter / setter
来源：http://env.birdmap.top

Py:   @property 与 @x.setter
来源：http://gln.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vrk.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://xxn.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://khn.hysaishi.cn

Java: public String getName() { return name; }
来源：http://cxl.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ufy.birdmap.top

Ruby: attr_accessor :name
来源：http://yut.birdmap.top

C#:   public string Name { get; set; }
来源：http://xlk.tianlin.xyz

[G12] 对象转字符串
来源：http://jkw.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://fry.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dln.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://nog.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://grf.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://sqg.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kbw.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://kuv.yj202588.top

C#:   public override string ToString() => Name;
来源：http://ycf.hywenlv.cn

[G13] 判断对象类型
来源：http://fjq.cdnleiting.top

Py:   isinstance(u, User)
来源：http://kat.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://avt.shanyushiyangtech.top

JS:   u instanceof User
来源：http://vxj.ivvv.top

TS:   u instanceof User
来源：http://scq.cucudq.cn


<!-- 参考信息 -->