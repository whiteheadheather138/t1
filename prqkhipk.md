代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lfp.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jsf.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mek.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kup.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rlf.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://lkn.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://okq.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dhx.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hxv.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ruc.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hob.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gkr.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hhy.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ywq.sxryk.cn

[E16] 数字千分位
来源：http://var.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://jux.cucudq.cn

PHP:  number_format(1234567);
来源：http://wgy.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://trr.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://kgq.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kuw.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lad.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pli.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://pga.pycfn.com

[E17] 首字母大写
来源：http://mgb.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://byt.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://urk.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvh.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hst.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vsk.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ade.nwbrower.top

Ruby: s.capitalize
来源：http://qyz.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fmc.haohaochexian.top

[E18] 模板占位符替换
来源：http://zrx.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qnx.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bjf.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zbw.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rjg.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://niz.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://duz.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tdc.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tmb.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://llk.aizwys.cn

Py:   s.splitlines()
来源：http://wxz.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lqq.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://rom.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://qgj.svipenyu.cn

Java: s.lines().toList()
来源：http://csj.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://zdv.smart0.xyz

Ruby: s.lines
来源：http://vmj.fktsv.cn

C#:   s.Split('\n')
来源：http://roq.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://xck.0kj1m.cn

Py:   if not s:
来源：http://tqh.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://azz.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hwa.sufxvd.cn

TS:   if (s === "") {}
来源：http://bwo.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://xyp.nwbrower.top

Go:   if s == "" {}
来源：http://bbo.ppjwa.cn

Ruby: if s.empty?
来源：http://zui.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bcx.aibaodan.cn

[E21] 超长截断加省略号
来源：http://baj.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://srh.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cbk.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqr.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nni.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emu.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://rph.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kqw.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ell.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://hgn.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tdt.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kjj.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lrz.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://asw.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tqx.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wfx.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://sof.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ojb.shangyingyoupin.top

================================================================================
来源：http://ray.sysykeji.top

F. 文件与目录
来源：http://igi.svipenyu.cn

================================================================================
来源：http://iui.zhiwuduotai.top

[F01] 读取整个文件
来源：http://uds.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ilm.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://lau.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lfk.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mtk.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://khj.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://muj.daxiang520.top

Ruby: File.read("a.txt")
来源：http://tpm.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://grd.shangyingyoupin.top

[F02] 逐行读取文件
来源：http://fhn.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fxz.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://trt.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvn.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bqm.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qvo.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://skw.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bxa.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://krc.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://wfm.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aml.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcj.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnj.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqy.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jlb.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tkp.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://nhp.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dkh.dashuyun.cn

[F04] 追加写入文件
来源：http://bik.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://smf.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqp.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdx.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gol.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hix.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vtv.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://idk.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxm.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://lvy.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://okd.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://dkk.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://rzf.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://wgu.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mxm.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lbm.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://ser.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://imp.nanxuanxn.top

[F06] 删除文件
来源：http://edd.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://yth.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://tsl.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://oaa.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dwf.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pgm.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://spk.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://qqv.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://yuc.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://rjy.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmy.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tjp.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hsm.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rul.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ghk.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eut.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://esi.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kxn.jinqigufen.top

[F08] 遍历目录
来源：http://xwx.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgt.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eto.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://rhh.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://awq.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://drj.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://obv.cashguo.top

Ruby: Dir.children("dir")
来源：http://vvb.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://uvr.jqgufenzy.top

[F09] 获取文件大小
来源：http://zlu.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://oot.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://hpi.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://zhe.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://kkh.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://nwk.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aqi.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://xrw.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://igg.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://ljh.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pli.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://btr.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dyo.ydzc1.top

TS:   path.extname("a.txt")
来源：http://lhf.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://viq.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aef.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mkq.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sod.gzhubu.top

[F11] 复制与移动文件
来源：http://ssg.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eld.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://crs.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qir.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fhh.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gch.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cir.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wbp.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gkt.cucudq.cn

[F12] CSV 读写
来源：http://tvh.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jxa.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dfh.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://frt.ehwqpu.com

TS:   // 同上
来源：http://xkd.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dzb.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bbx.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rbe.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ijf.zdqjudy.top

================================================================================
来源：http://atx.andypj.xyz

G. 面向对象
来源：http://kkv.hongshengwenyu.top

================================================================================
来源：http://mjz.yj20258.top

[G01] 定义类
来源：http://odz.hesvh.cn

Py:   class User: pass
来源：http://sat.gaohongyu789.top

PHP:  class User {}
来源：http://ysb.jinyuanbaomall.cn

