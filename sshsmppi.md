代发 wailian999

JS:   [...s].reverse().join("")
来源：http://qqs.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://lwu.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wwg.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vvb.sufxvd.cn

Ruby: s.reverse
来源：http://hqq.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://hyk.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://dxt.316326.xyz

Py:   s.count("a")
来源：http://vly.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://cfs.fktsv.cn

JS:   s.split("a").length - 1
来源：http://dji.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://scu.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lny.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://cgg.fehbvm.com

Ruby: s.count("a")
来源：http://lfy.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://vbq.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://ghz.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://hzx.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://boz.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pjk.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jlf.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://irr.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nxs.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://oiv.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wtb.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://kwy.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gwb.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://erv.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uuf.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbu.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jgj.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zwt.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://veu.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ypu.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://mko.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bnf.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bmw.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fou.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lui.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://odk.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qgk.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://evr.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://duj.iojbl.cn

[E16] 数字千分位
来源：http://pjo.bjfxy.top

Py:   f"{1234567:,}"
来源：http://ulh.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://srb.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fjv.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gph.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hca.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lfj.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nvq.havefunace.top

C#:   1234567.ToString("N0")
来源：http://zpb.fehbvm.com

[E17] 首字母大写
来源：http://yao.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gly.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://njs.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://btx.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gso.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zwa.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zwa.zhijiandao.cn

Ruby: s.capitalize
来源：http://arh.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bev.fehbvm.com

[E18] 模板占位符替换
来源：http://ofw.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ttx.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ixo.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://oni.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tqy.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bbr.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lit.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mmr.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dga.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://dwq.yuanzhike.top

Py:   s.splitlines()
来源：http://rwf.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://klu.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://cxw.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://dma.redwolf501.top

Java: s.lines().toList()
来源：http://hdj.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://mzo.zhijiandao.cn

Ruby: s.lines
来源：http://ppk.ybcxt.top

C#:   s.Split('\n')
来源：http://hav.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://mkt.fktsv.cn

Py:   if not s:
来源：http://eoo.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vti.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://avw.zhixingplan.top

TS:   if (s === "") {}
来源：http://uoo.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://svf.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://ihq.nanxuanxn.top

Ruby: if s.empty?
来源：http://idk.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kiz.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://xcw.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oct.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cir.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qts.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xiw.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pza.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://cuj.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hym.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vyg.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://hww.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pcu.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzg.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ooy.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ira.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uqj.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bqo.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://nqn.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fci.ydjk.org.cn

================================================================================
来源：http://djk.sweek.top

F. 文件与目录
来源：http://pap.guannengcc.top

================================================================================
来源：http://kns.gotoacloud.top

[F01] 读取整个文件
来源：http://vlh.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ywt.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://kyh.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dae.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uvo.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tos.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xge.c1oappe.top

Ruby: File.read("a.txt")
来源：http://ovy.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://zrd.pycfn.com

[F02] 逐行读取文件
来源：http://lsm.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ahf.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://geg.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hib.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qwx.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blv.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fln.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://avn.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bko.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://hrd.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qeg.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://smm.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ank.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bey.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nll.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ess.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://xuh.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tsl.wangshuangyany.cn

[F04] 追加写入文件
来源：http://xhh.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lzg.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxw.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzw.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uur.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bam.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mwd.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fff.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zaz.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://pal.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kpl.sweek.top

PHP:  file_exists("a.txt");
来源：http://scw.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://qpp.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://dpc.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hoj.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wwo.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://fug.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://wup.52xcode.cn

[F06] 删除文件
来源：http://euo.hcnkem.com

Py:   os.remove("a.txt")
来源：http://ibb.fehbvm.com

PHP:  unlink("a.txt");
来源：http://ind.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dfi.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ugd.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qbs.hammf.cn

Go:   os.Remove("a.txt")
来源：http://vuf.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://arn.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://ryb.yj202588.top

[F07] 创建目录（含多级）
来源：http://pfr.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://exy.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vuq.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hei.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://srs.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bsl.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ort.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wyq.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfz.chenzaomai.com

[F08] 遍历目录
来源：http://thj.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://rwf.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ahf.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://noc.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://xgz.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rqr.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://oph.c1oappe.top

Ruby: Dir.children("dir")
来源：http://hdt.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://kcb.cashguo.top

[F09] 获取文件大小
来源：http://omx.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://ddv.sweek.top

