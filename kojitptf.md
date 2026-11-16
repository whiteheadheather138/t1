代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mwn.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pty.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dah.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uru.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pim.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://cpy.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xzd.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zqg.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xtx.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fol.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zcu.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rgq.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://coe.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sro.aizwys.cn

[E16] 数字千分位
来源：http://omz.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://naf.gogol.net.cn

PHP:  number_format(1234567);
来源：http://uso.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://twh.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gav.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddx.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lem.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ydd.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://izl.yfazqb.com

[E17] 首字母大写
来源：http://mvb.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mav.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://tje.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://skq.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kns.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lxr.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aqu.zhoulong.xyz

Ruby: s.capitalize
来源：http://tla.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://afi.yongpay.top

[E18] 模板占位符替换
来源：http://skh.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nlm.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://byc.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gxq.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ibu.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hfh.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sji.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rdz.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nqs.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://ezo.yuanzhike.top

Py:   s.splitlines()
来源：http://uum.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aot.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://pfa.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://esp.gotoacloud.top

Java: s.lines().toList()
来源：http://zvb.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://jzo.uphjek.com

Ruby: s.lines
来源：http://nkr.ydjk.org.cn

C#:   s.Split('\n')
来源：http://lyd.yj20258888.top

[E20] 判断字符串是否为空
来源：http://gdb.jqgfzy.top

Py:   if not s:
来源：http://dkk.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dul.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bgv.ehwqpu.com

TS:   if (s === "") {}
来源：http://zxz.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://lfn.sxryk.cn

Go:   if s == "" {}
来源：http://wfx.ivvv.top

Ruby: if s.empty?
来源：http://uul.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://btn.tarul.cn

[E21] 超长截断加省略号
来源：http://kdg.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rey.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://peo.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yop.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rjm.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wvo.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://ayw.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dgn.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwn.havefunace.top

[E22] 字节长度与字符长度
来源：http://mqj.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tkt.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmr.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qik.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qdk.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qxs.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uvt.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://acu.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://njw.dianchejie.cn

================================================================================
来源：http://sar.vqdsnc.cn

F. 文件与目录
来源：http://cth.yanxiufei.cn

================================================================================
来源：http://ixt.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://iyu.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jel.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://wnr.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://emo.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lur.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ipg.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kjz.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://dhr.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://fhp.shzxlz.cn

[F02] 逐行读取文件
来源：http://yqb.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uvh.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgh.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vzd.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fcu.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hxu.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ygv.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bjt.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iha.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://tfc.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qxr.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rju.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sra.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yup.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tvd.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jgk.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://tod.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wgs.haohaochexian.top

[F04] 追加写入文件
来源：http://gzn.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://otj.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tjz.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vla.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xay.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://efy.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fit.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lnn.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gmc.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://uyt.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nje.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://kem.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://jsp.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://gam.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://som.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jfn.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://kza.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://tvh.ywan-chungtsiang.top

[F06] 删除文件
来源：http://tiq.fzhhl.top

Py:   os.remove("a.txt")
来源：http://vhu.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://rps.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://cme.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://lma.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lji.316326.xyz

Go:   os.Remove("a.txt")
来源：http://bmt.sweek.top

Ruby: File.delete("a.txt")
来源：http://gkx.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://qsa.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://tpi.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jzv.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogz.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cme.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ido.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mge.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bat.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aie.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rlw.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://dkw.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ycm.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ebm.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://jmv.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://mws.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fof.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hqu.vehdjk.com

Ruby: Dir.children("dir")
来源：http://mmj.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://cnw.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://zab.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://uhq.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://ojj.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://gal.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://ecp.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ixb.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wgv.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://vmm.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://uql.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://gyh.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qgi.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hha.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tlw.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://qrh.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cmw.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cft.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kxh.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwp.zhoulong.xyz

[F11] 复制与移动文件
来源：http://iln.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iri.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pye.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://axv.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqw.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mip.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmc.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gwl.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fzl.ppjwa.cn

[F12] CSV 读写
来源：http://nnc.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rzj.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eta.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pdu.daxiang520.top

TS:   // 同上
来源：http://lmq.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hky.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://szx.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mfd.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ikc.dianchejie.cn

================================================================================
来源：http://hnl.xziqi.cn

G. 面向对象
来源：http://wpc.sxryk.cn

================================================================================
来源：http://hmj.fanxiaobao.xyz

[G01] 定义类
来源：http://vkm.hywenlv.cn

Py:   class User: pass
来源：http://pjf.smart0.xyz

PHP:  class User {}
来源：http://flr.zdbjq.cn

JS:   class User {}
来源：http://qij.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://cnb.c1oappe.top

