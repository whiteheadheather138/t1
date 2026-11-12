代发 wailian999

Ruby: s.reverse
来源：http://yjv.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://cky.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://sgf.birdmap.top

Py:   s.count("a")
来源：http://ugi.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://pyl.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://auw.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://ukt.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rgs.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://lyt.ppjwa.cn

Ruby: s.count("a")
来源：http://jfi.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://ylc.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://cfs.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://soi.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://exn.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zob.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qns.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eld.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ajq.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://snx.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://htx.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://tqv.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wzj.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://yqj.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qqv.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://imq.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jjv.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cpn.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://znq.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mju.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://kgq.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qqu.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tiu.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kjx.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vkk.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jtn.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hwl.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://myw.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hca.yanxiufei.cn

[E16] 数字千分位
来源：http://nlx.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://eqc.cqqwz.cn

PHP:  number_format(1234567);
来源：http://dbg.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://prs.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ijc.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://smn.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oso.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gze.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://cmv.9152youxi.cn

[E17] 首字母大写
来源：http://ggu.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rga.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zkz.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nts.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aoy.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rle.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blf.daria6918.cn

Ruby: s.capitalize
来源：http://rgq.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kuu.yongpay.top

[E18] 模板占位符替换
来源：http://rdq.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mjx.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfe.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ljv.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dtr.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://czq.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kjg.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://myu.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bow.aizwys.cn

[E19] 多行文本按行拆分
来源：http://vcq.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://jgc.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cov.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://fnz.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://tfh.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://ffa.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://tux.nwbrower.top

Ruby: s.lines
来源：http://elk.jqgufenzy.top

C#:   s.Split('\n')
来源：http://nek.yueranfly.top

[E20] 判断字符串是否为空
来源：http://sqe.yuanzhike.top

Py:   if not s:
来源：http://bbz.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hmo.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hal.zdbjq.cn

TS:   if (s === "") {}
来源：http://wiw.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://uzq.jlsjyb.cn

Go:   if s == "" {}
来源：http://fio.tanke756.top

Ruby: if s.empty?
来源：http://rkc.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://upq.dianchejie.cn

[E21] 超长截断加省略号
来源：http://bgr.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gbt.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nom.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wux.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://icv.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hax.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://yrq.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbf.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://igo.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://fax.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://duy.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgw.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ivm.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qny.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zzd.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gok.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://okh.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dyu.nanxinkj.top

================================================================================
来源：http://frs.ivvv.top

F. 文件与目录
来源：http://hch.shanyushiyangkeji.top

================================================================================
来源：http://fjt.pengpengdd.cyou

[F01] 读取整个文件
来源：http://bew.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eds.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://ztu.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wio.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eed.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://esy.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ugg.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://heg.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://dvc.zdbjq.cn

[F02] 逐行读取文件
来源：http://kuh.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fqr.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vkv.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vkr.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gfr.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zug.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://otj.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cuy.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fgu.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://qbd.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pqq.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gub.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sap.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tfz.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msv.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lvv.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://fmp.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://icc.yuanzhike.top

[F04] 追加写入文件
来源：http://mzy.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qju.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eap.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lgh.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vvy.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dud.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pqb.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jiw.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cet.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://cti.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gcc.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://yzv.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://xav.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://qts.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kuf.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhb.sweek.top

Ruby: File.exist?("a.txt")
来源：http://nbk.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://avr.c1oappe.top

[F06] 删除文件
来源：http://qio.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://jks.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://nva.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://qdz.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://rwx.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tmd.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://jyt.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://gbn.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://xpx.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://wlr.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nwo.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bdg.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bpi.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mqw.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zdy.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rym.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://trr.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uke.yanxiufei.cn

[F08] 遍历目录
来源：http://pec.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dcj.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lnx.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://ego.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://kjw.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://inz.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://plq.andypj.xyz

Ruby: Dir.children("dir")
来源：http://rfs.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://scm.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://zsa.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://gef.meibo888.top

PHP:  filesize("a.txt");
来源：http://kbm.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://iiu.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://ols.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://mnc.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fyg.zycfv.cn

Ruby: File.size("a.txt")
来源：http://bvy.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ofm.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://srt.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ddk.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fwq.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xgv.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://wuv.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rqe.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ieq.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://att.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://loq.c1oappe.top

[F11] 复制与移动文件
来源：http://jjn.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zul.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fig.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gdl.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gji.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jdt.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ptk.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gri.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ugb.ivvv.top

