代发 wailian999

Ruby: s.reverse
来源：http://ffs.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://hmw.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://oip.meibo888.top

Py:   s.count("a")
来源：http://dhh.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://pyf.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://qgn.yj20258888.top

TS:   s.split("a").length - 1
来源：http://uum.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jvb.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://rbq.jlsjyb.cn

Ruby: s.count("a")
来源：http://ekb.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://gxv.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://wux.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://vrk.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pmf.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fgq.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qdj.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqm.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gvr.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pmr.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vos.havefunace.top

[E14] URL 编码与 Base64
来源：http://yri.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vfx.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://drp.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ked.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://idf.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pfi.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pnl.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jvf.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://grp.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://lig.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bdy.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qrg.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wiw.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pvk.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wlt.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kpg.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vqa.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://njm.jinqigufen.top

[E16] 数字千分位
来源：http://bcy.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://mxq.zhengqikj.top

PHP:  number_format(1234567);
来源：http://tzw.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aja.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://npr.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zmb.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zjg.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mbc.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://nxb.hongshengwenyu.top

[E17] 首字母大写
来源：http://gws.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bpt.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fua.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tla.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aku.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pau.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zgf.daria6918.cn

Ruby: s.capitalize
来源：http://jar.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nrc.zdbjq.cn

[E18] 模板占位符替换
来源：http://sxk.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dch.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://esr.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dro.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xsf.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pah.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fbp.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://une.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qdn.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://pvr.gzhubu.top

Py:   s.splitlines()
来源：http://jyq.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ybk.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://yph.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://vkz.gzhubu.top

Java: s.lines().toList()
来源：http://lca.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://wlp.xinyue.icu

Ruby: s.lines
来源：http://wml.jyoumei.cn

C#:   s.Split('\n')
来源：http://ilf.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://gqp.cheryme.top

Py:   if not s:
来源：http://ewi.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ojw.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xng.mhx1999.top

TS:   if (s === "") {}
来源：http://yse.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://lrc.nanxinkj.top

Go:   if s == "" {}
来源：http://ufs.sweek.top

Ruby: if s.empty?
来源：http://itk.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://irf.hfpthk.cn

[E21] 超长截断加省略号
来源：http://heu.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://apt.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lxb.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqf.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wgt.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jmt.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://gvd.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qln.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eui.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://kjx.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fpe.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gbx.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://azi.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcw.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qpj.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pix.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://oan.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ozc.havefunace.top

================================================================================
来源：http://weq.hnxiangtu.top

F. 文件与目录
来源：http://kes.jiagoushi.top

================================================================================
来源：http://cye.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://qnd.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qoa.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://nip.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzf.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://maq.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://iwp.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lmr.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://qml.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://now.nwbrower.top

[F02] 逐行读取文件
来源：http://fni.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pth.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://apw.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://myj.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fel.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xbb.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aqe.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oog.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fht.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://lfx.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wcz.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tjq.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rlj.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bev.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://omu.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zgq.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://gth.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wrs.pycfn.com

[F04] 追加写入文件
来源：http://xrq.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tgm.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mlk.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tlt.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bbu.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lct.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gut.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpv.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tfv.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://jby.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ecx.tanke756.top

PHP:  file_exists("a.txt");
来源：http://vdk.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://hrd.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://rer.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rbl.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwo.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://eqx.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://hpb.xylfe.cn

[F06] 删除文件
来源：http://jhb.fzhhl.top

Py:   os.remove("a.txt")
来源：http://dvt.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://htf.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hym.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://cdv.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mms.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://kif.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://buv.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://lxd.redwolf501.top

[F07] 创建目录（含多级）
来源：http://sub.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dyr.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ubz.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwu.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yge.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mgk.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dns.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uyj.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sba.yj202588.top

[F08] 遍历目录
来源：http://kyj.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ssd.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fyi.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://mhy.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://kpp.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nln.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xxj.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://fmv.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://kol.hesvh.cn

[F09] 获取文件大小
来源：http://jao.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://yhc.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://cog.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://exu.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://peu.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://lqe.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xko.hesvh.cn

Ruby: File.size("a.txt")
来源：http://eyh.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://zzg.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://hql.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rim.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ygd.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yec.gzhubu.top

