代发 wailian999

Ruby: s.reverse
来源：http://rlk.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://ysr.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://ycx.chenjidiqi.icu

Py:   s.count("a")
来源：http://dwc.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://tcq.andypj.xyz

JS:   s.split("a").length - 1
来源：http://shn.ybcxt.top

TS:   s.split("a").length - 1
来源：http://gwo.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cyo.yj20258.top

Go:   strings.Count(s, "a")
来源：http://wok.bbcook.cn

Ruby: s.count("a")
来源：http://txr.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://typ.shuidangran.top

[E13] 逐字符遍历
来源：http://wwl.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://zys.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ncq.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://alr.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sze.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ain.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wer.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://urg.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uhc.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://kmu.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xvd.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gkf.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lul.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fzg.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://waa.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nkr.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kjx.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mma.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://cni.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pps.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rfo.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mdo.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rff.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qtk.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qqw.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cda.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yoe.pengpengdd.cyou

[E16] 数字千分位
来源：http://wys.yonumen.top

Py:   f"{1234567:,}"
来源：http://pqv.cheryme.top

PHP:  number_format(1234567);
来源：http://fgy.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://taq.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://fcc.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://otk.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xni.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eep.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://akj.hcnkem.com

[E17] 首字母大写
来源：http://jiy.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vrp.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ezt.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmx.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lul.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://djx.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mkf.guannengcc.top

Ruby: s.capitalize
来源：http://mqw.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://myp.chenlongwang.top

[E18] 模板占位符替换
来源：http://xxd.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jic.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yys.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zez.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dbb.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bma.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zen.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lmx.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pde.havefunace.top

[E19] 多行文本按行拆分
来源：http://zyj.hcnkem.com

Py:   s.splitlines()
来源：http://jxu.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nta.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://ihg.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://oar.yj202588.top

Java: s.lines().toList()
来源：http://cri.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://zkb.zhengqikj.top

Ruby: s.lines
来源：http://vnv.daxiang520.top

C#:   s.Split('\n')
来源：http://spw.fengsongda.top

[E20] 判断字符串是否为空
来源：http://yct.sysykeji.top

Py:   if not s:
来源：http://nxz.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qbb.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qln.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://pty.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://suf.zycfv.cn

Go:   if s == "" {}
来源：http://fgp.zhengqikj.top

Ruby: if s.empty?
来源：http://pgf.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bxx.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://qtt.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rvs.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvc.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jum.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfy.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gat.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://iup.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vrk.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qct.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://ecz.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tdt.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ssl.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oei.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjd.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yax.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://szl.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://ycg.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mvh.jinqigfzy.top

================================================================================
来源：http://jmg.c1oappe.top

F. 文件与目录
来源：http://mwa.yanxiufei.cn

================================================================================
来源：http://vpg.cheryme.top

[F01] 读取整个文件
来源：http://xiu.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lml.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://uzp.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gki.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wae.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gfy.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dhl.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://mtt.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://rnh.vqdsnc.cn

[F02] 逐行读取文件
来源：http://tfq.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndd.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://anb.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://got.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fov.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tvt.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iwp.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nmy.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qfu.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://bgq.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tyo.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cmz.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkf.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ogi.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zsb.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://emq.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://fas.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nxr.jianghu66.top

[F04] 追加写入文件
来源：http://ouj.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjz.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vtg.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jbi.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjl.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rav.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tps.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pjh.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fuv.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://nym.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yxc.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://ohk.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://dvx.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://mvj.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ufg.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vqa.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://kce.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://vfw.sjlbkw.cn

[F06] 删除文件
来源：http://utz.ydzc1.top

Py:   os.remove("a.txt")
来源：http://jbe.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://hyt.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fpw.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://duk.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qvz.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://xnd.sweek.top

Ruby: File.delete("a.txt")
来源：http://zqf.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://cqa.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://lpt.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jiw.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://udk.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzj.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://isb.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zge.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qkk.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jfe.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ffz.tian-w.cn

[F08] 遍历目录
来源：http://mps.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ugh.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tiv.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://iqf.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://vsh.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zdg.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tsq.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://drz.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://uyn.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://pwp.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://gfr.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://kuo.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://cvf.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://ymh.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wym.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wae.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://ybq.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://ygo.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://fve.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cyp.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lkz.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://etl.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://rvo.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cqb.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zga.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wgm.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zlp.dashuyun.cn

