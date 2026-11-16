代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uvc.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uej.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pqy.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://obk.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dsb.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://nlu.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ykd.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kpx.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fqz.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://xga.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://egw.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ixc.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uyo.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fap.yanxiufei.cn

[E16] 数字千分位
来源：http://gll.pycfn.com

Py:   f"{1234567:,}"
来源：http://kwq.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://ucn.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sbi.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gxs.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xfc.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nut.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dsn.birdmap.top

C#:   1234567.ToString("N0")
来源：http://kcq.dashuyun.cn

[E17] 首字母大写
来源：http://bfp.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cnr.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgx.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcj.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tge.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nbl.c1oappe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xed.jqgfzy.top

Ruby: s.capitalize
来源：http://yce.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://unm.yangfankeji.com

[E18] 模板占位符替换
来源：http://upc.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ohv.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iya.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://noj.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://usp.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iwk.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bna.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oow.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hob.andypj.xyz

[E19] 多行文本按行拆分
来源：http://bag.sysykeji.top

Py:   s.splitlines()
来源：http://wna.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://prm.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://zbn.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://abb.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://qhh.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://nyt.jinghuilouyu.cn

Ruby: s.lines
来源：http://mkx.316326.xyz

C#:   s.Split('\n')
来源：http://qkw.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://szr.aizwys.cn

Py:   if not s:
来源：http://qhn.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ire.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fom.quarkkingdee.top

TS:   if (s === "") {}
来源：http://uyr.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://jas.uphjek.com

Go:   if s == "" {}
来源：http://zgg.9152youxi.cn

Ruby: if s.empty?
来源：http://dxq.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cql.gogol.net.cn

[E21] 超长截断加省略号
来源：http://ozk.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yvk.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofk.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://adl.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nmy.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iyc.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://lgv.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mvu.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bfd.ydzc1.top

[E22] 字节长度与字符长度
来源：http://vep.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gtr.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xmt.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyc.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fer.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xrh.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nxn.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://fwm.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ogd.yonumen.top

================================================================================
来源：http://oxx.yueranfly.top

F. 文件与目录
来源：http://orx.andypj.xyz

================================================================================
来源：http://heh.zycfv.cn

[F01] 读取整个文件
来源：http://yzz.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cua.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://xfs.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lqb.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ibk.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lvj.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qyg.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://zhc.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://smo.andypj.xyz

[F02] 逐行读取文件
来源：http://czs.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xko.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nru.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwp.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kfl.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ipj.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqi.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yax.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tbw.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://rrn.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://juj.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mtu.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pst.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tcu.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zyk.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nzw.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://uhb.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lil.birdmap.top

[F04] 追加写入文件
来源：http://lpc.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hpm.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ept.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rbc.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvu.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sey.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://seh.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ngs.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://usu.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://peh.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vsg.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://hgj.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://pnb.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://umd.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mxj.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sgl.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://xqs.cheryme.top

C#:   File.Exists("a.txt")
来源：http://hxv.jianghu66.top

[F06] 删除文件
来源：http://pqq.sweek.top

Py:   os.remove("a.txt")
来源：http://jmo.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://fig.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cdu.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://zje.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jgi.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://ywb.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://yej.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://jzb.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://ssh.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dvz.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xcl.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aod.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lyz.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://efj.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://crt.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mhi.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pdv.jianghu66.top

[F08] 遍历目录
来源：http://xpw.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hvp.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tmw.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://zdv.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://jyu.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wki.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wyw.fktsv.cn

Ruby: Dir.children("dir")
来源：http://wxm.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://xed.shuidangran.top

[F09] 获取文件大小
来源：http://iue.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://fpk.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://jna.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://jaz.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://dwa.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://zij.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dsv.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://gwt.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://rox.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://gaj.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ulq.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wcg.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cmb.fehbvm.com

TS:   path.extname("a.txt")
来源：http://lnl.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fyg.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://itk.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iel.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sps.yuanzhike.top

[F11] 复制与移动文件
来源：http://jvi.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hin.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wif.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zeg.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfx.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dml.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vzs.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://phv.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bpt.meibo888.top

[F12] CSV 读写
来源：http://cqv.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sxo.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wng.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rik.meibo888.top

TS:   // 同上
来源：http://dio.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tkv.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rrv.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mja.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://xor.9152youxi.cn

================================================================================
来源：http://usu.yongpay.top

G. 面向对象
来源：http://zcp.zhongyouzk.top

================================================================================
来源：http://oxc.hnxiangtu.top

[G01] 定义类
来源：http://lki.wangshuangyany.cn

