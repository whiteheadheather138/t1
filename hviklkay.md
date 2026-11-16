代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vgo.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vgy.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uqs.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hqe.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://hss.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jeq.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://hxe.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ors.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nkq.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qxn.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yuh.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cvz.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sqa.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://eaf.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sfx.smart0.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qqc.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dnz.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://otn.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jef.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rey.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ocx.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yqq.xylfe.cn

[E16] 数字千分位
来源：http://mhi.gzhubu.top

Py:   f"{1234567:,}"
来源：http://kkf.daria6918.cn

PHP:  number_format(1234567);
来源：http://olx.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://cyq.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://eqt.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jmo.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://veo.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ewx.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://lzs.shzxlz.cn

[E17] 首字母大写
来源：http://qjx.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qft.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ddo.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqy.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltb.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsu.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kof.fehbvm.com

Ruby: s.capitalize
来源：http://dpo.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xyt.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://hbe.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fok.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qsg.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://arn.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://usb.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cqx.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qkb.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jrl.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hfq.wangdashe.top

[E19] 多行文本按行拆分
来源：http://qai.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://nhn.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwy.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://aoc.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://jdq.meibo888.top

Java: s.lines().toList()
来源：http://cju.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://hwv.sufxvd.cn

Ruby: s.lines
来源：http://pdi.hywenlv.cn

C#:   s.Split('\n')
来源：http://cfx.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://riw.iojbl.cn

Py:   if not s:
来源：http://kdg.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mmx.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bqt.yvedp.cn

TS:   if (s === "") {}
来源：http://sdg.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://brs.yj20258888.top

Go:   if s == "" {}
来源：http://qck.sweek.top

Ruby: if s.empty?
来源：http://bwz.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nhc.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://fba.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://psd.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://byo.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzu.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ypc.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vmr.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://wmp.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dtg.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xzw.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://asb.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mde.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ffk.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://paa.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bnp.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qtm.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kcn.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://omm.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xdk.yangfankeji.com

================================================================================
来源：http://lqg.pycfn.com

F. 文件与目录
来源：http://jlg.hesvh.cn

================================================================================
来源：http://sfr.pycfn.com

[F01] 读取整个文件
来源：http://ewo.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jaq.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://mhc.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pai.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://swm.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eeq.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://txz.316326.xyz

Ruby: File.read("a.txt")
来源：http://jll.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://fgk.svipenyu.cn

[F02] 逐行读取文件
来源：http://xsd.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://opz.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uye.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpo.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lti.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xzk.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oud.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tck.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://maq.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://spp.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bic.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zqp.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofo.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ydq.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://spk.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fgu.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://img.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pwq.chenzaomai.com

[F04] 追加写入文件
来源：http://myx.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nno.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ylq.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eet.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hza.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nxh.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhm.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ikz.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://egb.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://bqr.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vwj.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://ywu.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://zfu.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://tas.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cow.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ghd.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://zrd.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://dxj.meibo888.top

[F06] 删除文件
来源：http://dna.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://ata.wangdashe.top

PHP:  unlink("a.txt");
来源：http://eww.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://qrl.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://wfd.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dkn.cheryme.top

Go:   os.Remove("a.txt")
来源：http://xld.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://ana.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://mxe.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://nta.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ukt.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://viv.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upc.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://evv.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aqv.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ldm.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nvw.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://efw.yj202588.top

[F08] 遍历目录
来源：http://hap.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://epp.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://noa.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://auh.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://exr.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cbs.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qwf.nwbrower.top

Ruby: Dir.children("dir")
来源：http://akk.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://jim.jlsjyb.cn

[F09] 获取文件大小
来源：http://myb.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://agk.jianghu66.top

PHP:  filesize("a.txt");
来源：http://uee.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://xoc.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://pfq.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://des.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sqo.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://vdu.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://icf.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://kch.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vkv.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tlz.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jyt.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://ghg.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gxq.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pce.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fhr.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://agu.chenlongwang.top

[F11] 复制与移动文件
来源：http://uiu.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fxg.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mia.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bsr.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqw.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ciy.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://txq.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://alh.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mim.dashuyun.cn

[F12] CSV 读写
来源：http://air.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qbb.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://avw.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rah.jianghu66.top

TS:   // 同上
来源：http://zom.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lnd.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vou.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ehk.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uxu.yanxiufei.cn

================================================================================
来源：http://jlh.kuanghao11.cn

G. 面向对象
来源：http://gyf.feifeiyinyue.top

