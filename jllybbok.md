代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://omp.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ujd.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dnx.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iys.fktsv.cn

[E14] URL 编码与 Base64
来源：http://gnx.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kfo.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kao.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cwt.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hew.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nzg.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://log.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpq.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yfj.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://nxf.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ujl.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wns.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uhk.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tia.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pdp.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jki.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tnz.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lpt.guannengcc.top

[E16] 数字千分位
来源：http://gqf.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://zxg.chenlongwang.top

PHP:  number_format(1234567);
来源：http://iti.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nyn.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ohd.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvr.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oir.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kpa.sweek.top

C#:   1234567.ToString("N0")
来源：http://xnl.jqgufenzy.top

[E17] 首字母大写
来源：http://jbr.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vke.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hik.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ujn.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://okx.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vbv.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ius.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://ttz.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://acc.gotoacloud.top

[E18] 模板占位符替换
来源：http://wgi.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pld.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://izv.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jwn.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qlk.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fhl.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hae.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gwj.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dmf.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://dnz.hnqzz.top

Py:   s.splitlines()
来源：http://lye.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mii.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://sds.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://cwb.cucudq.cn

Java: s.lines().toList()
来源：http://ivj.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://cui.52xcode.cn

Ruby: s.lines
来源：http://ptq.mhx1999.top

C#:   s.Split('\n')
来源：http://muw.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://bxo.zhaomingkeji.xyz

Py:   if not s:
来源：http://dcb.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://huu.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://anx.xziqi.cn

TS:   if (s === "") {}
来源：http://wth.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://mpa.smart0.xyz

Go:   if s == "" {}
来源：http://xnw.fengsongda.top

Ruby: if s.empty?
来源：http://cnh.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nls.tanke756.top

[E21] 超长截断加省略号
来源：http://upc.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ird.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://apd.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://itd.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcy.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xdp.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://djk.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vsf.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mpa.yfazqb.com

[E22] 字节长度与字符长度
来源：http://chm.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gaj.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://awo.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbd.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wzo.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nyf.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xcq.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://jne.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qkn.cheryme.top

================================================================================
来源：http://kld.yangfankeji.com

F. 文件与目录
来源：http://tas.9152youxi.cn

================================================================================
来源：http://txu.redwolf501.top

[F01] 读取整个文件
来源：http://iqo.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nyc.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://ode.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cia.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ukb.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fhx.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ujg.sweek.top

Ruby: File.read("a.txt")
来源：http://lqq.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://opn.vqdsnc.cn

[F02] 逐行读取文件
来源：http://rgg.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://exd.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fdg.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://viv.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vsp.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xph.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zgg.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fpa.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqj.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://npf.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jjw.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://enx.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztt.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjh.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hkr.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lfg.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ctw.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ztr.bbcook.cn

[F04] 追加写入文件
来源：http://ect.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wbf.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lkb.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwp.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfr.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oxv.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfk.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mop.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvn.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://ncp.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://icy.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://npe.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://xxr.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://yqx.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uem.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://efi.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://caw.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://giz.yuxming.cn

[F06] 删除文件
来源：http://qay.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://dla.xuanzx.com

PHP:  unlink("a.txt");
来源：http://eab.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://bty.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pxw.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhx.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://koi.birdmap.top

Ruby: File.delete("a.txt")
来源：http://vwr.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://cri.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://dsl.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lba.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xfi.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rtl.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ted.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://szp.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nbj.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kuu.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ymt.hnqzz.top

[F08] 遍历目录
来源：http://yqe.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fip.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eks.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://eno.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://pcc.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xfz.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gtl.xziqi.cn

Ruby: Dir.children("dir")
来源：http://fys.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://tas.aibaodan.cn

[F09] 获取文件大小
来源：http://ycl.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://rwa.xuanzx.com

PHP:  filesize("a.txt");
来源：http://voa.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://zki.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://cep.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tcw.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://csk.yj20258888.top

Ruby: File.size("a.txt")
来源：http://mvw.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://xau.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://uyx.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bxw.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fzc.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cfy.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://mxi.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dkk.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cgs.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uoq.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cdz.yfazqb.com

[F11] 复制与移动文件
来源：http://env.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzn.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qed.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ear.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wxf.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://npv.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pol.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lmz.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uux.sxryk.cn

[F12] CSV 读写
来源：http://ycl.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kjs.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iwb.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xsh.pengpengdd.cyou

TS:   // 同上
来源：http://mpg.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lwx.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyi.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mun.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hjb.iojbl.cn