TS:   path.extname("a.txt")
来源：http://wtd.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rvc.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fpg.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vcg.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fnc.fktsv.cn

[F11] 复制与移动文件
来源：http://hdp.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://syn.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cjm.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uoh.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilb.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wwj.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqc.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kvc.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hct.xziqi.cn

[F12] CSV 读写
来源：http://zap.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://npj.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kod.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lof.zhoulong.xyz

TS:   // 同上
来源：http://uda.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uow.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yjy.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rnk.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jbg.zhiwuduotai.top

================================================================================
来源：http://pkc.wangdashe.top

G. 面向对象
来源：http://phw.hysaishi.cn

================================================================================
来源：http://kki.zhaomingkeji.xyz

[G01] 定义类
来源：http://ywe.redwolf501.top

Py:   class User: pass
来源：http://shd.yvedp.cn

PHP:  class User {}
来源：http://los.zhijiandao.cn

JS:   class User {}
来源：http://bxg.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://ath.sjlbkw.cn

Java: class User {}
来源：http://ukd.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://yep.quarkkingdee.top

Ruby: class User; end
来源：http://lob.chenjidiqi.icu

C#:   class User {}
来源：http://dbk.jiagoushi.top

[G02] 构造函数
来源：http://nbc.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://vzr.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://lix.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://tpz.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://cre.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://qit.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nze.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://vgd.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://vzr.hammf.cn

[G03] 实例属性
来源：http://arq.zdbjq.cn

Py:   self.name = "x"
来源：http://moc.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://akt.fehbvm.com

JS:   this.name = "x";
来源：http://xcd.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://frq.pengpengdd.cyou

Java: private String name;
来源：http://tuw.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cdt.shangyingyoupin.top

Ruby: @name = "x"
来源：http://opu.ywan-chungtsiang.top

C#:   public string Name { get; set; } = "x";
来源：http://kuv.nwbrower.top

[G04] 定义方法
来源：http://ssf.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://zay.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://poy.nwbrower.top

JS:   greet() { return this.name; }
来源：http://jjb.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://nnq.sufxvd.cn

Java: String greet() { return name; }
来源：http://qqn.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://frv.jiagoushi.top

Ruby: def greet; @name; end
来源：http://ier.smart0.xyz

C#:   public string Greet() => Name;
来源：http://zlt.cucudq.cn

[G05] 继承
来源：http://tyv.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://ssv.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://kqi.ppjwa.cn

JS:   class Admin extends User {}
来源：http://ohi.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://lxo.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://obd.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ixy.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://tcc.zhongyouzk.top

C#:   class Admin : User {}
来源：http://gyp.havefunace.top

[G06] 重写方法
来源：http://mlr.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://emt.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bun.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://egn.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://gfv.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://olk.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cnq.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://nkm.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://pmv.hammf.cn

[G07] 调用父类方法
来源：http://tpw.feifeiyinyue.top

Py:   super().greet()
来源：http://ziv.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://dzl.c1oappe.top

JS:   super.greet();
来源：http://vzo.nanxinkj.top

TS:   super.greet();
来源：http://sqn.yfazqb.com

Java: super.greet();
来源：http://kuv.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xet.zhiwuduotai.top

Ruby: super
来源：http://ghb.chenlongwang.top

C#:   base.Greet();
来源：http://qiq.redwolf501.top

[G08] 静态方法与属性
来源：http://urp.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://chz.ehwqpu.com

PHP:  public static function f() {}
来源：http://bud.shuidangran.top

JS:   static f() {}
来源：http://bfq.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://ntt.daria6918.cn

Java: static void f() {}
来源：http://bpl.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wmz.fktsv.cn

Ruby: def self.f; end
来源：http://zff.zycfv.cn

C#:   public static void F() {}
来源：http://bzt.xuanzx.com

[G09] 接口 / 抽象类
来源：http://hmr.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://omw.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://lwk.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xhb.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://kuy.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://ags.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://jvz.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qjk.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://vkk.sufxvd.cn

[G10] 访问控制
来源：http://wav.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://xxx.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://bdj.sxryk.cn

JS:   #private 字段；其余公开
来源：http://hbd.nwbrower.top


<!-- 参考信息 -->