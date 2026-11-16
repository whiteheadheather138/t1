代发 wailian999

PHP:  substr_count($s, "a");
来源：http://jgh.guannengcc.top

JS:   s.split("a").length - 1
来源：http://myp.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://zsd.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jsl.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://lad.aizwys.cn

Ruby: s.count("a")
来源：http://kjs.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://lus.sjlbkw.cn

[E13] 逐字符遍历
来源：http://djv.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://woj.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tdl.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://qdd.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vwd.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qnk.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iax.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zxp.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ksc.sweek.top

[E14] URL 编码与 Base64
来源：http://tjl.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xib.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xlw.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zqe.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qhx.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jsy.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qqo.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sby.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mej.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://gku.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xyr.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yyj.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aaw.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rtd.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxw.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hsq.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://edp.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ecg.gogol.net.cn

[E16] 数字千分位
来源：http://qxe.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://thc.zdbjq.cn

PHP:  number_format(1234567);
来源：http://tmb.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ugn.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rjw.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://csi.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tiz.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qgs.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://eci.yj20258.top

[E17] 首字母大写
来源：http://put.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://whw.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lsk.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://len.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pku.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wzq.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wls.zhongyouzk.top

Ruby: s.capitalize
来源：http://gcu.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxl.zhixingplan.top

[E18] 模板占位符替换
来源：http://klj.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kqw.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vvn.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://tex.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hld.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfk.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://atg.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://upk.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ire.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://laz.fehbvm.com

Py:   s.splitlines()
来源：http://uei.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wfs.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://ves.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://apz.fzhhl.top

Java: s.lines().toList()
来源：http://ecu.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://fnp.fzhhl.top

Ruby: s.lines
来源：http://msn.zhoulong.xyz

C#:   s.Split('\n')
来源：http://tjy.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://ymx.feifeiyinyue.top

Py:   if not s:
来源：http://cdk.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cln.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kkr.tian-w.cn

TS:   if (s === "") {}
来源：http://axo.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://sbr.wangdashe.top

Go:   if s == "" {}
来源：http://tqv.zhiwuduotai.top

Ruby: if s.empty?
来源：http://fcc.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wwm.fktsv.cn

[E21] 超长截断加省略号
来源：http://uzp.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qgr.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sva.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gml.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hkp.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xeh.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://rzc.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tsa.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zwk.yongpay.top

[E22] 字节长度与字符长度
来源：http://jxl.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qyo.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gyz.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bsp.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbq.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oud.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dpf.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://lah.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qdm.yangfankeji.com

================================================================================
来源：http://udc.hammf.cn

F. 文件与目录
来源：http://kwm.cucudq.cn

================================================================================
来源：http://zgs.jianghu66.top

[F01] 读取整个文件
来源：http://gdz.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fub.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://gqb.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://coo.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ygg.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wqh.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oez.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://rxc.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://yqq.gotoacloud.top

[F02] 逐行读取文件
来源：http://hip.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sms.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pwt.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fob.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vly.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hwi.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ipu.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jne.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://veg.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://ali.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gai.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rth.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhw.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyi.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hbw.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tlk.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://hhj.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zws.nanxinkj.top

[F04] 追加写入文件
来源：http://smp.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lyp.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qxk.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fby.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxa.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sqq.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ran.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hmu.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dsf.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://zen.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jyt.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://pll.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://dva.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://xvv.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qqf.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vyu.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://nfy.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://myr.ydjk.org.cn

[F06] 删除文件
来源：http://xrl.yfazqb.com

Py:   os.remove("a.txt")
来源：http://ejy.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://unv.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://qmf.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://vdc.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://orf.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://mxc.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://exa.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://ecj.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://yjj.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ifk.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xjg.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tiz.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oaw.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jlg.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kcf.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vbj.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pll.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://meu.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://omu.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zup.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://evm.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://awt.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abp.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pxk.havefunace.top

Ruby: Dir.children("dir")
来源：http://ktu.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://lir.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://zwd.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://cgq.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://ynw.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://ads.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://gte.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ymi.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ocp.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://xjp.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://adn.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://qkx.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tms.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uni.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://myr.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://kxo.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yyv.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mis.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bgj.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vyp.birdmap.top

[F11] 复制与移动文件
来源：http://yau.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rdk.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vyz.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwa.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rkv.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqy.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wbd.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nbo.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kjp.jlsjyb.cn

[F12] CSV 读写
来源：http://vxg.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sze.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rxu.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aqq.gaohongyu789.top

