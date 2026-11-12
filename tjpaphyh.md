代发 wailian999

[E14] URL 编码与 Base64
来源：http://rlf.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://egx.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jje.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lyo.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vzr.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ibl.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qhv.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kjm.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gni.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://xfi.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qub.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xfe.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://koy.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kez.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ies.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbd.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zyy.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uqj.chenjidiqi.icu

[E16] 数字千分位
来源：http://xyt.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://nft.yfazqb.com

PHP:  number_format(1234567);
来源：http://zxg.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fuo.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tow.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://krn.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rcr.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dyn.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://evq.pengpengdd.cyou

[E17] 首字母大写
来源：http://rao.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsa.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://evz.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qpf.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnb.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpb.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cpm.shzxlz.cn

Ruby: s.capitalize
来源：http://vut.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cya.yuanzhike.top

[E18] 模板占位符替换
来源：http://pbx.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://arh.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://giw.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ozl.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qkp.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://csp.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xby.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jeh.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dpo.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://jrn.dashuyun.cn

Py:   s.splitlines()
来源：http://fnd.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lsp.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://qvp.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://sut.316326.xyz

Java: s.lines().toList()
来源：http://yhb.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://rji.epnwcf.com

Ruby: s.lines
来源：http://hqi.zdbjq.cn

C#:   s.Split('\n')
来源：http://ddy.sysykeji.top

[E20] 判断字符串是否为空
来源：http://jbt.ppjwa.cn

Py:   if not s:
来源：http://mti.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yue.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hnk.ydzc1.top

TS:   if (s === "") {}
来源：http://kgl.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://stz.fktsv.cn

Go:   if s == "" {}
来源：http://qlt.tarul.cn

Ruby: if s.empty?
来源：http://ebe.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nky.hywenlv.cn

[E21] 超长截断加省略号
来源：http://sms.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://grk.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kxn.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jip.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wpv.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dxz.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://zjq.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nfg.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivj.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://zuf.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nhc.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jyv.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://khp.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqj.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jrt.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sya.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://qjo.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nyt.sweek.top

================================================================================
来源：http://pvz.cheryme.top

F. 文件与目录
来源：http://gcg.nanxuanxn.top

================================================================================
来源：http://sab.xinyue.icu

[F01] 读取整个文件
来源：http://ppx.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wdq.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://sjk.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uag.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jsy.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fap.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nis.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://bcy.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://nsv.jinqigufen.top

[F02] 逐行读取文件
来源：http://mqr.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ats.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yzw.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://igb.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pck.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://spf.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ypc.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://apx.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hvb.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://bbh.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ggf.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rpo.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pae.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpl.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xnd.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hxl.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://nap.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cty.jyoumei.cn

[F04] 追加写入文件
来源：http://nfi.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ulg.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uke.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gad.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://can.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pra.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oat.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcn.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cxm.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://cbm.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vzu.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://myb.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://mdu.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://nwr.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tes.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vkb.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://ezt.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://dtw.sweek.top

[F06] 删除文件
来源：http://nxc.gzhubu.top

Py:   os.remove("a.txt")
来源：http://gmx.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://hon.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://hmq.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://hkz.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jix.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://pod.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://gtm.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://kua.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://mnq.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://owz.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yfe.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhx.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvn.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://luz.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qqo.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rva.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jqn.fktsv.cn

[F08] 遍历目录
来源：http://cnn.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pgl.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mah.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://myw.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://nie.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vwc.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dcc.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://udq.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://ycr.hcnkem.com

[F09] 获取文件大小
来源：http://ueh.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://hns.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://zvd.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://fvy.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://msn.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yyj.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mtf.nwbrower.top

Ruby: File.size("a.txt")
来源：http://hib.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://jxo.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://nbj.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nvb.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://avw.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xxh.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://asg.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ulg.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wwz.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cdo.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kme.yangfankeji.com

[F11] 复制与移动文件
来源：http://obi.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lqz.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tab.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://irk.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyo.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iyf.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qfb.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ssx.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zkb.yonumen.top

[F12] CSV 读写
来源：http://eip.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rhj.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tni.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wrz.hnqzz.top

TS:   // 同上
来源：http://szj.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wmr.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lyf.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zzj.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://aul.xuanzx.com

================================================================================
来源：http://bew.ydzc1.top

G. 面向对象
来源：http://qnm.yj202588.top

================================================================================
来源：http://fhz.vqdsnc.cn

[G01] 定义类
来源：http://lio.snrcjt.cn

