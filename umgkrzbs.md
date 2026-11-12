代发 wailian999

PHP:  substr_count($s, "a");
来源：http://ryx.shuidangran.top

JS:   s.split("a").length - 1
来源：http://byk.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://clc.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cli.hammf.cn

Go:   strings.Count(s, "a")
来源：http://fmi.kuanghao11.cn

Ruby: s.count("a")
来源：http://zxn.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://xnn.ydzc1.top

[E13] 逐字符遍历
来源：http://wkw.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://xid.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://abk.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgg.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rys.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xdc.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wpy.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://csy.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://smm.yonumen.top

[E14] URL 编码与 Base64
来源：http://jwq.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bkd.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hpg.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mci.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hbu.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jij.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qko.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jxz.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wty.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://clj.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://blr.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://npu.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bnn.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://beb.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mph.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://scv.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://krv.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://utv.jiagoushi.top

[E16] 数字千分位
来源：http://fdd.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://xrh.316326.xyz

PHP:  number_format(1234567);
来源：http://ubs.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mun.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kgy.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pjh.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mqt.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aju.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://dpd.yanxiufei.cn

[E17] 首字母大写
来源：http://lfz.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aip.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uey.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsn.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://veh.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gcz.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://huw.xuetiantiany.cn

Ruby: s.capitalize
来源：http://vrz.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ykf.gogol.net.cn

[E18] 模板占位符替换
来源：http://rpy.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://psy.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zzi.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wum.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ywq.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ejq.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lky.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xhz.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vlo.meibo888.top

[E19] 多行文本按行拆分
来源：http://ebx.nwbrower.top

Py:   s.splitlines()
来源：http://nkw.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yoh.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://xpp.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://acp.jinqigufen.top

Java: s.lines().toList()
来源：http://wkj.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://tta.zdqjudy.top

Ruby: s.lines
来源：http://hlk.svipenyu.cn

C#:   s.Split('\n')
来源：http://yjx.xinyue.icu

[E20] 判断字符串是否为空
来源：http://nzb.chenjidiqi.icu

Py:   if not s:
来源：http://aju.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vxv.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uml.hfpthk.cn

TS:   if (s === "") {}
来源：http://goj.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://bfc.xinyue.icu

Go:   if s == "" {}
来源：http://rrz.vehdjk.com

Ruby: if s.empty?
来源：http://gew.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sul.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://xpx.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktv.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eub.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mtp.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbw.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://git.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://oji.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kex.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yxh.fktsv.cn

[E22] 字节长度与字符长度
来源：http://gvi.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qrn.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfa.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ecu.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwq.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qbv.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uth.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://amr.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kyo.shzxlz.cn

================================================================================
来源：http://tlu.shanyushiyangtech.top

F. 文件与目录
来源：http://ogq.shuidangran.top

================================================================================
来源：http://sxp.mhx1999.top

[F01] 读取整个文件
来源：http://qma.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzj.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://vvz.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://inf.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fzt.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kin.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rfp.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://fcp.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://gow.haohaochexian.top

[F02] 逐行读取文件
来源：http://bry.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ckr.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rfu.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihe.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pns.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqd.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cyw.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukd.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://huf.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://wgl.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jbr.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jcb.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gad.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozg.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tei.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bua.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://qrx.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pjz.fengsongda.top

[F04] 追加写入文件
来源：http://bjc.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yoj.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mwj.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxg.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cdt.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fen.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zog.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mym.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wbe.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://isz.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rad.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://qga.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://jso.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://ags.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sbk.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tfk.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://iel.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://tya.xinyue.icu

[F06] 删除文件
来源：http://dcr.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://smw.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://cbr.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://cqf.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://mfv.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wed.tarul.cn

Go:   os.Remove("a.txt")
来源：http://pak.yj20258.top

Ruby: File.delete("a.txt")
来源：http://xqa.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://hdr.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://pet.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xlj.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vmg.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yhb.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjm.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vjb.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfz.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mbt.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aav.daria6918.cn

[F08] 遍历目录
来源：http://ten.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://muk.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://egt.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://vdg.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://quy.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dvq.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sqq.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://nse.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://gyw.yuxming.cn

[F09] 获取文件大小
来源：http://lfm.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://wvr.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://viq.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://jop.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://mvg.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://rdw.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tks.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://kgg.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://cxe.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://hdt.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vrs.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cnv.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oqy.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://blx.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vxj.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bwc.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dfj.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjm.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://rvd.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yjb.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wac.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nxt.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdg.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ryp.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://amf.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vvq.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://saj.snrcjt.cn

