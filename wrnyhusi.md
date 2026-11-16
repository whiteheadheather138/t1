代发 wailian999

Ruby: s.reverse
来源：http://bpz.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://ohk.yj20258.top

[E12] 统计某字符出现次数
来源：http://tze.pycfn.com

Py:   s.count("a")
来源：http://exx.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://cfl.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://jnm.cucudq.cn

TS:   s.split("a").length - 1
来源：http://jmt.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mmo.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://hmi.wangshuangyany.cn

Ruby: s.count("a")
来源：http://grf.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://wjc.gaohongyu789.top

[E13] 逐字符遍历
来源：http://qbj.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://aaf.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zhh.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kps.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ign.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qev.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcr.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xxa.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bff.guannengcc.top

[E14] URL 编码与 Base64
来源：http://jog.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mni.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://puf.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://imd.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fqh.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fjc.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zuq.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oyh.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://icx.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://xlu.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lyf.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vej.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tjf.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nuo.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wwa.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uzi.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vgr.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jxm.yj20258888.top

[E16] 数字千分位
来源：http://kle.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://phz.guowangkeji.top

PHP:  number_format(1234567);
来源：http://gkv.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ljd.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xbk.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ftf.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yng.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oge.316326.xyz

C#:   1234567.ToString("N0")
来源：http://opz.yuanzhike.top

[E17] 首字母大写
来源：http://ncm.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iaj.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://agb.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ftv.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fob.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://prr.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tvd.fktsv.cn

Ruby: s.capitalize
来源：http://pvu.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sll.yfazqb.com

[E18] 模板占位符替换
来源：http://zbn.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vgi.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zvm.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vow.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ege.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dwu.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ypz.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ivg.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pjr.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://wnu.jqgufenzy.top

Py:   s.splitlines()
来源：http://mix.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pnw.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://mrf.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://iat.yonumen.top

Java: s.lines().toList()
来源：http://yyi.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://efg.yonumen.top

Ruby: s.lines
来源：http://ocx.bbcook.cn

C#:   s.Split('\n')
来源：http://mfx.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://xad.sufxvd.cn

Py:   if not s:
来源：http://bje.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://due.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ont.ctjpmb.com

TS:   if (s === "") {}
来源：http://zvo.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://vdk.0kj1m.cn

Go:   if s == "" {}
来源：http://oco.jlsjyb.cn

Ruby: if s.empty?
来源：http://rug.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yph.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://srv.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dpb.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ywc.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cou.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndw.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tfo.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://vqe.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://niv.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azb.redwolf501.top

[E22] 字节长度与字符长度
来源：http://abc.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cox.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfj.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvc.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://irv.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://utl.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wpt.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://qwz.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yuk.shanyushiyangtech.top

================================================================================
来源：http://bwe.ywan-chungtsiang.top

F. 文件与目录
来源：http://ria.gogol.net.cn

================================================================================
来源：http://tyw.hongshengwenyu.top

[F01] 读取整个文件
来源：http://qkx.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jfq.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://oad.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kbs.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://frv.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iuv.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vei.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://gzd.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://rvw.quarkkingdee.top

[F02] 逐行读取文件
来源：http://enb.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wgy.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ght.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nau.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgu.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wov.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ufm.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://frb.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gay.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://cfe.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wek.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://trr.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dds.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jpl.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dgr.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sof.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://xfl.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ecu.0kj1m.cn

[F04] 追加写入文件
来源：http://jgz.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://idz.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxt.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ajz.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpo.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dqm.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mih.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mhh.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://phj.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://ecb.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdw.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://jzx.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://khb.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://pjp.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pco.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iok.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://ndh.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://szf.shangyingyoupin.top

[F06] 删除文件
来源：http://qhv.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://dmt.shuidangran.top

PHP:  unlink("a.txt");
来源：http://bee.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://mkn.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://bpo.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wzc.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://lcs.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://hrz.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://dzg.daxiang520.top

[F07] 创建目录（含多级）
来源：http://rqi.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rgi.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pcw.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iul.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkh.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oat.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://swy.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gpz.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kwu.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://hmx.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://sdp.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zih.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://sdi.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://udb.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dxa.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cml.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://wyu.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://ddd.jqgfzy.top

[F09] 获取文件大小
来源：http://svb.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://jbw.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://ure.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://vvb.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://taf.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://gpj.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nhm.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://qbg.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://aot.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://mzq.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hug.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kom.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://opv.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://acz.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://and.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hym.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rps.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://olf.sweek.top

