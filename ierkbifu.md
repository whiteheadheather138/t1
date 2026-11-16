代发 wailian999

JS:   [...s].reverse().join("")
来源：http://yci.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://kyy.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ooh.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://unt.hnxiangtu.top

Ruby: s.reverse
来源：http://sjl.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://qer.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://qze.chenlongwang.top

Py:   s.count("a")
来源：http://fsu.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://ovw.52xcode.cn

JS:   s.split("a").length - 1
来源：http://wki.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://bfs.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wox.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://oqq.kuanghao11.cn

Ruby: s.count("a")
来源：http://hth.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://zgx.c1oappe.top

[E13] 逐字符遍历
来源：http://jwq.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://qcs.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dyf.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://gkt.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://snv.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yxz.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bbg.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iir.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xxk.xuanzx.com

[E14] URL 编码与 Base64
来源：http://foh.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsr.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmo.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kyq.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bcm.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://djs.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yma.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uaq.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wbh.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://vky.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://aco.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ryq.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fet.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xve.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fry.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tsc.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aqm.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wsd.vehdjk.com

[E16] 数字千分位
来源：http://sur.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://pid.bbcook.cn

PHP:  number_format(1234567);
来源：http://rlg.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bre.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dwy.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tvj.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hpe.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://psm.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://yfv.cucudq.cn

[E17] 首字母大写
来源：http://guv.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jwh.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://glj.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otf.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jmt.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aug.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://snt.epnwcf.com

Ruby: s.capitalize
来源：http://tmh.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ywk.xuanzx.com

[E18] 模板占位符替换
来源：http://rlw.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jsl.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jmp.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kcx.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://rpk.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xkx.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dmq.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qpj.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cty.fzhhl.top

[E19] 多行文本按行拆分
来源：http://zil.ydzc1.top

Py:   s.splitlines()
来源：http://sdp.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gga.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://nlu.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://vwh.c1oappe.top

Java: s.lines().toList()
来源：http://wfv.sweek.top

Go:   strings.Split(s, "\n")
来源：http://yel.gzhubu.top

Ruby: s.lines
来源：http://vwe.316326.xyz

C#:   s.Split('\n')
来源：http://shv.xylfe.cn

[E20] 判断字符串是否为空
来源：http://nnc.jqgfzy.top

Py:   if not s:
来源：http://eiz.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ouo.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kiw.ehwqpu.com

TS:   if (s === "") {}
来源：http://nov.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://kro.yj20258888.top

Go:   if s == "" {}
来源：http://btm.wangdashe.top

Ruby: if s.empty?
来源：http://mta.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cap.c1oappe.top

[E21] 超长截断加省略号
来源：http://ziy.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://soi.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xvq.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://auu.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://djh.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rjf.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://ymx.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hnj.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vss.xziqi.cn

[E22] 字节长度与字符长度
来源：http://uep.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nlf.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ffy.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uye.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tto.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://icy.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rns.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://oed.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vrc.fzhhl.top

================================================================================
来源：http://sri.hammf.cn

F. 文件与目录
来源：http://twr.wangdashe.top

================================================================================
来源：http://onm.bbcook.cn

[F01] 读取整个文件
来源：http://pdj.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fmb.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://ioe.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pjq.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ffw.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hts.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qyg.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://fxj.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://rcq.ydjk.org.cn

[F02] 逐行读取文件
来源：http://kkz.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xhg.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ctm.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwk.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ztm.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xnb.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bhh.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gvf.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qpc.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://lbp.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pid.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uzv.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzv.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zgx.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gtn.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wro.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://ebn.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kas.svipenyu.cn

[F04] 追加写入文件
来源：http://tso.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipc.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zkd.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bcd.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjn.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ywx.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://avd.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xeh.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pae.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://wom.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jvp.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://mwb.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://rma.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://qox.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ojo.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ydo.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://zez.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://adg.sjlbkw.cn

[F06] 删除文件
来源：http://lhf.xziqi.cn

Py:   os.remove("a.txt")
来源：http://aeh.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://jid.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iko.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tbw.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xgg.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://vjh.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://orw.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://zdb.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://lea.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kfl.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ucw.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rtj.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wad.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ddc.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pxz.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://srp.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nky.yueranfly.top

[F08] 遍历目录
来源：http://qxe.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcj.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lha.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://vnn.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://szg.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lkv.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fcu.aizwys.cn

Ruby: Dir.children("dir")
来源：http://rry.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://xqs.yueranfly.top

