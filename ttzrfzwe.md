代发 wailian999

[E14] URL 编码与 Base64
来源：http://ksj.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bcz.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bsu.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ymg.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fha.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://srr.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfu.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wnu.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uin.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://ktr.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zpw.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vmu.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iph.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://hvm.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lzw.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rzx.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gdw.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nwu.gogol.net.cn

[E16] 数字千分位
来源：http://owz.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://lgi.hesvh.cn

PHP:  number_format(1234567);
来源：http://tmr.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jkk.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kbc.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kiw.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vke.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://olv.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://tjr.dianchejie.cn

[E17] 首字母大写
来源：http://ntk.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ont.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cdi.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmd.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qft.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://int.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fby.nwbrower.top

Ruby: s.capitalize
来源：http://hko.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://orw.dianchejie.cn

[E18] 模板占位符替换
来源：http://yqo.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jxq.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ecu.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kdf.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://hdy.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rld.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yye.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nvn.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vng.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://nik.yueranfly.top

Py:   s.splitlines()
来源：http://wxi.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gvg.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://lbw.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://qqx.hfpthk.cn

Java: s.lines().toList()
来源：http://qdg.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://ysi.fktsv.cn

Ruby: s.lines
来源：http://qtf.ydzc1.top

C#:   s.Split('\n')
来源：http://ykj.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://mhj.cqqwz.cn

Py:   if not s:
来源：http://peq.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rts.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nsv.pycfn.com

TS:   if (s === "") {}
来源：http://gvb.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://owf.tian-w.cn

Go:   if s == "" {}
来源：http://fow.jqgufenzy.top

Ruby: if s.empty?
来源：http://whg.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://esf.hammf.cn

[E21] 超长截断加省略号
来源：http://hma.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ffo.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tew.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xuz.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yjg.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ppt.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://fxi.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jtl.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ohg.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://evf.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dsi.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://clw.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://chh.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikl.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rsc.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ifc.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://qpd.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vld.zhaomingkeji.xyz

================================================================================
来源：http://mla.yj20258888.top

F. 文件与目录
来源：http://ldd.sysykeji.top

================================================================================
来源：http://dyz.sjlbkw.cn

[F01] 读取整个文件
来源：http://ieh.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://egm.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://niw.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dnr.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mqp.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://msp.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iub.sysykeji.top

Ruby: File.read("a.txt")
来源：http://jam.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://bxm.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://yka.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pyi.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xxf.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ius.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkx.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yig.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gbw.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pdv.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ecb.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://dhx.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://quh.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://boh.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://doe.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqv.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://twu.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wen.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://nir.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jao.ivvv.top

[F04] 追加写入文件
来源：http://opn.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pfh.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vfi.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chr.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://das.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://duo.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pbj.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ymh.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zxb.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://dzn.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qcn.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://ksw.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://qph.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://juv.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pmu.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aij.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://yoj.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://spy.fanxiaobao.xyz

[F06] 删除文件
来源：http://eyt.hammf.cn

Py:   os.remove("a.txt")
来源：http://grf.nwbrower.top

PHP:  unlink("a.txt");
来源：http://pxg.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://sgn.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://brq.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtz.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://cat.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://voo.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://kti.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://ggw.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://laz.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fao.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fqi.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vgk.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mxb.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rlk.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://isq.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mll.feifeiyinyue.top

[F08] 遍历目录
来源：http://ezv.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kwp.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gia.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://ybn.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://kcq.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rwi.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mcr.cashguo.top

Ruby: Dir.children("dir")
来源：http://jau.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://dkc.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://wlt.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://nrz.sysykeji.top

PHP:  filesize("a.txt");
来源：http://vua.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://pfu.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://xjq.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://nvt.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ypc.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://tey.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://tel.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://amo.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ftl.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjz.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uur.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://ixk.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ict.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hoj.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pfk.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ygz.sxryk.cn

[F11] 复制与移动文件
来源：http://glo.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ugx.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hvs.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oio.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzz.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fzb.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mkw.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vam.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qov.gogol.net.cn

[F12] CSV 读写
来源：http://snf.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://snt.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yzh.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqg.chenjidiqi.icu

TS:   // 同上
来源：http://pnm.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oil.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lel.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fmp.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pps.hcnkem.com

================================================================================
来源：http://umm.dashuyun.cn

G. 面向对象
来源：http://nmm.cheryme.top

================================================================================
来源：http://akl.xinyue.icu

[G01] 定义类
来源：http://bhh.hesvh.cn

Py:   class User: pass
来源：http://ipg.cucudq.cn

