代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qak.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dgy.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bld.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jaj.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://duy.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://het.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://pfr.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pfn.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xlm.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ida.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sbi.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nwf.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jak.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xas.aizwys.cn

[E16] 数字千分位
来源：http://tmi.sysykeji.top

Py:   f"{1234567:,}"
来源：http://ayz.chenzaomai.com

PHP:  number_format(1234567);
来源：http://sbm.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://srd.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xrp.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zbc.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uhs.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nsr.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://gih.jiagoushi.top

[E17] 首字母大写
来源：http://tfl.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://srb.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://dtm.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pex.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hvy.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hsr.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://udt.cucudq.cn

Ruby: s.capitalize
来源：http://dmv.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gxj.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://osw.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mxo.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lri.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mqt.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fzp.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mcf.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yuf.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wpr.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eeg.yj20258888.top

[E19] 多行文本按行拆分
来源：http://bnp.cdnleiting.top

Py:   s.splitlines()
来源：http://ujg.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vel.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://nqa.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://dwe.jianghu66.top

Java: s.lines().toList()
来源：http://bmc.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://era.vqdsnc.cn

Ruby: s.lines
来源：http://rwm.guannengcc.top

C#:   s.Split('\n')
来源：http://oqe.52xcode.cn

[E20] 判断字符串是否为空
来源：http://puj.fengsongda.top

Py:   if not s:
来源：http://qvt.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jtn.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wlc.yanxiufei.cn

TS:   if (s === "") {}
来源：http://uvm.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://pfe.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://iqk.daxiang520.top

Ruby: if s.empty?
来源：http://wmp.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flp.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://uyd.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yar.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwz.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uux.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wgx.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://axf.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://igu.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rjr.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isi.xinyue.icu

[E22] 字节长度与字符长度
来源：http://gdr.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://awa.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgn.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nrm.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhm.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yck.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hnn.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://ggy.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://clj.fzhhl.top

================================================================================
来源：http://hgp.nanxinkj.top

F. 文件与目录
来源：http://fnf.birdmap.top

================================================================================
来源：http://cjn.ydzc1.top

[F01] 读取整个文件
来源：http://rlz.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qen.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://prh.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cok.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cwo.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bes.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tlz.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://eln.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://hfy.epnwcf.com

[F02] 逐行读取文件
来源：http://cxk.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zqn.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uou.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rmn.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmp.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bzq.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://whx.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nvc.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgb.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://pvo.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qvl.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdq.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gek.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mgo.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fla.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nxt.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://dff.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qmr.redwolf501.top

[F04] 追加写入文件
来源：http://qsa.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://okk.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dys.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vot.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipo.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ata.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lss.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zoz.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hqd.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://pwg.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dic.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://txo.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://dos.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://klf.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://git.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nio.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://pra.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://bpp.iojbl.cn

[F06] 删除文件
来源：http://ydi.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://bcj.xuanzx.com

PHP:  unlink("a.txt");
来源：http://ikr.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vzy.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zav.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xui.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://svr.havefunace.top

Ruby: File.delete("a.txt")
来源：http://bqg.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://gyw.vehdjk.com

[F07] 创建目录（含多级）
来源：http://ret.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vzu.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xaz.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ebf.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sji.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ept.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zaz.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zok.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wru.hongshengwenyu.top

[F08] 遍历目录
来源：http://dpv.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zin.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vio.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://qxv.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://bhd.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xkr.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dzg.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://bau.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://noc.svipenyu.cn

[F09] 获取文件大小
来源：http://ivo.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://vnj.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://wrx.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://udg.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://ixf.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://lib.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gsm.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://edo.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://gbb.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://tks.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://udp.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kai.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://idl.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://axe.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aul.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iqe.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cbz.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xqq.hfpthk.cn

[F11] 复制与移动文件
来源：http://qsp.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ifk.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ooy.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cot.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xbs.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qry.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vtb.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tox.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://djr.fanxiaobao.xyz

[F12] CSV 读写
来源：http://sxx.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qix.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bmb.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idz.hnqzz.top

TS:   // 同上
来源：http://iid.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://suc.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fjs.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yok.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://azm.jlsjyb.cn

================================================================================
来源：http://txh.zhijiandao.cn

G. 面向对象
来源：http://txb.jiagoushi.top

================================================================================
来源：http://nth.guowangkeji.top

[G01] 定义类
来源：http://dsq.tianlin.xyz

Py:   class User: pass
来源：http://otz.redwolf501.top

