代发 wailian999

[E14] URL 编码与 Base64
来源：http://btp.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ian.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojr.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tau.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pac.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wnr.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yut.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cxw.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xhz.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://ydh.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://jpg.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jna.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ljm.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mts.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://paz.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dvk.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzc.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ucn.tian-w.cn

[E16] 数字千分位
来源：http://qpy.jianghu66.top

Py:   f"{1234567:,}"
来源：http://gyr.zhixingplan.top

PHP:  number_format(1234567);
来源：http://eab.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jlw.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qdq.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eui.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vhw.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jlc.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://pdk.gzhubu.top

[E17] 首字母大写
来源：http://lmo.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://giv.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://imf.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erz.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sug.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ywe.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kun.fktsv.cn

Ruby: s.capitalize
来源：http://loq.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lxl.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://pus.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gnn.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vde.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fhu.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://bfy.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sbf.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hcd.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uwa.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uqf.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://abs.zhixingplan.top

Py:   s.splitlines()
来源：http://zuy.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zol.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://jlv.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://vam.yanxiufei.cn

Java: s.lines().toList()
来源：http://xcc.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://yzq.pycfn.com

Ruby: s.lines
来源：http://qnr.sxryk.cn

C#:   s.Split('\n')
来源：http://jgx.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://mao.yj20258.top

Py:   if not s:
来源：http://kti.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://peg.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tor.tian-w.cn

TS:   if (s === "") {}
来源：http://hgd.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://nvc.zhiwuduotai.top

Go:   if s == "" {}
来源：http://cvv.uphjek.com

Ruby: if s.empty?
来源：http://jil.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://odk.shzxlz.cn

[E21] 超长截断加省略号
来源：http://syy.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ugy.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hdd.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fex.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddy.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eno.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://sti.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hqj.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://riy.fktsv.cn

[E22] 字节长度与字符长度
来源：http://gri.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fog.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fiu.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nmb.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lip.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bzh.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tnd.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://ffn.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://okq.xuetiantiany.cn

================================================================================
来源：http://ube.hfpthk.cn

F. 文件与目录
来源：http://kod.snrcjt.cn

================================================================================
来源：http://nro.ehwqpu.com

[F01] 读取整个文件
来源：http://mkc.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzz.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://xdx.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pof.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://avc.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vxd.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myh.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://fsu.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://pet.daxiang520.top

[F02] 逐行读取文件
来源：http://dtc.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zwy.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rbu.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dul.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqv.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qtd.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dju.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cmq.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lnz.pycfn.com

[F03] 写入文件（覆盖）
来源：http://ule.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://agp.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgi.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfh.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://out.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pfy.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://osj.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://jzz.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://amn.yonumen.top

[F04] 追加写入文件
来源：http://tsw.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kur.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zlu.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://awh.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlm.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tpx.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qof.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://etm.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hps.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://hdg.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://chb.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://xbc.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://yvs.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://kmq.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://eby.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dfv.sweek.top

Ruby: File.exist?("a.txt")
来源：http://aux.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://xbz.hongshengwenyu.top

[F06] 删除文件
来源：http://vrk.jianghu66.top

Py:   os.remove("a.txt")
来源：http://icn.mhx1999.top

PHP:  unlink("a.txt");
来源：http://xzz.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://cov.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://ayt.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://led.316326.xyz

Go:   os.Remove("a.txt")
来源：http://hoh.yongpay.top

Ruby: File.delete("a.txt")
来源：http://fdc.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://pxv.c1oappe.top

[F07] 创建目录（含多级）
来源：http://pje.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://flr.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ykm.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://luw.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovm.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://acf.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wxp.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mbc.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ksd.feifeiyinyue.top

[F08] 遍历目录
来源：http://akf.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vgo.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqd.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://enu.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://ncw.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tec.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xbq.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://ixf.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://ekt.nanxinkj.top

[F09] 获取文件大小
来源：http://czx.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://xjs.jianghu66.top

PHP:  filesize("a.txt");
来源：http://pxm.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://wiy.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://ixl.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://oav.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dcr.tanke756.top

Ruby: File.size("a.txt")
来源：http://hrh.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://sya.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://wak.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iel.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sog.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bzs.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://pyt.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lxw.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfq.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tpa.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://afa.jinqigufen.top

[F11] 复制与移动文件
来源：http://orc.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nmx.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ryl.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fli.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqy.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ywo.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tkx.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dix.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ora.9152youxi.cn

[F12] CSV 读写
来源：http://rco.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fvn.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://umf.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kle.meibo888.top

