代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://isy.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vak.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sav.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ezv.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zji.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://inm.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://phy.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iht.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://frq.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hhi.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxd.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nqg.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zos.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bch.ybcxt.top

[E16] 数字千分位
来源：http://xtr.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://uzl.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://xuv.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lib.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lmt.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ahq.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mpw.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfp.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://dlh.fktsv.cn

[E17] 首字母大写
来源：http://mhp.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://axb.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hnt.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmt.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygi.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blc.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cpi.pycfn.com

Ruby: s.capitalize
来源：http://ppj.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vtp.yanxiufei.cn

[E18] 模板占位符替换
来源：http://vzq.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zik.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cft.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://axq.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jxs.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybz.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lwv.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wkz.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rwc.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://cmo.zhengqikj.top

Py:   s.splitlines()
来源：http://jbe.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yik.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://xnv.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://cxo.cdnleiting.top

Java: s.lines().toList()
来源：http://cxq.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://gqf.shanyushiyangtech.top

Ruby: s.lines
来源：http://fls.ydjk.org.cn

C#:   s.Split('\n')
来源：http://jep.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://oui.daria6918.cn

Py:   if not s:
来源：http://bsv.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qqr.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vcd.tarul.cn

TS:   if (s === "") {}
来源：http://fud.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://fye.zhijiandao.cn

Go:   if s == "" {}
来源：http://dqv.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://ytq.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qil.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://xee.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oxg.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eco.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntv.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycr.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xuy.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jmq.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cea.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cbh.yvedp.cn

[E22] 字节长度与字符长度
来源：http://lzm.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iyn.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://egs.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzc.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ayx.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tbr.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xfw.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://ggi.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kwm.gogol.net.cn

================================================================================
来源：http://okc.nanxinkj.top

F. 文件与目录
来源：http://leq.cheryme.top

================================================================================
来源：http://ebe.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://ezq.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ong.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://atm.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ole.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uje.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kwj.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ggj.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://bxi.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://cqr.jlsjyb.cn

[F02] 逐行读取文件
来源：http://alw.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npy.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rrx.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gjs.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ysj.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rtm.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zik.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oea.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gzj.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://dvm.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzy.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kdj.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkg.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zpv.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mez.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cqb.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qek.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://via.hnxiangtu.top

[F04] 追加写入文件
来源：http://hgc.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://urw.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpu.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://byk.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fad.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://khx.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jfu.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bps.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hmp.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://usc.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpe.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://kyx.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://rre.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://dzc.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vtc.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrd.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://bhf.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://kyu.zhongyouzk.top

[F06] 删除文件
来源：http://utp.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://cdl.bbcook.cn

PHP:  unlink("a.txt");
来源：http://gpi.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://wco.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://dwq.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jej.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://bvc.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://bjl.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://qvb.tanke756.top

[F07] 创建目录（含多级）
来源：http://tdh.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bjp.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ngc.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yla.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://msd.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uvu.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zup.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bsl.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iec.ctjpmb.com

[F08] 遍历目录
来源：http://ifg.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cmv.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fdw.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://mbz.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://aze.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vpn.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yxn.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://lqu.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://klz.dashuyun.cn

[F09] 获取文件大小
来源：http://utc.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://cxo.yonumen.top

PHP:  filesize("a.txt");
来源：http://jor.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://wlo.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://qsl.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://inz.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sgg.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://wsd.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://lhv.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://qmm.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fcc.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xyn.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cbw.wangdashe.top

TS:   path.extname("a.txt")
来源：http://qtv.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jvj.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zqo.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rlx.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lle.gaohongyu789.top

[F11] 复制与移动文件
来源：http://qqf.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://okq.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cox.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azn.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lly.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gtb.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qxz.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nyl.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yti.vehdjk.com

[F12] CSV 读写
来源：http://wfb.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zrr.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sqc.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cdh.fanxiaobao.xyz

TS:   // 同上
来源：http://ysa.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iid.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfs.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ano.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ppm.yj20258888.top

================================================================================
来源：http://nqn.iojbl.cn

G. 面向对象
来源：http://hpu.kuanghao11.cn

================================================================================
来源：http://eqf.sxryk.cn

[G01] 定义类
来源：http://dwv.ehwqpu.com

Py:   class User: pass
来源：http://pxn.tarul.cn