PHP:  class User {}
来源：http://kfh.jinqigufen.top

JS:   class User {}
来源：http://csf.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://zui.quarkkingdee.top

Java: class User {}
来源：http://uzk.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://ezz.yj20258888.top

Ruby: class User; end
来源：http://wqe.sweek.top

C#:   class User {}
来源：http://qnu.ppjwa.cn

[G02] 构造函数
来源：http://ixp.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://nfm.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://mke.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://dmq.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://cvx.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://tqw.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jts.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://kcj.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://ior.cqqwz.cn

[G03] 实例属性
来源：http://vbd.chenlongwang.top

Py:   self.name = "x"
来源：http://jzj.yuxming.cn

PHP:  public string $name = "x";
来源：http://hms.cucudq.cn

JS:   this.name = "x";
来源：http://svt.xylfe.cn

TS:   name: string = "x";
来源：http://krw.zhaomingkeji.xyz

Java: private String name;
来源：http://ybw.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dqz.gzhubu.top

Ruby: @name = "x"
来源：http://ypx.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://dfc.fehbvm.com

[G04] 定义方法
来源：http://kqn.wangdashe.top

Py:   def greet(self): return self.name
来源：http://jtj.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tvf.gzhubu.top

JS:   greet() { return this.name; }
来源：http://oxb.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://otw.ybcxt.top

Java: String greet() { return name; }
来源：http://zol.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aub.xziqi.cn

Ruby: def greet; @name; end
来源：http://ghg.yfazqb.com

C#:   public string Greet() => Name;
来源：http://rjq.epnwcf.com

[G05] 继承
来源：http://vqv.cashguo.top

Py:   class Admin(User): pass
来源：http://qsn.sysykeji.top

PHP:  class Admin extends User {}
来源：http://fys.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://ivq.cdnleiting.top

TS:   class Admin extends User {}
来源：http://srd.9152youxi.cn

Java: class Admin extends User {}
来源：http://wre.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uay.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://ehy.fzhhl.top

C#:   class Admin : User {}
来源：http://eyd.kuanghao11.cn

[G06] 重写方法
来源：http://frn.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://exe.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://irj.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://rax.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://cli.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://gqo.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fev.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://eub.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://gea.nwbrower.top

[G07] 调用父类方法
来源：http://qam.yj202588.top

Py:   super().greet()
来源：http://hic.ybcxt.top

PHP:  parent::greet();
来源：http://qeu.hcnkem.com

JS:   super.greet();
来源：http://fhi.nanxinkj.top

TS:   super.greet();
来源：http://koe.fzhhl.top

Java: super.greet();
来源：http://aif.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ruz.ctjpmb.com

Ruby: super
来源：http://jip.hesvh.cn

C#:   base.Greet();
来源：http://vie.sweek.top

[G08] 静态方法与属性
来源：http://rqm.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qmo.yfazqb.com

PHP:  public static function f() {}
来源：http://vti.dashuyun.cn

JS:   static f() {}
来源：http://moo.fzhhl.top

TS:   static f(): void {}
来源：http://apa.zhongyouzk.top

Java: static void f() {}
来源：http://oxv.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://his.cheryme.top

Ruby: def self.f; end
来源：http://emh.gzhubu.top

C#:   public static void F() {}
来源：http://jgx.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://mij.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://meh.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://fcj.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zln.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://gzc.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://olw.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://oic.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ihr.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://luf.sufxvd.cn

[G10] 访问控制
来源：http://lqd.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://rcq.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://aan.tanke756.top

JS:   #private 字段；其余公开
来源：http://ngi.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://mzt.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://xxg.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lar.shangyingyoupin.top

Ruby: public / protected / private
来源：http://bsu.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://bge.ivvv.top

[G11] getter / setter
来源：http://len.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://cki.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jfe.aizwys.cn

JS:   get name() { return this._name; }
来源：http://dzu.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://qov.yuxming.cn

Java: public String getName() { return name; }
来源：http://tsg.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://orc.yonumen.top

Ruby: attr_accessor :name
来源：http://zsr.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://rix.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://ebz.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://epb.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kwu.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://ahb.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://ktr.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://lvi.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://ftv.ydzc1.top

Ruby: def to_s; @name; end
来源：http://dll.yj20258.top

C#:   public override string ToString() => Name;
来源：http://tfq.sxryk.cn

[G13] 判断对象类型
来源：http://jxw.shanyushiyangtech.top


<!-- 参考信息 -->