[F12] CSV 读写
来源：http://nms.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://foo.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wxf.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://inu.chenjidiqi.icu

TS:   // 同上
来源：http://gfd.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dql.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ypc.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lrt.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eik.zhaomingkeji.xyz

================================================================================
来源：http://vij.zhaomingkeji.xyz

G. 面向对象
来源：http://sqt.zdbjq.cn

================================================================================
来源：http://eyr.shuidangran.top

[G01] 定义类
来源：http://ajf.yfazqb.com

Py:   class User: pass
来源：http://qdk.fehbvm.com

PHP:  class User {}
来源：http://lti.yvedp.cn

JS:   class User {}
来源：http://ljf.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://fgg.shuidangran.top

Java: class User {}
来源：http://ywr.sufxvd.cn

Go:   type User struct { Name string }
来源：http://jrt.xinyue.icu

Ruby: class User; end
来源：http://oqm.0kj1m.cn

C#:   class User {}
来源：http://fki.yangfankeji.com

[G02] 构造函数
来源：http://etp.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://qpw.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ufi.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://ybu.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://rny.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://chz.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wzt.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://ggb.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://pts.dianchejie.cn

[G03] 实例属性
来源：http://nkb.nanxinkj.top

Py:   self.name = "x"
来源：http://bcf.bjfxy.top

PHP:  public string $name = "x";
来源：http://tuk.quarkkingdee.top

JS:   this.name = "x";
来源：http://ivv.hongshengwenyu.top

TS:   name: string = "x";
来源：http://qnl.hongshengwenyu.top

Java: private String name;
来源：http://ygq.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wsw.kuanghao11.cn

Ruby: @name = "x"
来源：http://bly.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://scl.cdnleiting.top

[G04] 定义方法
来源：http://byw.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://fus.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://liy.redwolf501.top

JS:   greet() { return this.name; }
来源：http://vlz.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://jvc.cashguo.top

Java: String greet() { return name; }
来源：http://adh.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dow.tianlin.xyz

Ruby: def greet; @name; end
来源：http://dli.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://eum.chenjidiqi.icu

[G05] 继承
来源：http://qzs.nanxinkj.top

Py:   class Admin(User): pass
来源：http://upa.mhx1999.top

PHP:  class Admin extends User {}
来源：http://fql.zycfv.cn

JS:   class Admin extends User {}
来源：http://dgl.fehbvm.com

TS:   class Admin extends User {}
来源：http://kgg.tian-w.cn

Java: class Admin extends User {}
来源：http://vuk.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kej.yangfankeji.com

Ruby: class Admin < User; end
来源：http://gyq.tianlin.xyz

C#:   class Admin : User {}
来源：http://akx.kuanghao11.cn

[G06] 重写方法
来源：http://pmv.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://xdt.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pqw.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://pbi.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://ytg.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://yzv.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jry.ivvv.top

Ruby: def greet; "admin"; end
来源：http://bhf.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://tmw.yuanzhike.top

[G07] 调用父类方法
来源：http://nrp.hfpthk.cn

Py:   super().greet()
来源：http://rkd.zhengqikj.top

PHP:  parent::greet();
来源：http://lhp.dashuyun.cn

JS:   super.greet();
来源：http://qhz.yueranfly.top

TS:   super.greet();
来源：http://rrc.jlsjyb.cn

Java: super.greet();
来源：http://zut.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rtd.havefunace.top

Ruby: super
来源：http://swd.kuanghao11.cn

C#:   base.Greet();
来源：http://wcc.daxiang520.top

[G08] 静态方法与属性
来源：http://yuw.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwd.andypj.xyz

PHP:  public static function f() {}
来源：http://ifw.ppjwa.cn

JS:   static f() {}
来源：http://hfl.quarkkingdee.top

TS:   static f(): void {}
来源：http://wok.hywenlv.cn

Java: static void f() {}
来源：http://ayd.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cjt.hcnkem.com

Ruby: def self.f; end
来源：http://jrt.cdnleiting.top

C#:   public static void F() {}
来源：http://qdj.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://geg.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://pkv.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pto.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbv.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://plg.cucudq.cn

Java: interface Shape { double area(); }
来源：http://krx.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://fqv.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iug.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://zdl.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://amu.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://jpy.epnwcf.com

PHP:  public / protected / private
来源：http://nsw.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://ptu.guowangkeji.top


<!-- 参考信息 -->