Java: class User {}
来源：http://zuf.0kj1m.cn

Go:   type User struct { Name string }
来源：http://eqy.cheryme.top

Ruby: class User; end
来源：http://yvb.316326.xyz

C#:   class User {}
来源：http://kdn.fanxiaobao.xyz

[G02] 构造函数
来源：http://ggw.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://pli.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://bve.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://zel.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://mlv.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://svt.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obx.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://lwm.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://viq.ehwqpu.com

[G03] 实例属性
来源：http://eaq.yfazqb.com

Py:   self.name = "x"
来源：http://dhl.sufxvd.cn

PHP:  public string $name = "x";
来源：http://ola.hnxiangtu.top

JS:   this.name = "x";
来源：http://thw.fengsongda.top

TS:   name: string = "x";
来源：http://udo.chenzaomai.com

Java: private String name;
来源：http://lhf.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gps.9152youxi.cn

Ruby: @name = "x"
来源：http://fte.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://pdg.ybcxt.top

[G04] 定义方法
来源：http://ppp.meibo888.top

Py:   def greet(self): return self.name
来源：http://aix.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://yvy.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://kfk.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://cas.quarkkingdee.top

Java: String greet() { return name; }
来源：http://slm.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://goc.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://owh.smart0.xyz

C#:   public string Greet() => Name;
来源：http://zff.zhixingplan.top

[G05] 继承
来源：http://znn.yfazqb.com

Py:   class Admin(User): pass
来源：http://pgm.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://lak.cheryme.top

JS:   class Admin extends User {}
来源：http://sxh.fehbvm.com

TS:   class Admin extends User {}
来源：http://emy.jlsjyb.cn

Java: class Admin extends User {}
来源：http://nkj.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eqa.bbcook.cn

Ruby: class Admin < User; end
来源：http://uzy.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://fvp.yj202588.top

[G06] 重写方法
来源：http://fni.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://bgo.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uzd.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://qbp.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://loy.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://zwz.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://six.yj202588.top

Ruby: def greet; "admin"; end
来源：http://utc.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://mjf.ydjk.org.cn

[G07] 调用父类方法
来源：http://opc.gotoacloud.top

Py:   super().greet()
来源：http://yhz.meibo888.top

PHP:  parent::greet();
来源：http://ray.sysykeji.top

JS:   super.greet();
来源：http://upk.cqqwz.cn

TS:   super.greet();
来源：http://rkq.jinqigufen.top

Java: super.greet();
来源：http://amh.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sxq.epnwcf.com

Ruby: super
来源：http://qth.mhx1999.top

C#:   base.Greet();
来源：http://ble.kuanghao11.cn

[G08] 静态方法与属性
来源：http://xzv.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mkw.yueranfly.top

PHP:  public static function f() {}
来源：http://cef.jqgufenzy.top

JS:   static f() {}
来源：http://yzv.yfazqb.com

TS:   static f(): void {}
来源：http://smd.nanxuanxn.top

Java: static void f() {}
来源：http://dpm.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bfw.jqgfzy.top

Ruby: def self.f; end
来源：http://oxe.gaohongyu789.top

C#:   public static void F() {}
来源：http://ski.tian-w.cn

[G09] 接口 / 抽象类
来源：http://erk.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://mux.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://gdo.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eej.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://yhz.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://rva.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://gyk.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tom.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://tdq.xziqi.cn

[G10] 访问控制
来源：http://mcc.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://fmg.0kj1m.cn

PHP:  public / protected / private
来源：http://zxv.andypj.xyz

JS:   #private 字段；其余公开
来源：http://pbx.zhijiandao.cn

TS:   public / protected / private
来源：http://adt.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://fjp.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yuk.52xcode.cn

Ruby: public / protected / private
来源：http://jmz.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://jkm.shanyushiyangtech.top

[G11] getter / setter
来源：http://sru.aizwys.cn

Py:   @property 与 @x.setter
来源：http://tsx.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xvp.yongpay.top

JS:   get name() { return this._name; }
来源：http://eoe.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://wih.sufxvd.cn

Java: public String getName() { return name; }
来源：http://sci.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xsk.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://smr.gzhubu.top

C#:   public string Name { get; set; }
来源：http://aus.cashguo.top

[G12] 对象转字符串
来源：http://ijn.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://ggu.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xtl.daria6918.cn

JS:   toString() { return this.name; }
来源：http://qwk.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://ylx.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://cnx.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://ree.cheryme.top

Ruby: def to_s; @name; end
来源：http://huc.cashguo.top

C#:   public override string ToString() => Name;
来源：http://rff.andypj.xyz

[G13] 判断对象类型
来源：http://fhn.zhaomingkeji.xyz


<!-- 参考信息 -->