================================================================================
来源：http://brv.zhongyouzk.top

G. 面向对象
来源：http://aan.epnwcf.com

================================================================================
来源：http://vse.hywenlv.cn

[G01] 定义类
来源：http://zyr.jinqigufen.top

Py:   class User: pass
来源：http://avy.gogol.net.cn

PHP:  class User {}
来源：http://kvh.shzxlz.cn

JS:   class User {}
来源：http://req.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://gyu.zhongyouzk.top

Java: class User {}
来源：http://emp.ctjpmb.com

Go:   type User struct { Name string }
来源：http://uuz.cucudq.cn

Ruby: class User; end
来源：http://qyt.hnqzz.top

C#:   class User {}
来源：http://wsz.sweek.top

[G02] 构造函数
来源：http://fwb.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://rms.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://usm.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://itt.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://wmc.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://fdh.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qji.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://uup.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://ydw.tian-w.cn

[G03] 实例属性
来源：http://ttj.c1oappe.top

Py:   self.name = "x"
来源：http://wve.yuanzhike.top

PHP:  public string $name = "x";
来源：http://pgz.ydjk.org.cn

JS:   this.name = "x";
来源：http://vwa.dashuyun.cn

TS:   name: string = "x";
来源：http://xfd.guannengcc.top

Java: private String name;
来源：http://drp.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rsk.yfazqb.com

Ruby: @name = "x"
来源：http://van.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://ymo.fanxiaobao.xyz

[G04] 定义方法
来源：http://qxp.tian-w.cn

Py:   def greet(self): return self.name
来源：http://xqg.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wfh.ivvv.top

JS:   greet() { return this.name; }
来源：http://abk.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://kzu.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://miw.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pnu.cucudq.cn

Ruby: def greet; @name; end
来源：http://iax.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://gwi.hongshengwenyu.top

[G05] 继承
来源：http://bit.daxiang520.top

Py:   class Admin(User): pass
来源：http://gaj.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://mwa.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://bwn.aibaodan.cn

TS:   class Admin extends User {}
来源：http://cvt.redwolf501.top

Java: class Admin extends User {}
来源：http://iby.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ark.pycfn.com

Ruby: class Admin < User; end
来源：http://yjl.hywenlv.cn

C#:   class Admin : User {}
来源：http://zmn.sysykeji.top

[G06] 重写方法
来源：http://avo.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://uky.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ddf.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://aip.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://dso.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://wka.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tbc.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://bus.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://hil.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://djx.zhongyouzk.top

Py:   super().greet()
来源：http://kft.zhoulong.xyz

PHP:  parent::greet();
来源：http://yjs.tian-w.cn

JS:   super.greet();
来源：http://jrw.shanyushiyangtech.top

TS:   super.greet();
来源：http://gmq.0kj1m.cn

Java: super.greet();
来源：http://oki.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://leh.kuanghao11.cn

Ruby: super
来源：http://swi.fengsongda.top

C#:   base.Greet();
来源：http://hpl.hfpthk.cn

[G08] 静态方法与属性
来源：http://sss.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qgn.gaohongyu789.top

PHP:  public static function f() {}
来源：http://vdw.xziqi.cn

JS:   static f() {}
来源：http://oky.birdmap.top

TS:   static f(): void {}
来源：http://qfb.chenzaomai.com

Java: static void f() {}
来源：http://vcb.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zeh.9152youxi.cn

Ruby: def self.f; end
来源：http://ynb.xylfe.cn

C#:   public static void F() {}
来源：http://edg.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://ipn.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://tao.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://kis.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jbq.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://fmq.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://juu.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://omj.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uml.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://uyn.yueranfly.top

[G10] 访问控制
来源：http://cri.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://yun.xziqi.cn

PHP:  public / protected / private
来源：http://mdq.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://kww.feifeiyinyue.top

TS:   public / protected / private
来源：http://zzz.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://uum.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qka.xuetiantiany.cn

Ruby: public / protected / private
来源：http://nvk.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://zmf.zhoulong.xyz

[G11] getter / setter
来源：http://qzb.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://qnv.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://njt.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://dai.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://sei.fktsv.cn

Java: public String getName() { return name; }
来源：http://bij.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xzg.c1oappe.top

Ruby: attr_accessor :name
来源：http://ibj.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://lqe.fengsongda.top

[G12] 对象转字符串
来源：http://ayp.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://htr.epnwcf.com


<!-- 参考信息 -->