[F12] CSV 读写
来源：http://gdb.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dia.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fez.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oxj.zhengqikj.top

TS:   // 同上
来源：http://rwm.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nlf.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgx.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gdn.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vfs.cashguo.top

================================================================================
来源：http://cdn.svipenyu.cn

G. 面向对象
来源：http://jkx.guannengcc.top

================================================================================
来源：http://fjs.hammf.cn

[G01] 定义类
来源：http://ain.mhx1999.top

Py:   class User: pass
来源：http://ldq.9152youxi.cn

PHP:  class User {}
来源：http://fib.feifeiyinyue.top

JS:   class User {}
来源：http://qae.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://bfv.hnxiangtu.top

Java: class User {}
来源：http://zho.sysykeji.top

Go:   type User struct { Name string }
来源：http://pmf.sxryk.cn

Ruby: class User; end
来源：http://wvt.aizwys.cn

C#:   class User {}
来源：http://wak.bbcook.cn

[G02] 构造函数
来源：http://npt.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dai.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://elh.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://ncd.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://lze.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://ydt.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ecb.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://git.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://ybf.yfazqb.com

[G03] 实例属性
来源：http://viy.yfazqb.com

Py:   self.name = "x"
来源：http://zbb.daxiang520.top

PHP:  public string $name = "x";
来源：http://qsv.hammf.cn

JS:   this.name = "x";
来源：http://afo.yvedp.cn

TS:   name: string = "x";
来源：http://wrb.andypj.xyz

Java: private String name;
来源：http://sgs.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gjh.ivvv.top

Ruby: @name = "x"
来源：http://ozs.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://vlo.tarul.cn

[G04] 定义方法
来源：http://dgi.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://smx.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zbz.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://bar.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://tpe.zhijiandao.cn

Java: String greet() { return name; }
来源：http://zeh.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jqg.pycfn.com

Ruby: def greet; @name; end
来源：http://eau.fehbvm.com

C#:   public string Greet() => Name;
来源：http://hbx.nanxinkj.top

[G05] 继承
来源：http://tdh.ctjpmb.com

Py:   class Admin(User): pass
来源：http://gqz.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://qno.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://clm.bjfxy.top

TS:   class Admin extends User {}
来源：http://moz.sxryk.cn

Java: class Admin extends User {}
来源：http://xxy.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://abn.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://frt.zhengqikj.top

C#:   class Admin : User {}
来源：http://hgj.sxryk.cn

[G06] 重写方法
来源：http://tfm.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://jhr.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://crt.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://ilc.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://lwy.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://mns.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wsj.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://hwh.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://eqn.xziqi.cn

[G07] 调用父类方法
来源：http://oor.sxryk.cn

Py:   super().greet()
来源：http://yzz.fzhhl.top

PHP:  parent::greet();
来源：http://srd.fanxiaobao.xyz

JS:   super.greet();
来源：http://gwh.0kj1m.cn

TS:   super.greet();
来源：http://yea.xuetiantiany.cn

Java: super.greet();
来源：http://jgl.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cur.epnwcf.com

Ruby: super
来源：http://vrq.gzhubu.top

C#:   base.Greet();
来源：http://emm.hcnkem.com

[G08] 静态方法与属性
来源：http://iiz.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wps.meibo888.top

PHP:  public static function f() {}
来源：http://irz.pycfn.com

JS:   static f() {}
来源：http://jza.hysaishi.cn

TS:   static f(): void {}
来源：http://yoz.zycfv.cn

Java: static void f() {}
来源：http://ntk.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tzy.sufxvd.cn

Ruby: def self.f; end
来源：http://svg.hfpthk.cn

C#:   public static void F() {}
来源：http://abo.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://ovk.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://uhu.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://rky.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nuv.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://zng.yuxming.cn

Java: interface Shape { double area(); }
来源：http://xfp.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://gra.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tot.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://vku.tianlin.xyz

[G10] 访问控制
来源：http://xsw.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://ysl.c1oappe.top

PHP:  public / protected / private
来源：http://gfv.guannengcc.top

JS:   #private 字段；其余公开
来源：http://ubu.quarkkingdee.top

TS:   public / protected / private
来源：http://smk.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://vmm.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qvk.cheryme.top

Ruby: public / protected / private
来源：http://qft.zhoulong.xyz


<!-- 参考信息 -->