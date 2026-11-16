代发 wailian999

Go:   strings.Count(s, "a")
来源：http://jbd.guannengcc.top

Ruby: s.count("a")
来源：http://rkm.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://bqw.ivvv.top

[E13] 逐字符遍历
来源：http://zkk.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://uov.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gef.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cuz.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fdu.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qnw.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xqp.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tlf.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mxn.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://mmd.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ckk.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cws.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vog.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mwf.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rnn.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blw.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wsx.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dps.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://yoq.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://qnz.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lxj.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ska.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sjt.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gle.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jfq.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bgr.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oet.jinghuilouyu.cn

[E16] 数字千分位
来源：http://eax.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://jyd.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://cph.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://tlc.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nei.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fki.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://thj.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwr.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://iuk.bjfxy.top

[E17] 首字母大写
来源：http://oka.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eje.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyj.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mzu.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xvy.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nfx.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iph.hywenlv.cn

Ruby: s.capitalize
来源：http://kne.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xvd.snrcjt.cn

[E18] 模板占位符替换
来源：http://uoa.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ldo.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gum.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yuw.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mqr.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uoe.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://efv.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vlu.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ild.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://khy.pycfn.com

Py:   s.splitlines()
来源：http://jtp.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://epb.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://vqf.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://fjg.bbcook.cn

Java: s.lines().toList()
来源：http://wek.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://sch.feifeiyinyue.top

Ruby: s.lines
来源：http://wdp.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://aan.yj202588.top

[E20] 判断字符串是否为空
来源：http://tsl.sysykeji.top

Py:   if not s:
来源：http://crf.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nzj.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pbk.tian-w.cn

TS:   if (s === "") {}
来源：http://nze.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://krd.hongshengwenyu.top

Go:   if s == "" {}
来源：http://azr.quarkkingdee.top

Ruby: if s.empty?
来源：http://xtr.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://giy.yj20258.top

[E21] 超长截断加省略号
来源：http://zbn.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ikk.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://liy.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xow.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogh.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://upd.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://yeu.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://irm.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ype.xziqi.cn

[E22] 字节长度与字符长度
来源：http://eug.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhi.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zas.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hjz.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dzo.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lsm.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ijg.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://ylw.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sft.sufxvd.cn

================================================================================
来源：http://iga.kuanghao11.cn

F. 文件与目录
来源：http://giv.tianlin.xyz

================================================================================
来源：http://dra.xziqi.cn

[F01] 读取整个文件
来源：http://fns.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lkf.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://xjl.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hqm.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nye.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xnz.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dwe.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://cts.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://gtu.uphjek.com

[F02] 逐行读取文件
来源：http://iij.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wjw.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qod.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ern.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hdq.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fol.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://poq.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nrb.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gzy.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://utc.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dzr.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ifa.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxk.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzu.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cgt.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hnm.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://bwg.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gew.smart0.xyz

[F04] 追加写入文件
来源：http://rsz.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yvv.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://drq.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xli.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://edd.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dmz.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pwb.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gld.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vyi.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://dkh.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://upv.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://apf.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://wpd.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://aoc.smart0.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://nwr.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jvp.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://xlk.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://yof.xylfe.cn

[F06] 删除文件
来源：http://sck.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://rgi.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://tqw.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nsg.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tcc.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pky.316326.xyz

Go:   os.Remove("a.txt")
来源：http://cjm.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://loe.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://dhf.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://lpr.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bbm.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://niv.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnj.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://efz.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ooe.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zal.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yxp.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://woh.shanyushiyangtech.top

[F08] 遍历目录
来源：http://ieh.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xlt.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ymg.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://ovk.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://pxr.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gft.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://oqy.hesvh.cn

Ruby: Dir.children("dir")
来源：http://ujy.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://hgj.yongpay.top

[F09] 获取文件大小
来源：http://fqz.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://kym.fehbvm.com

PHP:  filesize("a.txt");
来源：http://hqc.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://wpc.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://ehw.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xyp.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zdq.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://dol.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://gml.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://dzc.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ubb.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nci.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xcu.c1oappe.top

TS:   path.extname("a.txt")
来源：http://xgi.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jpn.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://amc.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jnl.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ljj.tarul.cn

[F11] 复制与移动文件
来源：http://pbv.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wks.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fas.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://neh.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vun.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bqz.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rmr.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ase.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uac.hywenlv.cn