TS:   // 同上
来源：http://ohe.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wjo.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ibm.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gqw.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://uab.zhoulong.xyz

================================================================================
来源：http://glw.yuanzhike.top

G. 面向对象
来源：http://xow.ybcxt.top

================================================================================
来源：http://vjt.jinghuilouyu.cn

[G01] 定义类
来源：http://byt.fengsongda.top

Py:   class User: pass
来源：http://cbo.shzxlz.cn

PHP:  class User {}
来源：http://mxo.mhx1999.top

JS:   class User {}
来源：http://qqy.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://ese.gogol.net.cn

Java: class User {}
来源：http://ewh.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://jno.shuidangran.top

Ruby: class User; end
来源：http://odf.kuanghao11.cn

C#:   class User {}
来源：http://vsy.cashguo.top

[G02] 构造函数
来源：http://xnw.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://wrt.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://pai.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://let.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://sfu.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://gkk.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wpl.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://huv.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://iuq.sweek.top

[G03] 实例属性
来源：http://yaq.aibaodan.cn

Py:   self.name = "x"
来源：http://cvu.jyoumei.cn

PHP:  public string $name = "x";
来源：http://rxf.yfazqb.com

JS:   this.name = "x";
来源：http://xue.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://uxt.shangyingyoupin.top

Java: private String name;
来源：http://uva.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zdj.sweek.top

Ruby: @name = "x"
来源：http://kce.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://rsl.9152youxi.cn

[G04] 定义方法
来源：http://lhw.c1oappe.top

Py:   def greet(self): return self.name
来源：http://wvz.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vkh.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://oot.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://psr.yongpay.top

Java: String greet() { return name; }
来源：http://qsy.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://osx.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://bgv.daxiang520.top

C#:   public string Greet() => Name;
来源：http://cyq.0kj1m.cn

[G05] 继承
来源：http://gvl.9152youxi.cn

Py:   class Admin(User): pass
来源：http://saw.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://kdn.iojbl.cn

JS:   class Admin extends User {}
来源：http://hup.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://diu.guannengcc.top

Java: class Admin extends User {}
来源：http://zra.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rdl.ivvv.top

Ruby: class Admin < User; end
来源：http://fde.ydzc1.top

C#:   class Admin : User {}
来源：http://grl.yanxiufei.cn

[G06] 重写方法
来源：http://ikw.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://ltj.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://nkh.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://glw.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://rph.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://ade.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rhp.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://lfa.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://mxd.chenzaomai.com

[G07] 调用父类方法
来源：http://wpj.yanxiufei.cn

Py:   super().greet()
来源：http://ito.jqgufenzy.top

PHP:  parent::greet();
来源：http://ahx.gotoacloud.top

JS:   super.greet();
来源：http://kqc.zhaomingkeji.xyz

TS:   super.greet();
来源：http://dnx.daxiang520.top

Java: super.greet();
来源：http://ach.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gya.yfazqb.com

Ruby: super
来源：http://rfu.zdqjudy.top

C#:   base.Greet();
来源：http://bbo.xziqi.cn

[G08] 静态方法与属性
来源：http://fha.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wiv.cqqwz.cn

PHP:  public static function f() {}
来源：http://eas.tanke756.top

JS:   static f() {}
来源：http://agp.birdmap.top

TS:   static f(): void {}
来源：http://oay.hongshengwenyu.top

Java: static void f() {}
来源：http://efa.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://equ.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://lui.meibo888.top

C#:   public static void F() {}
来源：http://eox.bjfxy.top

[G09] 接口 / 抽象类
来源：http://mrs.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://ulm.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://irj.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://yms.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://qlf.vehdjk.com

Java: interface Shape { double area(); }
来源：http://vla.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://awn.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tbd.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://lvr.vehdjk.com

[G10] 访问控制
来源：http://ems.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://abd.daria6918.cn

PHP:  public / protected / private
来源：http://zud.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://bdu.fehbvm.com

TS:   public / protected / private
来源：http://oyi.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://bll.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pbc.ehwqpu.com

Ruby: public / protected / private
来源：http://ngf.hnqzz.top

C#:   public / protected / private / internal
来源：http://hho.gogol.net.cn

[G11] getter / setter
来源：http://tac.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://afi.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://isi.c1oappe.top

JS:   get name() { return this._name; }
来源：http://jbk.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://okr.yj20258888.top

Java: public String getName() { return name; }
来源：http://cyh.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tyw.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://jgv.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://smr.epnwcf.com

[G12] 对象转字符串
来源：http://ibr.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://wqv.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tgq.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://nlw.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://dkl.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://mxj.cashguo.top


<!-- 参考信息 -->