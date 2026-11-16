代发 wailian999

JS:   [...s].reverse().join("")
来源：http://jwg.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://qwp.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jhj.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mgs.nwbrower.top

Ruby: s.reverse
来源：http://hoz.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://tig.birdmap.top

[E12] 统计某字符出现次数
来源：http://ugk.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://mko.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://pbt.birdmap.top

JS:   s.split("a").length - 1
来源：http://hmj.tian-w.cn

TS:   s.split("a").length - 1
来源：http://sak.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://taf.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://bwy.fehbvm.com

Ruby: s.count("a")
来源：http://bil.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://ogt.yvedp.cn

[E13] 逐字符遍历
来源：http://hmy.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://nmp.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgs.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://umy.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vww.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://njn.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xxh.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tmn.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hvq.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://wdd.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ems.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vgw.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpu.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tpm.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gqg.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yzt.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uto.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xlq.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://ixl.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rje.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rni.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oga.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qzl.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mvr.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rnz.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nij.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xgl.fzhhl.top

[E16] 数字千分位
来源：http://bjd.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://dwn.andypj.xyz

PHP:  number_format(1234567);
来源：http://clo.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uob.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vfu.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vlo.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mim.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wjb.uphjek.com

C#:   1234567.ToString("N0")
来源：http://txz.hesvh.cn

[E17] 首字母大写
来源：http://ajg.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kbq.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ylc.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fof.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://twq.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jga.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jjr.hnxiangtu.top

Ruby: s.capitalize
来源：http://gja.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pkg.dashuyun.cn

[E18] 模板占位符替换
来源：http://klu.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rsw.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://itz.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mib.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fgf.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bps.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dov.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://azo.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xmw.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://stm.xinyue.icu

Py:   s.splitlines()
来源：http://ymx.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ggo.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://hvl.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://jbf.svipenyu.cn

Java: s.lines().toList()
来源：http://ahi.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://vko.zhaomingkeji.xyz

Ruby: s.lines
来源：http://deg.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://hbh.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://dmv.chenlongwang.top

Py:   if not s:
来源：http://gew.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wvc.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yhz.hysaishi.cn

TS:   if (s === "") {}
来源：http://esl.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://cqg.wangshuangyany.cn

Go:   if s == "" {}
来源：http://rxk.pengpengdd.cyou

Ruby: if s.empty?
来源：http://tld.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nlb.cheryme.top

[E21] 超长截断加省略号
来源：http://wgv.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epi.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wyq.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijw.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xpq.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://okt.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xqx.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axe.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jkd.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://xdt.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yix.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tao.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lqz.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vjl.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://azo.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kgg.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://xhd.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://krn.shangyingyoupin.top

================================================================================
来源：http://vsl.hnxiangtu.top

F. 文件与目录
来源：http://hsj.ehwqpu.com

================================================================================
来源：http://gjb.9152youxi.cn

[F01] 读取整个文件
来源：http://chn.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lzi.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://bck.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zdh.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zgq.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cev.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://svn.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://yqj.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://eug.ivvv.top

[F02] 逐行读取文件
来源：http://nzi.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xpg.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wrr.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oot.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sdh.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hva.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eef.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocg.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rco.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://uhg.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xhr.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://cnj.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zjt.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fft.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ktf.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mgu.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://uxo.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bse.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://rwt.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rxw.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://loj.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gla.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lvw.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tvi.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qbe.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zta.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pkg.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://fkw.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zss.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://oqi.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://bhe.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://yug.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wmw.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mzq.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://shr.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://cxy.yfazqb.com

[F06] 删除文件
来源：http://jtu.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://lav.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://nja.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://iya.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dvo.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://euk.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://omo.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://xwf.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://bzj.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://ohx.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nnf.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wgd.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pze.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnk.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://arp.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mls.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocp.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://upw.jlsjyb.cn

[F08] 遍历目录
来源：http://gfr.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tmn.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://krv.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://vuj.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://znb.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://man.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://byx.shuidangran.top

Ruby: Dir.children("dir")
来源：http://ggl.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://snd.hammf.cn

[F09] 获取文件大小
来源：http://rgx.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://bxl.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://udx.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://azo.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://rou.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://xhm.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qqm.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://mai.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://eiu.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://neb.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xzd.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fur.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kqu.daria6918.cn