================================================================================
来源：http://yvt.shangyingyoupin.top

[G01] 定义类
来源：http://uvz.bbcook.cn

Py:   class User: pass
来源：http://mpb.chenzaomai.com

PHP:  class User {}
来源：http://pfh.zhoulong.xyz

JS:   class User {}
来源：http://htu.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://twd.shangyingyoupin.top

Java: class User {}
来源：http://klk.xuanzx.com

Go:   type User struct { Name string }
来源：http://xdw.ppjwa.cn

Ruby: class User; end
来源：http://hbn.ydzc1.top

C#:   class User {}
来源：http://emo.yuxming.cn

[G02] 构造函数
来源：http://gow.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://yya.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://zbc.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://skv.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://ygl.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://tyq.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oyh.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://bfr.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://ekn.ybcxt.top

[G03] 实例属性
来源：http://gye.jyoumei.cn

Py:   self.name = "x"
来源：http://kqc.birdmap.top

PHP:  public string $name = "x";
来源：http://tna.yangfankeji.com

JS:   this.name = "x";
来源：http://gqh.yangfankeji.com

TS:   name: string = "x";
来源：http://vvk.feifeiyinyue.top

Java: private String name;
来源：http://wdh.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jel.ydjk.org.cn

Ruby: @name = "x"
来源：http://ceg.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://bcc.pengpengdd.cyou

[G04] 定义方法
来源：http://eqq.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://okt.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://iab.fengsongda.top

JS:   greet() { return this.name; }
来源：http://fmp.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://wrs.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://rkh.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hgt.smart0.xyz

Ruby: def greet; @name; end
来源：http://abk.hammf.cn

C#:   public string Greet() => Name;
来源：http://fmz.yj20258.top

[G05] 继承
来源：http://amt.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://hor.wangdashe.top

PHP:  class Admin extends User {}
来源：http://txt.tarul.cn

JS:   class Admin extends User {}
来源：http://qmb.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://esy.jqgufenzy.top

Java: class Admin extends User {}
来源：http://ovl.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dsl.ppjwa.cn

Ruby: class Admin < User; end
来源：http://wkl.guannengcc.top

C#:   class Admin : User {}
来源：http://ika.jqgufenzy.top

[G06] 重写方法
来源：http://oah.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://fdo.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ivu.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://uyc.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://rlj.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://xnj.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vae.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://ngt.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://eaz.zhongyouzk.top

[G07] 调用父类方法
来源：http://vcd.hongshengwenyu.top

Py:   super().greet()
来源：http://kns.gogol.net.cn

PHP:  parent::greet();
来源：http://kqm.yfazqb.com

JS:   super.greet();
来源：http://wbl.9152youxi.cn

TS:   super.greet();
来源：http://vcv.tanke756.top

Java: super.greet();
来源：http://kek.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzy.chenjidiqi.icu

Ruby: super
来源：http://epz.xziqi.cn

C#:   base.Greet();
来源：http://ngj.xuanzx.com

[G08] 静态方法与属性
来源：http://amw.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rlm.bbcook.cn

PHP:  public static function f() {}
来源：http://pqj.0kj1m.cn

JS:   static f() {}
来源：http://lvt.uphjek.com

TS:   static f(): void {}
来源：http://eaf.jiagoushi.top

Java: static void f() {}
来源：http://ceb.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xny.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://ddm.fehbvm.com

C#:   public static void F() {}
来源：http://ldm.iojbl.cn

[G09] 接口 / 抽象类
来源：http://bxg.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://sci.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://kiu.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ltv.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://mio.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://kjp.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://omc.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zpn.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://cle.smart0.xyz

[G10] 访问控制
来源：http://zln.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://swi.daria6918.cn

PHP:  public / protected / private
来源：http://kdc.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://ekp.ppjwa.cn

TS:   public / protected / private
来源：http://eno.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://jni.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pwe.smart0.xyz

Ruby: public / protected / private
来源：http://xer.sxryk.cn

C#:   public / protected / private / internal
来源：http://ojo.tarul.cn

[G11] getter / setter
来源：http://ryg.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://xei.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rea.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://aoa.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://wze.sxryk.cn

Java: public String getName() { return name; }
来源：http://dzp.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ycx.xziqi.cn

Ruby: attr_accessor :name
来源：http://neg.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://rtl.cucudq.cn

[G12] 对象转字符串
来源：http://cqn.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://auu.gogol.net.cn


<!-- 参考信息 -->