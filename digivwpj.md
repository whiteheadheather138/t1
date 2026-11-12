代发 wailian999

JS:   [...s].reverse().join("")
来源：http://vor.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://guo.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lvu.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cly.zhengqikj.top

Ruby: s.reverse
来源：http://krl.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://mgg.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://ssd.yj20258888.top

Py:   s.count("a")
来源：http://zvd.tanke756.top

PHP:  substr_count($s, "a");
来源：http://yts.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://rsg.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://vow.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://szh.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://thn.quarkkingdee.top

Ruby: s.count("a")
来源：http://zxi.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://knk.gaohongyu789.top

[E13] 逐字符遍历
来源：http://oxj.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://qqx.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://meo.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nsa.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jky.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fik.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nyp.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mfr.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgk.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://gqt.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pud.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://wxn.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zur.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qbv.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qhs.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fue.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gsm.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dqq.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://trc.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hzd.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pei.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lkd.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://veg.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kcf.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ost.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://omc.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ito.jqgufenzy.top

[E16] 数字千分位
来源：http://cmz.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://itg.smart0.xyz

PHP:  number_format(1234567);
来源：http://jmc.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://ucj.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gqt.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://woo.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uxa.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhv.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://ywj.xuetiantiany.cn

[E17] 首字母大写
来源：http://ehs.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bqt.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zqy.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mpv.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://myu.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gqq.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uix.tanke756.top

Ruby: s.capitalize
来源：http://wdf.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wcu.guowangkeji.top

[E18] 模板占位符替换
来源：http://ylc.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrc.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yew.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pio.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://egc.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ucj.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xhc.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://geh.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zqb.cucudq.cn

[E19] 多行文本按行拆分
来源：http://hhp.fktsv.cn

Py:   s.splitlines()
来源：http://uap.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hlm.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://oni.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://znv.ybcxt.top

Java: s.lines().toList()
来源：http://jxm.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://upm.jinghuilouyu.cn

Ruby: s.lines
来源：http://sve.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://nab.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://wlr.andypj.xyz

Py:   if not s:
来源：http://tdh.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ctb.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hvi.gogol.net.cn

TS:   if (s === "") {}
来源：http://rfv.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://fcz.jqgfzy.top

Go:   if s == "" {}
来源：http://gxu.hfpthk.cn

Ruby: if s.empty?
来源：http://myy.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wjq.yonumen.top

[E21] 超长截断加省略号
来源：http://lop.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dye.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gfo.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxf.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qty.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ihg.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://tad.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://keo.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ktb.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://obc.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yhg.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mic.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfr.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aca.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yxj.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cbk.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://utu.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vno.feifeiyinyue.top

================================================================================
来源：http://hjv.chenjidiqi.icu

F. 文件与目录
来源：http://qxb.yangfankeji.com

================================================================================
来源：http://prr.guannengcc.top

[F01] 读取整个文件
来源：http://rit.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uey.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://zfy.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://osm.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dpg.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hui.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xmo.guannengcc.top

Ruby: File.read("a.txt")
来源：http://dka.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://lhx.gzhubu.top

[F02] 逐行读取文件
来源：http://ymf.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fmh.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iyf.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oiv.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lvj.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqk.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xyb.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zvx.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mhy.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://nxj.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hhk.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qws.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://del.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pnq.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kvj.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://omj.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://ckn.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yaq.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://jns.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ggq.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kai.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tah.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://doz.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wqz.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://prh.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://voe.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tgm.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://uyi.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hdz.yj20258.top

PHP:  file_exists("a.txt");
来源：http://pwx.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://rhc.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://awz.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://unq.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aiw.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://cvp.tarul.cn

C#:   File.Exists("a.txt")
来源：http://shr.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://onj.yj202588.top

Py:   os.remove("a.txt")
来源：http://ngf.fengsongda.top

PHP:  unlink("a.txt");
来源：http://vti.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jlq.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://oxl.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsu.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://pnm.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://avk.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://qdp.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://dpw.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxi.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ihi.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://api.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvu.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlf.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://odg.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ort.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://maw.zdbjq.cn

[F08] 遍历目录
来源：http://rng.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wok.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lvn.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://tmh.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://xwc.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kzo.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dvx.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://tnu.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://oup.ctjpmb.com

[F09] 获取文件大小
来源：http://qwi.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://nuw.xinyue.icu

PHP:  filesize("a.txt");
来源：http://dog.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://cuz.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://tre.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zyi.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://scg.ydzc1.top