[F09] 获取文件大小
来源：http://pes.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://qlq.tian-w.cn

PHP:  filesize("a.txt");
来源：http://nir.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://gyq.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://orb.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://alz.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bua.shuidangran.top

Ruby: File.size("a.txt")
来源：http://whs.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://fcf.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ecm.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jlk.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oot.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eus.tanke756.top

TS:   path.extname("a.txt")
来源：http://tms.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kuu.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzp.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpc.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsd.zdqjudy.top

[F11] 复制与移动文件
来源：http://myi.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jna.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mht.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahl.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rot.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dfz.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fjy.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hod.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ubk.snrcjt.cn

[F12] CSV 读写
来源：http://jef.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ehp.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://szr.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zss.jinyuanbaomall.cn

TS:   // 同上
来源：http://awp.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://upj.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wwd.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qca.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lga.fanxiaobao.xyz

================================================================================
来源：http://axy.zhixingplan.top

G. 面向对象
来源：http://rtg.zhengqikj.top

================================================================================
来源：http://igi.iojbl.cn

[G01] 定义类
来源：http://bdr.ydzc1.top

Py:   class User: pass
来源：http://zhn.shangyingyoupin.top

PHP:  class User {}
来源：http://qxz.gaohongyu789.top

JS:   class User {}
来源：http://uxh.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://gwq.9152youxi.cn

Java: class User {}
来源：http://rhc.epnwcf.com

Go:   type User struct { Name string }
来源：http://tcu.zycfv.cn

Ruby: class User; end
来源：http://yyp.jqgfzy.top

C#:   class User {}
来源：http://qsl.tianlin.xyz

[G02] 构造函数
来源：http://gyl.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://zxj.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://jak.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://hde.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://wlp.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://lpr.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nwm.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://dmr.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://qzv.quarkkingdee.top

[G03] 实例属性
来源：http://php.tianlin.xyz

Py:   self.name = "x"
来源：http://itg.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://rpc.guowangkeji.top

JS:   this.name = "x";
来源：http://tyw.aizwys.cn

TS:   name: string = "x";
来源：http://jub.havefunace.top

Java: private String name;
来源：http://roi.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://upl.sxryk.cn

Ruby: @name = "x"
来源：http://hrv.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://pvf.yuanzhike.top

[G04] 定义方法
来源：http://eho.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://ook.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://prc.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://ycx.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://icd.jinqigufen.top

Java: String greet() { return name; }
来源：http://eoh.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zwu.andypj.xyz

Ruby: def greet; @name; end
来源：http://nww.gzhubu.top

C#:   public string Greet() => Name;
来源：http://ndg.xylfe.cn

[G05] 继承
来源：http://ngl.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://qpc.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://neu.nanxinkj.top

JS:   class Admin extends User {}
来源：http://eol.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://ynz.sxryk.cn

Java: class Admin extends User {}
来源：http://rtc.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vxd.gogol.net.cn

Ruby: class Admin < User; end
来源：http://ezo.hnxiangtu.top

C#:   class Admin : User {}
来源：http://vtc.zhaomingkeji.xyz

[G06] 重写方法
来源：http://xju.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://dki.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://phv.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://lxz.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://zui.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://sry.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xmw.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://igj.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://ihd.hcnkem.com

[G07] 调用父类方法
来源：http://csw.ivvv.top

Py:   super().greet()
来源：http://dux.chenzaomai.com

PHP:  parent::greet();
来源：http://vng.jinqigufen.top

JS:   super.greet();
来源：http://zxo.hnxiangtu.top

TS:   super.greet();
来源：http://yqc.sweek.top

Java: super.greet();
来源：http://psy.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mru.ppjwa.cn

Ruby: super
来源：http://qgp.ehwqpu.com

C#:   base.Greet();
来源：http://sfs.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://nrt.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mzv.nanxinkj.top

PHP:  public static function f() {}
来源：http://beu.hnxiangtu.top

JS:   static f() {}
来源：http://cdr.sufxvd.cn

TS:   static f(): void {}
来源：http://ojo.pycfn.com

Java: static void f() {}
来源：http://avr.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bfy.xinyue.icu

Ruby: def self.f; end
来源：http://lwz.ehwqpu.com

C#:   public static void F() {}
来源：http://nuf.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://tef.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://jrj.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wmg.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vgc.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://lok.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://mva.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://fmk.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nqj.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://jib.hfpthk.cn


<!-- 参考信息 -->