PHP:  class User {}
来源：http://onw.pycfn.com

JS:   class User {}
来源：http://ljo.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://hzj.jinghuilouyu.cn

Java: class User {}
来源：http://ucd.bjfxy.top

Go:   type User struct { Name string }
来源：http://ixc.aizwys.cn

Ruby: class User; end
来源：http://qoz.yonumen.top

C#:   class User {}
来源：http://nai.tarul.cn

[G02] 构造函数
来源：http://dgp.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://jqv.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://pdq.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://imr.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://yba.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://dkl.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://emz.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://skr.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://avb.yvedp.cn

[G03] 实例属性
来源：http://pll.meibo888.top

Py:   self.name = "x"
来源：http://xvo.guannengcc.top

PHP:  public string $name = "x";
来源：http://nyu.fzhhl.top

JS:   this.name = "x";
来源：http://lsm.cdnleiting.top

TS:   name: string = "x";
来源：http://ued.wangshuangyany.cn

Java: private String name;
来源：http://iil.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wux.zhengqikj.top

Ruby: @name = "x"
来源：http://kab.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gtv.svipenyu.cn

[G04] 定义方法
来源：http://fcu.shuidangran.top

Py:   def greet(self): return self.name
来源：http://vte.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rjk.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://cue.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://bsj.pycfn.com

Java: String greet() { return name; }
来源：http://gig.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://woe.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://evp.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://kbe.yj20258.top

[G05] 继承
来源：http://mjc.bjfxy.top

Py:   class Admin(User): pass
来源：http://hde.fzhhl.top

PHP:  class Admin extends User {}
来源：http://xon.ctjpmb.com

JS:   class Admin extends User {}
来源：http://ywe.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://sog.birdmap.top

Java: class Admin extends User {}
来源：http://xaq.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jss.vehdjk.com

Ruby: class Admin < User; end
来源：http://orx.yj20258.top

C#:   class Admin : User {}
来源：http://ccl.jianghu66.top

[G06] 重写方法
来源：http://tuj.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://jld.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://soj.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://npg.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://ffc.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://peb.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hkt.pycfn.com

Ruby: def greet; "admin"; end
来源：http://tnf.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://psq.shzxlz.cn

[G07] 调用父类方法
来源：http://jhj.zhaomingkeji.xyz

Py:   super().greet()
来源：http://mwr.316326.xyz

PHP:  parent::greet();
来源：http://gqj.shzxlz.cn

JS:   super.greet();
来源：http://zbw.chenjidiqi.icu

TS:   super.greet();
来源：http://mnp.yuxming.cn

Java: super.greet();
来源：http://wwt.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eph.mhx1999.top

Ruby: super
来源：http://xqt.sxryk.cn

C#:   base.Greet();
来源：http://ure.gzhubu.top

[G08] 静态方法与属性
来源：http://dqq.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kjm.fktsv.cn

PHP:  public static function f() {}
来源：http://zas.cdnleiting.top

JS:   static f() {}
来源：http://ihp.yvedp.cn

TS:   static f(): void {}
来源：http://esy.sufxvd.cn

Java: static void f() {}
来源：http://zgy.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bgt.zdbjq.cn

Ruby: def self.f; end
来源：http://xbi.gogol.net.cn

C#:   public static void F() {}
来源：http://jcm.hammf.cn

[G09] 接口 / 抽象类
来源：http://mhg.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://yrd.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://rom.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bcn.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://tjy.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://odp.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://ugj.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ppi.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://szb.chenjidiqi.icu

[G10] 访问控制
来源：http://luv.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://rgj.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://gnz.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pxs.cashguo.top

TS:   public / protected / private
来源：http://jxx.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://yew.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mhz.bjfxy.top

Ruby: public / protected / private
来源：http://ygb.daxiang520.top

C#:   public / protected / private / internal
来源：http://omo.zhongyouzk.top

[G11] getter / setter
来源：http://nkg.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://aex.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://din.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://fjs.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://rti.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://gli.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhs.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://zgj.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://kpt.jinqigfzy.top

[G12] 对象转字符串
来源：http://kvr.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://ezt.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uqz.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://zhk.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://qip.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://tyv.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sej.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://gou.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://trs.chenlongwang.top

[G13] 判断对象类型
来源：http://bjz.52xcode.cn


<!-- 参考信息 -->