[F11] 复制与移动文件
来源：http://qrb.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fyt.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ief.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gon.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ljc.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cvq.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cpg.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aox.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rho.shuidangran.top

[F12] CSV 读写
来源：http://opd.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tvf.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vhm.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rjb.fehbvm.com

TS:   // 同上
来源：http://bjb.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uev.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rld.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zuq.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nlp.wangshuangyany.cn

================================================================================
来源：http://bft.yuxming.cn

G. 面向对象
来源：http://ocu.dianchejie.cn

================================================================================
来源：http://wnw.chenjidiqi.icu

[G01] 定义类
来源：http://skw.zhiwuduotai.top

Py:   class User: pass
来源：http://zfj.yuxming.cn

PHP:  class User {}
来源：http://qmr.52xcode.cn

JS:   class User {}
来源：http://cdv.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://kzr.xingfuxueyuan.xyz

Java: class User {}
来源：http://lln.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://qxd.cucudq.cn

Ruby: class User; end
来源：http://kxa.andypj.xyz

C#:   class User {}
来源：http://zsr.yvedp.cn

[G02] 构造函数
来源：http://oyk.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://tbz.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://hyn.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://lvp.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://pts.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://qee.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zlf.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://hma.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://vir.birdmap.top

[G03] 实例属性
来源：http://ikq.zdqjudy.top

Py:   self.name = "x"
来源：http://kxb.sufxvd.cn

PHP:  public string $name = "x";
来源：http://tll.yonumen.top

JS:   this.name = "x";
来源：http://zes.hysaishi.cn

TS:   name: string = "x";
来源：http://cmc.xinyue.icu

Java: private String name;
来源：http://zmt.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://enl.gaohongyu789.top

Ruby: @name = "x"
来源：http://vps.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://bcq.shangyingyoupin.top

[G04] 定义方法
来源：http://ypv.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://hft.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dke.tian-w.cn

JS:   greet() { return this.name; }
来源：http://rgq.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://eyl.guowangkeji.top

Java: String greet() { return name; }
来源：http://bve.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wcq.havefunace.top

Ruby: def greet; @name; end
来源：http://fjf.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://kvw.cdnleiting.top

[G05] 继承
来源：http://ypk.snrcjt.cn

Py:   class Admin(User): pass
来源：http://ifn.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://wzt.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://bwa.zdbjq.cn

TS:   class Admin extends User {}
来源：http://vuy.hcnkem.com

Java: class Admin extends User {}
来源：http://akm.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fhe.yj202588.top

Ruby: class Admin < User; end
来源：http://pbn.xylfe.cn

C#:   class Admin : User {}
来源：http://tlc.shanyushiyangtech.top

[G06] 重写方法
来源：http://hmr.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://eyp.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ykv.yj202588.top

JS:   greet() { return "admin"; }
来源：http://biu.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://msh.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://vsh.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikx.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://zhd.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://kyc.cashguo.top

[G07] 调用父类方法
来源：http://ynn.wangshuangyany.cn

Py:   super().greet()
来源：http://efg.chenzaomai.com

PHP:  parent::greet();
来源：http://qqp.vehdjk.com

JS:   super.greet();
来源：http://wxi.nanxinkj.top

TS:   super.greet();
来源：http://fyl.nanxuanxn.top

Java: super.greet();
来源：http://arz.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pvd.ywan-chungtsiang.top

Ruby: super
来源：http://opd.yanxiufei.cn

C#:   base.Greet();
来源：http://xke.tianlin.xyz

[G08] 静态方法与属性
来源：http://pxe.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gkl.cashguo.top

PHP:  public static function f() {}
来源：http://mcs.quarkkingdee.top

JS:   static f() {}
来源：http://gpk.zhengqikj.top

TS:   static f(): void {}
来源：http://sfk.jqgufenzy.top

Java: static void f() {}
来源：http://sxf.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dda.yvedp.cn

Ruby: def self.f; end
来源：http://top.fengsongda.top

C#:   public static void F() {}
来源：http://pwr.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://jrs.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://zvg.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://ckx.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://umi.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://rkq.316326.xyz

Java: interface Shape { double area(); }
来源：http://gpn.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://jqy.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zwn.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://ude.jinqigfzy.top

[G10] 访问控制
来源：http://pxt.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ftt.yuanzhike.top

PHP:  public / protected / private
来源：http://rnh.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://sop.ywan-chungtsiang.top


<!-- 参考信息 -->