Py:   class User: pass
来源：http://rrj.zdbjq.cn

PHP:  class User {}
来源：http://zki.hesvh.cn

JS:   class User {}
来源：http://ymy.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://goh.aizwys.cn

Java: class User {}
来源：http://ere.shuidangran.top

Go:   type User struct { Name string }
来源：http://iis.tanke756.top

Ruby: class User; end
来源：http://uxx.fehbvm.com

C#:   class User {}
来源：http://mlo.mhx1999.top

[G02] 构造函数
来源：http://vql.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://yhm.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://ugi.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://ijt.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://qdp.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://kaf.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rpm.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://wop.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://htc.xylfe.cn

[G03] 实例属性
来源：http://vqq.haohaochexian.top

Py:   self.name = "x"
来源：http://jyq.gotoacloud.top

PHP:  public string $name = "x";
来源：http://yfy.jinqigufen.top

JS:   this.name = "x";
来源：http://ipq.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://uvd.nwbrower.top

Java: private String name;
来源：http://tmm.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ime.0kj1m.cn

Ruby: @name = "x"
来源：http://ejl.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ohe.xuetiantiany.cn

[G04] 定义方法
来源：http://bcu.pycfn.com

Py:   def greet(self): return self.name
来源：http://vkk.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://klp.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://axo.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://nbl.zhongyouzk.top

Java: String greet() { return name; }
来源：http://xpm.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gwn.vehdjk.com

Ruby: def greet; @name; end
来源：http://yuq.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://slo.yonumen.top

[G05] 继承
来源：http://kww.shuidangran.top

Py:   class Admin(User): pass
来源：http://uxp.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://rjl.sxryk.cn

JS:   class Admin extends User {}
来源：http://yji.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://vfw.vqdsnc.cn

Java: class Admin extends User {}
来源：http://tly.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://coe.tian-w.cn

Ruby: class Admin < User; end
来源：http://czb.zhijiandao.cn

C#:   class Admin : User {}
来源：http://mwl.yonumen.top

[G06] 重写方法
来源：http://vmf.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://bkr.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vmt.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://jhp.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://szo.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://lzd.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jak.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://lea.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://nqv.316326.xyz

[G07] 调用父类方法
来源：http://jkl.nanxuanxn.top

Py:   super().greet()
来源：http://dvj.meibo888.top

PHP:  parent::greet();
来源：http://mvr.tanke756.top

JS:   super.greet();
来源：http://jnw.meibo888.top

TS:   super.greet();
来源：http://atg.fehbvm.com

Java: super.greet();
来源：http://juv.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hrx.shanyushiyangtech.top

Ruby: super
来源：http://jxt.cucudq.cn

C#:   base.Greet();
来源：http://zjh.vqdsnc.cn

[G08] 静态方法与属性
来源：http://ffk.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://szy.yj202588.top

PHP:  public static function f() {}
来源：http://azk.fktsv.cn

JS:   static f() {}
来源：http://utr.yuxming.cn

TS:   static f(): void {}
来源：http://kng.daxiang520.top

Java: static void f() {}
来源：http://lly.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dgy.yangfankeji.com

Ruby: def self.f; end
来源：http://dtu.yuanzhike.top

C#:   public static void F() {}
来源：http://xvt.tanke756.top

[G09] 接口 / 抽象类
来源：http://wme.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://wwd.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://qfp.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qmj.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://bgs.jianghu66.top

Java: interface Shape { double area(); }
来源：http://mct.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://omm.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxk.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://evs.ehwqpu.com

[G10] 访问控制
来源：http://uwj.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://bec.xylfe.cn

PHP:  public / protected / private
来源：http://mdc.hnqzz.top

JS:   #private 字段；其余公开
来源：http://wuy.jianghu66.top

TS:   public / protected / private
来源：http://mrc.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://utj.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fvx.nwbrower.top

Ruby: public / protected / private
来源：http://ard.yuxming.cn

C#:   public / protected / private / internal
来源：http://kla.hongshengwenyu.top

[G11] getter / setter
来源：http://dxd.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://mjg.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://gfq.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ygl.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://zoe.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://txn.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://suk.cucudq.cn

Ruby: attr_accessor :name
来源：http://rwh.fengsongda.top

C#:   public string Name { get; set; }
来源：http://okz.0kj1m.cn

[G12] 对象转字符串
来源：http://dwn.yonumen.top

Py:   def __str__(self): return self.name
来源：http://zwi.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vyu.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://rpz.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://knm.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://eyz.iojbl.cn


<!-- 参考信息 -->