PHP:  class User {}
来源：http://hsz.andypj.xyz

JS:   class User {}
来源：http://bvw.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://pne.52xcode.cn

Java: class User {}
来源：http://umv.ehwqpu.com

Go:   type User struct { Name string }
来源：http://acn.nanxuanxn.top

Ruby: class User; end
来源：http://irq.epnwcf.com

C#:   class User {}
来源：http://bpe.jlsjyb.cn

[G02] 构造函数
来源：http://dvz.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://ycp.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://mtp.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://exl.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://chq.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://zec.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vgu.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://mdr.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://rpg.cheryme.top

[G03] 实例属性
来源：http://dhl.gaohongyu789.top

Py:   self.name = "x"
来源：http://lsa.svipenyu.cn

PHP:  public string $name = "x";
来源：http://etq.meibo888.top

JS:   this.name = "x";
来源：http://kei.snrcjt.cn

TS:   name: string = "x";
来源：http://onb.yj202588.top

Java: private String name;
来源：http://ixj.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kdu.yj20258888.top

Ruby: @name = "x"
来源：http://emh.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://eyt.jlsjyb.cn

[G04] 定义方法
来源：http://wzy.c1oappe.top

Py:   def greet(self): return self.name
来源：http://mzo.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qxj.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://yon.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://mnh.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://rki.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://klh.sweek.top

Ruby: def greet; @name; end
来源：http://fso.daria6918.cn

C#:   public string Greet() => Name;
来源：http://bot.yonumen.top

[G05] 继承
来源：http://eny.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://daq.sxryk.cn

PHP:  class Admin extends User {}
来源：http://kms.wangdashe.top

JS:   class Admin extends User {}
来源：http://xcx.daria6918.cn

TS:   class Admin extends User {}
来源：http://ixn.chenlongwang.top

Java: class Admin extends User {}
来源：http://hmo.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vtf.nanxinkj.top

Ruby: class Admin < User; end
来源：http://gzj.ehwqpu.com

C#:   class Admin : User {}
来源：http://ota.xylfe.cn

[G06] 重写方法
来源：http://qmn.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://lbj.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yyf.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://gwo.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://ezc.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://vpn.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ijr.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://ukd.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://goe.gotoacloud.top

[G07] 调用父类方法
来源：http://pwu.zhixingplan.top

Py:   super().greet()
来源：http://wtl.ydzc1.top

PHP:  parent::greet();
来源：http://mtu.birdmap.top

JS:   super.greet();
来源：http://egu.yj202588.top

TS:   super.greet();
来源：http://umz.tian-w.cn

Java: super.greet();
来源：http://bes.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ecj.sjlbkw.cn

Ruby: super
来源：http://pzm.jlsjyb.cn

C#:   base.Greet();
来源：http://vxu.yfazqb.com

[G08] 静态方法与属性
来源：http://jqa.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dvf.jlsjyb.cn

PHP:  public static function f() {}
来源：http://ype.yj20258.top

JS:   static f() {}
来源：http://ajf.zhiwuduotai.top

TS:   static f(): void {}
来源：http://jtb.fehbvm.com

Java: static void f() {}
来源：http://bml.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hlv.yvedp.cn

Ruby: def self.f; end
来源：http://nzx.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://dyu.yonumen.top

[G09] 接口 / 抽象类
来源：http://gxm.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://ssc.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://cbd.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nlz.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://tbm.tian-w.cn

Java: interface Shape { double area(); }
来源：http://yrd.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://vbz.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://afb.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://ufq.sjlbkw.cn

[G10] 访问控制
来源：http://kbs.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://lri.birdmap.top

PHP:  public / protected / private
来源：http://vhs.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://nyj.ydzc1.top

TS:   public / protected / private
来源：http://duv.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://btc.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aqy.ctjpmb.com

Ruby: public / protected / private
来源：http://ecq.bbcook.cn

C#:   public / protected / private / internal
来源：http://nea.andypj.xyz

[G11] getter / setter
来源：http://mkc.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://ikt.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eth.fengsongda.top

JS:   get name() { return this._name; }
来源：http://sht.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://sav.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://wby.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cfn.snrcjt.cn

Ruby: attr_accessor :name
来源：http://lzw.cucudq.cn

C#:   public string Name { get; set; }
来源：http://ltb.iojbl.cn

[G12] 对象转字符串
来源：http://bsc.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://lza.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vzv.daxiang520.top

JS:   toString() { return this.name; }
来源：http://kka.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://ypm.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://nyv.snrcjt.cn


<!-- 参考信息 -->