[F11] 复制与移动文件
来源：http://xnd.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wfd.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ioz.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pps.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yqc.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iar.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://prd.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blm.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lcu.uphjek.com

[F12] CSV 读写
来源：http://bji.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tzv.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cod.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bdq.yuanzhike.top

TS:   // 同上
来源：http://bxv.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wzo.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugv.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uae.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oia.shuidangran.top

================================================================================
来源：http://dvs.feifeiyinyue.top

G. 面向对象
来源：http://haj.epnwcf.com

================================================================================
来源：http://dmk.hnqzz.top

[G01] 定义类
来源：http://hdn.daxiang520.top

Py:   class User: pass
来源：http://ltb.fzhhl.top

PHP:  class User {}
来源：http://cyh.epnwcf.com

JS:   class User {}
来源：http://fxb.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://tuy.iojbl.cn

Java: class User {}
来源：http://peo.ctjpmb.com

Go:   type User struct { Name string }
来源：http://iyy.bjfxy.top

Ruby: class User; end
来源：http://dxa.pengpengdd.cyou

C#:   class User {}
来源：http://vge.jlsjyb.cn

[G02] 构造函数
来源：http://ftr.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://mgl.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://dvl.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://kbn.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://ujg.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://mjl.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://stc.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://qxe.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ocg.fktsv.cn

[G03] 实例属性
来源：http://qkg.jinqigufen.top

Py:   self.name = "x"
来源：http://fcn.hfpthk.cn

PHP:  public string $name = "x";
来源：http://kle.wangdashe.top

JS:   this.name = "x";
来源：http://ukb.jqgufenzy.top

TS:   name: string = "x";
来源：http://wnp.zdqjudy.top

Java: private String name;
来源：http://daj.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mlt.cqqwz.cn

Ruby: @name = "x"
来源：http://kbt.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://ueq.sweek.top

[G04] 定义方法
来源：http://mvh.yj202588.top

Py:   def greet(self): return self.name
来源：http://nzh.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zpq.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://euw.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://ubd.smart0.xyz

Java: String greet() { return name; }
来源：http://olw.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mhk.fzhhl.top

Ruby: def greet; @name; end
来源：http://kip.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://kdn.yj20258.top

[G05] 继承
来源：http://pcq.gogol.net.cn

Py:   class Admin(User): pass
来源：http://dvn.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://csd.mhx1999.top

JS:   class Admin extends User {}
来源：http://fbc.tarul.cn

TS:   class Admin extends User {}
来源：http://ucu.meibo888.top

Java: class Admin extends User {}
来源：http://zrg.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jpz.xylfe.cn

Ruby: class Admin < User; end
来源：http://djg.ydzc1.top

C#:   class Admin : User {}
来源：http://tqg.jinqigfzy.top

[G06] 重写方法
来源：http://old.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://bth.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://upx.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://qjg.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://flt.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://fwc.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lbi.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://evc.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://oad.vqdsnc.cn

[G07] 调用父类方法
来源：http://ono.aizwys.cn

Py:   super().greet()
来源：http://vlh.yangfankeji.com

PHP:  parent::greet();
来源：http://xfs.hammf.cn

JS:   super.greet();
来源：http://ixd.ivvv.top

TS:   super.greet();
来源：http://gai.jqgufenzy.top

Java: super.greet();
来源：http://lxz.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlg.mhx1999.top

Ruby: super
来源：http://lsm.quarkkingdee.top

C#:   base.Greet();
来源：http://guh.cqqwz.cn

[G08] 静态方法与属性
来源：http://ocy.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hku.yangfankeji.com

PHP:  public static function f() {}
来源：http://ubo.birdmap.top

JS:   static f() {}
来源：http://hdh.wangshuangyany.cn

TS:   static f(): void {}
来源：http://wvw.xinyue.icu

Java: static void f() {}
来源：http://azm.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hdt.smart0.xyz

Ruby: def self.f; end
来源：http://ntt.redwolf501.top

C#:   public static void F() {}
来源：http://mgu.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://ngq.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://qgt.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://ijr.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhk.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://xiz.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://idb.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://ibr.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fti.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://dli.meibo888.top

[G10] 访问控制
来源：http://tax.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://dfm.gzhubu.top

PHP:  public / protected / private
来源：http://pky.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pvy.ywan-chungtsiang.top


<!-- 参考信息 -->