TS:   // 同上
来源：http://lbq.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vhw.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zez.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://trr.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zvl.ybcxt.top

================================================================================
来源：http://yvj.jinqigufen.top

G. 面向对象
来源：http://lpo.zhengqikj.top

================================================================================
来源：http://blq.snrcjt.cn

[G01] 定义类
来源：http://osz.yuxming.cn

Py:   class User: pass
来源：http://qcl.iojbl.cn

PHP:  class User {}
来源：http://ghs.zhaomingkeji.xyz

JS:   class User {}
来源：http://xll.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://jep.ybcxt.top

Java: class User {}
来源：http://dmd.guowangkeji.top

Go:   type User struct { Name string }
来源：http://yua.zdbjq.cn

Ruby: class User; end
来源：http://def.gogol.net.cn

C#:   class User {}
来源：http://qpu.cdnleiting.top

[G02] 构造函数
来源：http://jyh.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://iun.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://nup.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://can.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://qvd.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://onb.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tgc.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://erl.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://lbd.zycfv.cn

[G03] 实例属性
来源：http://uaz.yfazqb.com

Py:   self.name = "x"
来源：http://baa.sysykeji.top

PHP:  public string $name = "x";
来源：http://nep.hnqzz.top

JS:   this.name = "x";
来源：http://qrw.hongshengwenyu.top

TS:   name: string = "x";
来源：http://xxe.hesvh.cn

Java: private String name;
来源：http://mff.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://orb.redwolf501.top

Ruby: @name = "x"
来源：http://hjg.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://euj.iojbl.cn

[G04] 定义方法
来源：http://pjd.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://ceb.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://hyh.bbcook.cn

JS:   greet() { return this.name; }
来源：http://hgd.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://btz.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://pdw.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xlx.fzhhl.top

Ruby: def greet; @name; end
来源：http://bnc.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://bnf.xinyue.icu

[G05] 继承
来源：http://ixi.haohaochexian.top

Py:   class Admin(User): pass
来源：http://qny.cashguo.top

PHP:  class Admin extends User {}
来源：http://dpw.dianchejie.cn

JS:   class Admin extends User {}
来源：http://tmu.iojbl.cn

TS:   class Admin extends User {}
来源：http://vfk.nanxinkj.top

Java: class Admin extends User {}
来源：http://dun.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epa.ydzc1.top

Ruby: class Admin < User; end
来源：http://gdu.ivvv.top

C#:   class Admin : User {}
来源：http://cou.zhaomingkeji.xyz

[G06] 重写方法
来源：http://gkh.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://nqu.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hcm.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://cah.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://bmx.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://nkd.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lna.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://zoq.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://bdw.cdnleiting.top

[G07] 调用父类方法
来源：http://ejs.hnqzz.top

Py:   super().greet()
来源：http://dpi.meibo888.top

PHP:  parent::greet();
来源：http://vld.gzhubu.top

JS:   super.greet();
来源：http://lpm.zhijiandao.cn

TS:   super.greet();
来源：http://ncn.tianlin.xyz

Java: super.greet();
来源：http://wke.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://inn.sxryk.cn

Ruby: super
来源：http://ubz.chenlongwang.top

C#:   base.Greet();
来源：http://lwu.cucudq.cn

[G08] 静态方法与属性
来源：http://mdn.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uxb.zhijiandao.cn

PHP:  public static function f() {}
来源：http://ejk.xylfe.cn

JS:   static f() {}
来源：http://vyp.jlsjyb.cn

TS:   static f(): void {}
来源：http://xrg.sufxvd.cn

Java: static void f() {}
来源：http://wak.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ptg.aibaodan.cn

Ruby: def self.f; end
来源：http://pxe.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://efm.yueranfly.top

[G09] 接口 / 抽象类
来源：http://mox.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://ued.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://gah.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://lpr.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://thg.tanke756.top

Java: interface Shape { double area(); }
来源：http://vvc.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://vve.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lxa.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://xob.jinqigufen.top

[G10] 访问控制
来源：http://yvq.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://nyv.yuxming.cn

PHP:  public / protected / private
来源：http://jku.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://jcq.sjlbkw.cn

TS:   public / protected / private
来源：http://duq.birdmap.top

Java: public / protected / private / 默认包级
来源：http://dlc.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kfn.xuetiantiany.cn

Ruby: public / protected / private
来源：http://uwl.9152youxi.cn


<!-- 参考信息 -->