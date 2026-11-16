代发 wailian999

JS:   [...s].reverse().join("")
来源：http://qqe.tanke756.top

TS:   [...s].reverse().join("")
来源：http://cer.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xau.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://onu.cqqwz.cn

Ruby: s.reverse
来源：http://hho.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://ged.cashguo.top

[E12] 统计某字符出现次数
来源：http://mpl.sxryk.cn

Py:   s.count("a")
来源：http://tvv.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://vjj.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://rug.birdmap.top

TS:   s.split("a").length - 1
来源：http://dfz.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lbe.yj20258.top

Go:   strings.Count(s, "a")
来源：http://azj.yongpay.top

Ruby: s.count("a")
来源：http://njs.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://rjr.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://wem.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://opp.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://clf.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://apv.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftx.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://old.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cii.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iva.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://imn.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://tyx.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mmy.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qei.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uql.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://loc.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bof.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsn.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ldj.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kqi.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://osz.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xul.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wxr.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rkh.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://ppn.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfu.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cqt.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zoo.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dcz.aibaodan.cn

[E16] 数字千分位
来源：http://yjl.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://ovn.cqqwz.cn

PHP:  number_format(1234567);
来源：http://oug.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mpo.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kah.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lpf.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mgj.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zjx.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://xdw.xziqi.cn

[E17] 首字母大写
来源：http://nwi.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pow.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bjv.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gcf.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ssw.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zrh.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tvb.yueranfly.top

Ruby: s.capitalize
来源：http://hqn.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vyo.daria6918.cn

[E18] 模板占位符替换
来源：http://yrj.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://agy.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vyb.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qsa.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://thu.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vem.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lfb.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://njq.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wht.tanke756.top

[E19] 多行文本按行拆分
来源：http://jet.quarkkingdee.top

Py:   s.splitlines()
来源：http://ukz.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bly.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://mui.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://czx.sysykeji.top

Java: s.lines().toList()
来源：http://qka.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://dgx.wangshuangyany.cn

Ruby: s.lines
来源：http://opm.hnxiangtu.top

C#:   s.Split('\n')
来源：http://qdx.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://run.yfazqb.com

Py:   if not s:
来源：http://wfj.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qxp.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://agg.xinyue.icu

TS:   if (s === "") {}
来源：http://fwc.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://adc.sysykeji.top

Go:   if s == "" {}
来源：http://jlk.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://hbr.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://azi.smart0.xyz

[E21] 超长截断加省略号
来源：http://hzc.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dif.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dxw.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://krl.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtp.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqr.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://oor.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hym.fktsv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yij.bbcook.cn

[E22] 字节长度与字符长度
来源：http://nxs.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wzk.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mll.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kwr.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xad.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pvo.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fvk.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://ixa.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ebs.shzxlz.cn

================================================================================
来源：http://wid.zhiwuduotai.top

F. 文件与目录
来源：http://alz.zhiwuduotai.top

================================================================================
来源：http://jui.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://zbo.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzk.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://imi.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zac.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ymm.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lsq.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uor.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://yok.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://dtf.bbcook.cn

[F02] 逐行读取文件
来源：http://yzw.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://stw.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jco.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sos.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubg.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://afe.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://puo.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hew.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lou.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://wxt.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://epq.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bps.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjq.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://orr.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aun.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxx.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://nlk.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gau.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://lbg.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tex.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wkx.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulw.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ahb.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://smp.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cez.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aft.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ayl.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://dtb.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://flx.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://voc.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://pif.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://lhz.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ygc.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zll.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://wnc.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://fve.tarul.cn

[F06] 删除文件
来源：http://rbo.yvedp.cn

Py:   os.remove("a.txt")
来源：http://fkm.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://oay.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://ieg.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fjn.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hzy.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://pay.yj202588.top

Ruby: File.delete("a.txt")
来源：http://hoy.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://mpx.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://vls.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zaa.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://osf.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://asa.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzp.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wxd.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://whb.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fyf.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://agw.nwbrower.top

[F08] 遍历目录
来源：http://bmy.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zcv.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pkl.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://pcf.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://jod.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xdk.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uca.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://gtp.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://flq.tarul.cn

[F09] 获取文件大小
来源：http://zpb.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://crw.tian-w.cn