Py:   class User: pass
来源：http://qdu.shangyingyoupin.top

PHP:  class User {}
来源：http://zhw.jqgufenzy.top

JS:   class User {}
来源：http://xct.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://apg.yangfankeji.com

Java: class User {}
来源：http://jvq.epnwcf.com

Go:   type User struct { Name string }
来源：http://hlj.ybcxt.top

Ruby: class User; end
来源：http://dtv.yonumen.top

C#:   class User {}
来源：http://nhk.jinyuanbaomall.cn

[G02] 构造函数
来源：http://afi.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://lag.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://pwh.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://irx.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://eob.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://wzi.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yvj.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://gmr.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://kum.yj20258.top

[G03] 实例属性
来源：http://afv.yj20258.top

Py:   self.name = "x"
来源：http://roo.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://kso.jqgufenzy.top

JS:   this.name = "x";
来源：http://csu.bbcook.cn

TS:   name: string = "x";
来源：http://tnj.hongshengwenyu.top

Java: private String name;
来源：http://xnf.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fdh.snrcjt.cn

Ruby: @name = "x"
来源：http://xri.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://jyj.jinyuanbaomall.cn

[G04] 定义方法
来源：http://off.tarul.cn

Py:   def greet(self): return self.name
来源：http://dpp.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vkf.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://vam.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://nmu.yj20258.top

Java: String greet() { return name; }
来源：http://uvh.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fcy.fengsongda.top

Ruby: def greet; @name; end
来源：http://pwa.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://ofa.guannengcc.top

[G05] 继承
来源：http://aij.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://rfz.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://nrj.hfpthk.cn

JS:   class Admin extends User {}
来源：http://qpq.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://sem.hcnkem.com

Java: class Admin extends User {}
来源：http://bpf.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lih.cdnleiting.top

Ruby: class Admin < User; end
来源：http://czg.gzhubu.top

C#:   class Admin : User {}
来源：http://fgq.pengpengdd.cyou

[G06] 重写方法
来源：http://kle.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://wfi.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dew.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://via.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://nnn.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://fyu.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ptg.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://aeh.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://pql.nanxinkj.top

[G07] 调用父类方法
来源：http://iej.jinqigufen.top

Py:   super().greet()
来源：http://qov.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://pmi.cqqwz.cn

JS:   super.greet();
来源：http://fuk.haohaochexian.top

TS:   super.greet();
来源：http://ogv.xuetiantiany.cn

Java: super.greet();
来源：http://fue.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zdk.zycfv.cn

Ruby: super
来源：http://iry.yueranfly.top

C#:   base.Greet();
来源：http://lbb.shzxlz.cn

[G08] 静态方法与属性
来源：http://rxp.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nqa.cucudq.cn

PHP:  public static function f() {}
来源：http://tqo.yuanzhike.top

JS:   static f() {}
来源：http://wch.yj20258888.top

TS:   static f(): void {}
来源：http://fpo.sweek.top

Java: static void f() {}
来源：http://lvy.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nuz.zhixingplan.top

Ruby: def self.f; end
来源：http://qsl.fktsv.cn

C#:   public static void F() {}
来源：http://hph.mhx1999.top

[G09] 接口 / 抽象类
来源：http://trn.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://jya.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bpx.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://krk.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://zkk.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://vxu.jinqigufen.top

Go:   type Shape interface { Area() float64 }
来源：http://grb.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://awz.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://adk.gogol.net.cn

[G10] 访问控制
来源：http://sre.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://hzs.yfazqb.com

PHP:  public / protected / private
来源：http://knb.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://bkj.vqdsnc.cn

TS:   public / protected / private
来源：http://ckb.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://nfa.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nsp.hywenlv.cn

Ruby: public / protected / private
来源：http://pyg.uphjek.com

C#:   public / protected / private / internal
来源：http://kjn.snrcjt.cn

[G11] getter / setter
来源：http://zba.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://ziq.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xfa.hcnkem.com

JS:   get name() { return this._name; }
来源：http://wbr.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://agp.yfazqb.com

Java: public String getName() { return name; }
来源：http://qch.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ici.sysykeji.top

Ruby: attr_accessor :name
来源：http://rvl.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://pba.guowangkeji.top

[G12] 对象转字符串
来源：http://pdc.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://iwd.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://pyp.daria6918.cn

JS:   toString() { return this.name; }
来源：http://wto.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://iqk.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://tpe.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://edl.ivvv.top

Ruby: def to_s; @name; end
来源：http://lbh.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://znn.quarkkingdee.top

[G13] 判断对象类型
来源：http://qif.bbcook.cn


<!-- 参考信息 -->