Ruby: File.size("a.txt")
来源：http://bbb.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://fvd.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://bus.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfa.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://amt.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajz.birdmap.top

TS:   path.extname("a.txt")
来源：http://sqr.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aef.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hwd.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dbe.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uvg.quarkkingdee.top

[F11] 复制与移动文件
来源：http://pmv.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mwt.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://avy.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdu.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ely.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oia.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bhz.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iok.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oqp.pycfn.com

[F12] CSV 读写
来源：http://deo.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gnp.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cjc.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://heg.yanxiufei.cn

TS:   // 同上
来源：http://kvj.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://teu.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jya.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cxk.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qpk.hysaishi.cn

================================================================================
来源：http://agg.zhijiandao.cn

G. 面向对象
来源：http://nvn.vqdsnc.cn

================================================================================
来源：http://ryx.yuxming.cn

[G01] 定义类
来源：http://eta.bbcook.cn

Py:   class User: pass
来源：http://xnp.pengpengdd.cyou

PHP:  class User {}
来源：http://wdy.ivvv.top

JS:   class User {}
来源：http://muj.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://kyj.jinyuanbaomall.cn

Java: class User {}
来源：http://qry.guannengcc.top

Go:   type User struct { Name string }
来源：http://lyt.xuanzx.com

Ruby: class User; end
来源：http://kwb.yj202588.top

C#:   class User {}
来源：http://cwz.aibaodan.cn

[G02] 构造函数
来源：http://rkp.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://opf.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://nlk.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://rzj.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://pap.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://olo.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rtq.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://iaz.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://dso.kuanghao11.cn

[G03] 实例属性
来源：http://wfa.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://btt.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://vnc.fzhhl.top

JS:   this.name = "x";
来源：http://fex.yongpay.top

TS:   name: string = "x";
来源：http://vac.cucudq.cn

Java: private String name;
来源：http://vrp.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ufv.vehdjk.com

Ruby: @name = "x"
来源：http://zul.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://khu.wangshuangyany.cn

[G04] 定义方法
来源：http://cnf.yj20258888.top

Py:   def greet(self): return self.name
来源：http://sbn.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://ggv.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://zqd.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://ere.chenzaomai.com

Java: String greet() { return name; }
来源：http://exf.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qju.wangdashe.top

Ruby: def greet; @name; end
来源：http://jgu.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://jhx.fzhhl.top

[G05] 继承
来源：http://ukt.9152youxi.cn

Py:   class Admin(User): pass
来源：http://ihr.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://tlq.316326.xyz

JS:   class Admin extends User {}
来源：http://jvk.ctjpmb.com

TS:   class Admin extends User {}
来源：http://voq.fktsv.cn

Java: class Admin extends User {}
来源：http://qqk.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gjd.ctjpmb.com

Ruby: class Admin < User; end
来源：http://vow.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://cae.jlsjyb.cn

[G06] 重写方法
来源：http://npf.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://jjr.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yjp.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://xlr.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://jam.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://mmj.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xbe.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://fid.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://ggi.zdbjq.cn

[G07] 调用父类方法
来源：http://xmd.fehbvm.com

Py:   super().greet()
来源：http://zrr.hysaishi.cn

PHP:  parent::greet();
来源：http://ylt.xuanzx.com

JS:   super.greet();
来源：http://gio.hcnkem.com

TS:   super.greet();
来源：http://iop.xziqi.cn

Java: super.greet();
来源：http://bpd.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ont.ehwqpu.com

Ruby: super
来源：http://nby.ydzc1.top

C#:   base.Greet();
来源：http://byc.tarul.cn

[G08] 静态方法与属性
来源：http://dcs.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ohr.fengsongda.top

PHP:  public static function f() {}
来源：http://jaj.hnqzz.top

JS:   static f() {}
来源：http://doa.nwbrower.top

TS:   static f(): void {}
来源：http://sfj.fehbvm.com

Java: static void f() {}
来源：http://xsd.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vlp.zhixingplan.top

Ruby: def self.f; end
来源：http://rke.ppjwa.cn

C#:   public static void F() {}
来源：http://spa.birdmap.top

[G09] 接口 / 抽象类
来源：http://pkn.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://zco.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://hcu.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dgu.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://ftm.meibo888.top

Java: interface Shape { double area(); }
来源：http://sko.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://mep.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://drt.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://zxt.fanxiaobao.xyz


<!-- 参考信息 -->