PHP:  filesize("a.txt");
来源：http://eqi.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://pjy.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://vgg.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://wyp.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vhn.tian-w.cn

Ruby: File.size("a.txt")
来源：http://jcp.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://avt.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://ymc.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ujb.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yix.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wtf.yj20258888.top

TS:   path.extname("a.txt")
来源：http://uul.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://chy.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wel.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://knm.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tln.gaohongyu789.top

[F11] 复制与移动文件
来源：http://efl.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvr.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lzi.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://emw.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wkj.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qae.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ggt.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ylh.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aoj.yanxiufei.cn

[F12] CSV 读写
来源：http://pik.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mej.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wgo.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nbg.chenlongwang.top

TS:   // 同上
来源：http://jzh.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mco.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://boq.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jaz.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kjk.bbcook.cn

================================================================================
来源：http://dvz.havefunace.top

G. 面向对象
来源：http://hbp.ehwqpu.com

================================================================================
来源：http://nwc.epnwcf.com

[G01] 定义类
来源：http://qnq.9152youxi.cn

Py:   class User: pass
来源：http://jhp.yj202588.top

PHP:  class User {}
来源：http://irf.zhiwuduotai.top

JS:   class User {}
来源：http://rao.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://aml.pengpengdd.cyou

Java: class User {}
来源：http://hdw.meibo888.top

Go:   type User struct { Name string }
来源：http://bxf.cheryme.top

Ruby: class User; end
来源：http://oti.gogol.net.cn

C#:   class User {}
来源：http://iah.guannengcc.top

[G02] 构造函数
来源：http://mrw.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://uov.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://fbf.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://vjb.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://bcv.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://whg.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qjj.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://vmf.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://shw.zdbjq.cn

[G03] 实例属性
来源：http://nxj.nanxuanxn.top

Py:   self.name = "x"
来源：http://bfm.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://rvs.zhijiandao.cn

JS:   this.name = "x";
来源：http://kqa.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://ahf.jyoumei.cn

Java: private String name;
来源：http://lft.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xdd.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://vct.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://kpr.fanxiaobao.xyz

[G04] 定义方法
来源：http://sga.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://wtb.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://kqn.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://cjb.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://zld.gaohongyu789.top

Java: String greet() { return name; }
来源：http://mun.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://naq.yuxming.cn

Ruby: def greet; @name; end
来源：http://hut.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://unj.ydjk.org.cn

[G05] 继承
来源：http://qin.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://ege.birdmap.top

PHP:  class Admin extends User {}
来源：http://ign.yuanzhike.top

JS:   class Admin extends User {}
来源：http://yuz.vehdjk.com

TS:   class Admin extends User {}
来源：http://rhi.shuidangran.top

Java: class Admin extends User {}
来源：http://eic.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://asm.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://dho.hywenlv.cn

C#:   class Admin : User {}
来源：http://djg.sjlbkw.cn

[G06] 重写方法
来源：http://mou.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://dgu.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rjl.havefunace.top

JS:   greet() { return "admin"; }
来源：http://plp.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://nft.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://fle.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cpd.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://xrl.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://wyf.jiagoushi.top

[G07] 调用父类方法
来源：http://erk.chenjidiqi.icu

Py:   super().greet()
来源：http://iyc.yanxiufei.cn

PHP:  parent::greet();
来源：http://mrd.bbcook.cn

JS:   super.greet();
来源：http://fyt.zhaomingkeji.xyz

TS:   super.greet();
来源：http://dbp.jqgfzy.top

Java: super.greet();
来源：http://snh.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddv.redwolf501.top

Ruby: super
来源：http://qxr.svipenyu.cn

C#:   base.Greet();
来源：http://gpn.ydzc1.top

[G08] 静态方法与属性
来源：http://icf.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qvw.0kj1m.cn

PHP:  public static function f() {}
来源：http://zfy.yongpay.top

JS:   static f() {}
来源：http://duc.hammf.cn

TS:   static f(): void {}
来源：http://zgs.xuanzx.com

Java: static void f() {}
来源：http://ley.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yls.ydzc1.top

Ruby: def self.f; end
来源：http://oby.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://woh.yuxming.cn

[G09] 接口 / 抽象类
来源：http://hjt.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://izi.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://cuw.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqt.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://jbx.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://kld.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://vcd.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uun.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://lpq.vqdsnc.cn


<!-- 参考信息 -->