JS:   class User {}
来源：http://irs.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://fuq.jqgufenzy.top

Java: class User {}
来源：http://fgo.haohaochexian.top

Go:   type User struct { Name string }
来源：http://zgc.epnwcf.com

Ruby: class User; end
来源：http://lbv.yuxming.cn

C#:   class User {}
来源：http://eyu.hammf.cn

[G02] 构造函数
来源：http://umz.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://dhk.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://oxg.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://bqa.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://jku.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://bwg.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gqk.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://gwk.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://mrx.316326.xyz

[G03] 实例属性
来源：http://oms.svipenyu.cn

Py:   self.name = "x"
来源：http://qmm.fehbvm.com

PHP:  public string $name = "x";
来源：http://nzi.zycfv.cn

JS:   this.name = "x";
来源：http://vnm.bjfxy.top

TS:   name: string = "x";
来源：http://dla.snrcjt.cn

Java: private String name;
来源：http://jxn.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oam.gotoacloud.top

Ruby: @name = "x"
来源：http://zak.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://cjr.dashuyun.cn

[G04] 定义方法
来源：http://zcx.iojbl.cn

Py:   def greet(self): return self.name
来源：http://tvq.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uao.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://rjy.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://fha.kuanghao11.cn

Java: String greet() { return name; }
来源：http://bvc.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mes.fktsv.cn

Ruby: def greet; @name; end
来源：http://efv.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://bcc.jianghu66.top

[G05] 继承
来源：http://tpy.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://uon.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://zqq.daria6918.cn

JS:   class Admin extends User {}
来源：http://oep.vehdjk.com

TS:   class Admin extends User {}
来源：http://zhf.yueranfly.top

Java: class Admin extends User {}
来源：http://ndt.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dye.bbcook.cn

Ruby: class Admin < User; end
来源：http://oef.havefunace.top

C#:   class Admin : User {}
来源：http://frb.cucudq.cn

[G06] 重写方法
来源：http://lty.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://yxz.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://cuj.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://eeh.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://vhx.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://skr.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bvf.pycfn.com

Ruby: def greet; "admin"; end
来源：http://niz.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://rqj.jianghu66.top

[G07] 调用父类方法
来源：http://sqg.shuidangran.top

Py:   super().greet()
来源：http://hti.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://tro.yj20258888.top

JS:   super.greet();
来源：http://cdd.yj202588.top

TS:   super.greet();
来源：http://lsq.zhongyouzk.top

Java: super.greet();
来源：http://ihi.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vez.hesvh.cn

Ruby: super
来源：http://fsg.cqqwz.cn

C#:   base.Greet();
来源：http://zjm.fehbvm.com

[G08] 静态方法与属性
来源：http://mkb.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ble.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://pbb.hesvh.cn

JS:   static f() {}
来源：http://laz.sxryk.cn

TS:   static f(): void {}
来源：http://ubt.jinghuilouyu.cn

Java: static void f() {}
来源：http://ygc.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nvm.sysykeji.top

Ruby: def self.f; end
来源：http://rqi.52xcode.cn

C#:   public static void F() {}
来源：http://tmy.fzhhl.top

[G09] 接口 / 抽象类
来源：http://qkp.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://emp.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://upi.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://boi.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://qkc.xuanzx.com

Java: interface Shape { double area(); }
来源：http://rsw.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://koi.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mqv.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://yhu.ydzc1.top

[G10] 访问控制
来源：http://asg.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://hxx.vehdjk.com

PHP:  public / protected / private
来源：http://pfe.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://kpm.hywenlv.cn

TS:   public / protected / private
来源：http://gxo.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://zwq.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nen.9152youxi.cn

Ruby: public / protected / private
来源：http://lui.jqgfzy.top

C#:   public / protected / private / internal
来源：http://rfd.sufxvd.cn

[G11] getter / setter
来源：http://lwv.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://xko.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qmz.iojbl.cn

JS:   get name() { return this._name; }
来源：http://xqs.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://neq.ppjwa.cn

Java: public String getName() { return name; }
来源：http://cng.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://svf.bbcook.cn

Ruby: attr_accessor :name
来源：http://zmk.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://cke.pycfn.com

[G12] 对象转字符串
来源：http://lcg.yj202588.top

Py:   def __str__(self): return self.name
来源：http://hni.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gil.jianghu66.top

JS:   toString() { return this.name; }
来源：http://rem.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://obr.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://pyq.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vts.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://wtx.316326.xyz

C#:   public override string ToString() => Name;
来源：http://msd.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://qtn.redwolf501.top


<!-- 参考信息 -->