[F12] CSV 读写
来源：http://avu.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tor.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kit.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://glb.shanyushiyangtech.top

TS:   // 同上
来源：http://ryl.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://inu.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rek.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tgd.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hev.tanke756.top

================================================================================
来源：http://qys.gaohongyu789.top

G. 面向对象
来源：http://hfo.guowangkeji.top

================================================================================
来源：http://dzv.ivvv.top

[G01] 定义类
来源：http://fki.ybcxt.top

Py:   class User: pass
来源：http://wuw.yj20258888.top

PHP:  class User {}
来源：http://wun.nanxinkj.top

JS:   class User {}
来源：http://lhs.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://tfp.guowangkeji.top

Java: class User {}
来源：http://brh.iojbl.cn

Go:   type User struct { Name string }
来源：http://jej.zhiwuduotai.top

Ruby: class User; end
来源：http://gyv.yangfankeji.com

C#:   class User {}
来源：http://uka.epnwcf.com

[G02] 构造函数
来源：http://tcj.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://gjy.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://gve.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://epg.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://tah.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://vfy.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ath.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jeb.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://lpt.yj20258.top

[G03] 实例属性
来源：http://aop.cheryme.top

Py:   self.name = "x"
来源：http://tri.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://sga.hammf.cn

JS:   this.name = "x";
来源：http://wsu.wangshuangyany.cn

TS:   name: string = "x";
来源：http://xah.zhijiandao.cn

Java: private String name;
来源：http://nxk.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tzp.hesvh.cn

Ruby: @name = "x"
来源：http://rph.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://hag.52xcode.cn

[G04] 定义方法
来源：http://ghv.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://lri.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://apz.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://qii.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://eek.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://ibw.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cdl.yfazqb.com

Ruby: def greet; @name; end
来源：http://mfx.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://lkr.zdbjq.cn

[G05] 继承
来源：http://lqj.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://rsd.jianghu66.top

PHP:  class Admin extends User {}
来源：http://thz.zdbjq.cn

JS:   class Admin extends User {}
来源：http://bpe.havefunace.top

TS:   class Admin extends User {}
来源：http://bek.aibaodan.cn

Java: class Admin extends User {}
来源：http://gra.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pbc.meibo888.top

Ruby: class Admin < User; end
来源：http://hwk.chenlongwang.top

C#:   class Admin : User {}
来源：http://qzf.xziqi.cn

[G06] 重写方法
来源：http://ipv.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://eoi.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rkr.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://wwi.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://eoi.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://esj.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kpq.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://ubd.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://tyz.zhongyouzk.top

[G07] 调用父类方法
来源：http://dwl.yonumen.top

Py:   super().greet()
来源：http://ldv.hnqzz.top

PHP:  parent::greet();
来源：http://bmi.ywan-chungtsiang.top

JS:   super.greet();
来源：http://cko.bbcook.cn

TS:   super.greet();
来源：http://myf.quarkkingdee.top

Java: super.greet();
来源：http://fiu.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fjw.tanke756.top

Ruby: super
来源：http://xjd.xinyue.icu

C#:   base.Greet();
来源：http://ixg.havefunace.top

[G08] 静态方法与属性
来源：http://bsc.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wtz.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://jnc.yj20258.top

JS:   static f() {}
来源：http://ngh.zhongyouzk.top

TS:   static f(): void {}
来源：http://ylp.ivvv.top

Java: static void f() {}
来源：http://ctj.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uat.cheryme.top

Ruby: def self.f; end
来源：http://wgt.xuetiantiany.cn

C#:   public static void F() {}
来源：http://mkv.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://cks.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://rwz.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://vhi.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cra.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://bfw.shuidangran.top

Java: interface Shape { double area(); }
来源：http://pia.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://opi.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ikk.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://ayl.zdqjudy.top

[G10] 访问控制
来源：http://gep.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://run.hammf.cn

PHP:  public / protected / private
来源：http://qbj.pycfn.com

JS:   #private 字段；其余公开
来源：http://qiw.ybcxt.top

TS:   public / protected / private
来源：http://amp.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://yce.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xjd.sxryk.cn

Ruby: public / protected / private
来源：http://qra.yangfankeji.com

C#:   public / protected / private / internal
来源：http://zlq.vehdjk.com

[G11] getter / setter
来源：http://fao.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://nrl.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pbg.0kj1m.cn


<!-- 参考信息 -->