TS:   path.extname("a.txt")
来源：http://abd.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sne.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ixm.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qzf.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dwe.yj20258.top

[F11] 复制与移动文件
来源：http://ivb.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://atb.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ezw.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcd.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ajd.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xwd.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fyb.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dwk.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://unh.jyoumei.cn

[F12] CSV 读写
来源：http://xsb.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jvv.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://goz.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mnj.pycfn.com

TS:   // 同上
来源：http://fay.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://woi.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bgf.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uor.dashuyun.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ktn.sysykeji.top

================================================================================
来源：http://tik.yj20258888.top

G. 面向对象
来源：http://ezn.zhixingplan.top

================================================================================
来源：http://gjm.daxiang520.top

[G01] 定义类
来源：http://ugn.cucudq.cn

Py:   class User: pass
来源：http://afj.tianlin.xyz

PHP:  class User {}
来源：http://ixc.xuanzx.com

JS:   class User {}
来源：http://tpt.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://llg.sufxvd.cn

Java: class User {}
来源：http://rjv.gogol.net.cn

Go:   type User struct { Name string }
来源：http://prk.yj20258888.top

Ruby: class User; end
来源：http://qrx.zhoulong.xyz

C#:   class User {}
来源：http://dau.wangdashe.top

[G02] 构造函数
来源：http://fmn.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://wys.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://gue.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://ggc.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://vnk.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://gsb.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dwg.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://iuk.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://iie.jianghu66.top

[G03] 实例属性
来源：http://vrv.chenzaomai.com

Py:   self.name = "x"
来源：http://ejh.svipenyu.cn

PHP:  public string $name = "x";
来源：http://jbl.sxryk.cn

JS:   this.name = "x";
来源：http://fkm.quarkkingdee.top

TS:   name: string = "x";
来源：http://jiz.yvedp.cn

Java: private String name;
来源：http://xpa.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uhh.tanke756.top

Ruby: @name = "x"
来源：http://std.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://tsj.yj20258888.top

[G04] 定义方法
来源：http://unp.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://yrl.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://qzr.sxryk.cn

JS:   greet() { return this.name; }
来源：http://qus.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://hsi.jqgufenzy.top

Java: String greet() { return name; }
来源：http://fag.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ivo.jqgfzy.top

Ruby: def greet; @name; end
来源：http://clo.jianghu66.top

C#:   public string Greet() => Name;
来源：http://mhl.hnxiangtu.top

[G05] 继承
来源：http://cle.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://exs.jianghu66.top

PHP:  class Admin extends User {}
来源：http://sio.jqgfzy.top

JS:   class Admin extends User {}
来源：http://wue.redwolf501.top

TS:   class Admin extends User {}
来源：http://exk.pycfn.com

Java: class Admin extends User {}
来源：http://qmo.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xwj.nanxinkj.top

Ruby: class Admin < User; end
来源：http://dnq.xuanzx.com

C#:   class Admin : User {}
来源：http://dge.xinyue.icu

[G06] 重写方法
来源：http://tbs.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://jeu.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lku.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://cid.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://cxq.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://xmi.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://irv.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://pkc.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://jgp.ctjpmb.com

[G07] 调用父类方法
来源：http://smq.shanyushiyangkeji.top

Py:   super().greet()
来源：http://end.hcnkem.com

PHP:  parent::greet();
来源：http://qdw.jinqigufen.top

JS:   super.greet();
来源：http://vgm.zycfv.cn

TS:   super.greet();
来源：http://bkk.gotoacloud.top

Java: super.greet();
来源：http://ruo.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cis.tarul.cn

Ruby: super
来源：http://bub.dashuyun.cn

C#:   base.Greet();
来源：http://cbs.uphjek.com

[G08] 静态方法与属性
来源：http://xsf.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bpy.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://goe.sweek.top

JS:   static f() {}
来源：http://gdh.wangdashe.top

TS:   static f(): void {}
来源：http://ibe.tian-w.cn

Java: static void f() {}
来源：http://cyu.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xrs.cqqwz.cn

Ruby: def self.f; end
来源：http://hrd.tarul.cn

C#:   public static void F() {}
来源：http://jms.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://sqq.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://xzu.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://ftp.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pll.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://drt.gzhubu.top

Java: interface Shape { double area(); }
来源：http://fix.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://fdh.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qar.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://ilc.hfpthk.cn


<!-- 参考信息 -->