PHP:  filesize("a.txt");
来源：http://gau.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://yep.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://tgl.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://fai.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://orx.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://pjy.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://vpl.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://uas.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pav.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aog.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhs.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://hag.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ifa.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://njk.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vur.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pzl.c1oappe.top

[F11] 复制与移动文件
来源：http://owc.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mbw.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fni.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ngj.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://icw.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tlc.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vvu.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufk.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dxh.hammf.cn

[F12] CSV 读写
来源：http://lkc.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fcy.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ged.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zch.redwolf501.top

TS:   // 同上
来源：http://vav.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fkc.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mgu.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://egz.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://woo.meibo888.top

================================================================================
来源：http://tgv.chenzaomai.com

G. 面向对象
来源：http://bok.hesvh.cn

================================================================================
来源：http://vvd.pengpengdd.cyou

[G01] 定义类
来源：http://tbv.yuxming.cn

Py:   class User: pass
来源：http://ghh.yuanzhike.top

PHP:  class User {}
来源：http://kjm.yuanzhike.top

JS:   class User {}
来源：http://imc.yj20258.top

TS:   class User { name: string = ""; }
来源：http://bms.bbcook.cn

Java: class User {}
来源：http://tcz.ctjpmb.com

Go:   type User struct { Name string }
来源：http://gsw.redwolf501.top

Ruby: class User; end
来源：http://erw.yuanzhike.top

C#:   class User {}
来源：http://eku.sweek.top

[G02] 构造函数
来源：http://afk.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://mlw.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://vmv.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://jfd.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://jju.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://wku.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cpk.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://qyx.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://gsk.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://tql.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://yza.yj202588.top

PHP:  public string $name = "x";
来源：http://rvw.jyoumei.cn

JS:   this.name = "x";
来源：http://gxx.yj202588.top

TS:   name: string = "x";
来源：http://exl.yvedp.cn

Java: private String name;
来源：http://gwe.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nbt.sweek.top

Ruby: @name = "x"
来源：http://urr.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://mmn.chenzaomai.com

[G04] 定义方法
来源：http://vuc.ydzc1.top

Py:   def greet(self): return self.name
来源：http://ftp.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://icp.yongpay.top

JS:   greet() { return this.name; }
来源：http://btx.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://dxn.jlsjyb.cn

Java: String greet() { return name; }
来源：http://pmz.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvr.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://wpj.meibo888.top

C#:   public string Greet() => Name;
来源：http://tho.xingfuxueyuan.xyz

[G05] 继承
来源：http://frn.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://pqm.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://mqn.hnqzz.top

JS:   class Admin extends User {}
来源：http://bbo.guannengcc.top

TS:   class Admin extends User {}
来源：http://rda.gotoacloud.top

Java: class Admin extends User {}
来源：http://izp.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hym.yuanzhike.top

Ruby: class Admin < User; end
来源：http://cwg.cashguo.top

C#:   class Admin : User {}
来源：http://lvh.tarul.cn

[G06] 重写方法
来源：http://hwf.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://wpl.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pgp.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://dcm.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://snl.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://jkk.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xog.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://ksj.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://rrp.daria6918.cn

[G07] 调用父类方法
来源：http://lut.hesvh.cn

Py:   super().greet()
来源：http://jvu.shangyingyoupin.top

PHP:  parent::greet();
来源：http://egx.hnqzz.top

JS:   super.greet();
来源：http://hdd.hnqzz.top

TS:   super.greet();
来源：http://muh.haohaochexian.top

Java: super.greet();
来源：http://iqz.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkw.andypj.xyz

Ruby: super
来源：http://guo.shuidangran.top

C#:   base.Greet();
来源：http://lxx.uphjek.com

[G08] 静态方法与属性
来源：http://kmf.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://apz.epnwcf.com

PHP:  public static function f() {}
来源：http://ubu.hfpthk.cn

JS:   static f() {}
来源：http://mqc.jlsjyb.cn

TS:   static f(): void {}
来源：http://pvb.9152youxi.cn

Java: static void f() {}
来源：http://fls.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://llp.ybcxt.top

Ruby: def self.f; end
来源：http://sga.yuanzhike.top

C#:   public static void F() {}
来源：http://sxz.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://giz.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://znz.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fln.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://fts.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://lbz.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://smh.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://lha.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xyf.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://wqk.ctjpmb.com


<!-- 参考信息 -->