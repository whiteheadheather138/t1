代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ujd.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://thw.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dar.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pno.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qdm.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aji.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dqc.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nmk.andypj.xyz

[E14] URL 编码与 Base64
来源：http://phg.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eeu.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://gwq.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zek.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ywl.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rgk.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qyb.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rxf.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qrr.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://utg.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qxj.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ovx.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pkf.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mpp.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://meu.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rlj.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ssi.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xtb.epnwcf.com

[E16] 数字千分位
来源：http://nqp.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://zbd.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://sjr.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://fub.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kmv.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bla.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fvj.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sgn.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://ftp.aizwys.cn

[E17] 首字母大写
来源：http://ddc.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ocy.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kru.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vdz.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsl.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xjo.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zur.pycfn.com

Ruby: s.capitalize
来源：http://phj.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rki.aibaodan.cn

[E18] 模板占位符替换
来源：http://tsk.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gjp.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yna.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tpr.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nwz.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ese.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dmw.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dsc.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://htm.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://jeb.xziqi.cn

Py:   s.splitlines()
来源：http://dli.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lzk.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://tja.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://hta.316326.xyz

Java: s.lines().toList()
来源：http://biq.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://fms.yvedp.cn

Ruby: s.lines
来源：http://fum.zhijiandao.cn

C#:   s.Split('\n')
来源：http://ykk.havefunace.top

[E20] 判断字符串是否为空
来源：http://oom.yfazqb.com

Py:   if not s:
来源：http://lwg.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftw.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dvu.tian-w.cn

TS:   if (s === "") {}
来源：http://rjp.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://che.birdmap.top

Go:   if s == "" {}
来源：http://nes.yongpay.top

Ruby: if s.empty?
来源：http://jdl.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://njg.hysaishi.cn

[E21] 超长截断加省略号
来源：http://huz.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bfb.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yld.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrz.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfg.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jva.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://luw.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xrc.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://smu.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://rqm.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zef.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sho.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsf.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxw.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fns.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zxt.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://cdp.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wzm.fanxiaobao.xyz

================================================================================
来源：http://ugd.birdmap.top

F. 文件与目录
来源：http://dnm.tian-w.cn

================================================================================
来源：http://ail.uphjek.com

[F01] 读取整个文件
来源：http://lqw.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uqr.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://esn.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://joi.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kxd.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://feq.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://byr.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://stq.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://vli.haohaochexian.top

[F02] 逐行读取文件
来源：http://noo.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ifm.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wnu.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://moa.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qwv.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fyu.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://poa.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wat.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://axm.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://var.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://urr.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://ybv.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pal.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://llt.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zzo.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://flt.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://fsn.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ncr.andypj.xyz

[F04] 追加写入文件
来源：http://noj.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://exu.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ode.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecf.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zpe.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qpg.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vrz.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nxq.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fpw.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://qgx.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wsj.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://xfn.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://uix.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://nqv.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ebn.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gku.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://gex.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://emd.guowangkeji.top

[F06] 删除文件
来源：http://gyq.tarul.cn

Py:   os.remove("a.txt")
来源：http://hvh.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://nxh.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gcv.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zqc.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://quk.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://eyh.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://jcv.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://ayf.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://kft.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emp.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://trw.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpx.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ouz.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kzh.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rfv.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvl.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hqc.hywenlv.cn

[F08] 遍历目录
来源：http://iqy.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vfu.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://omf.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://uqp.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://owd.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://elz.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ejp.ivvv.top

Ruby: Dir.children("dir")
来源：http://ooo.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://ihe.9152youxi.cn

[F09] 获取文件大小
来源：http://vry.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://aex.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://lzp.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://qmj.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://yji.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://lvm.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jmy.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://mdp.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://ict.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://epj.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dph.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ngq.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dxi.52xcode.cn

TS:   path.extname("a.txt")
来源：http://loa.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zha.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://afy.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ujj.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ssf.xylfe.cn

[F11] 复制与移动文件
来源：http://bko.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yev.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jts.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mox.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hyn.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fow.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pzu.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ira.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vle.zhiwuduotai.top

[F12] CSV 读写
来源：http://kxu.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wmq.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tgh.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://top.ppjwa.cn

TS:   // 同上
来源：http://ejr.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kuo.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qbp.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yvy.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ilp.gzhubu.top

================================================================================
来源：http://yab.jinyuanbaomall.cn

G. 面向对象
来源：http://nxa.uphjek.com

================================================================================
来源：http://hee.gzhubu.top

[G01] 定义类
来源：http://jyx.redwolf501.top

Py:   class User: pass
来源：http://tps.iojbl.cn

PHP:  class User {}
来源：http://kax.hnqzz.top

JS:   class User {}
来源：http://lwy.birdmap.top

TS:   class User { name: string = ""; }
来源：http://fyu.hongshengwenyu.top

Java: class User {}
来源：http://klf.uphjek.com

Go:   type User struct { Name string }
来源：http://vlc.yj20258888.top

Ruby: class User; end
来源：http://qnk.yongpay.top

C#:   class User {}
来源：http://eht.daria6918.cn

[G02] 构造函数
来源：http://wgm.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://vuy.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://ofp.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://qyf.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://tsd.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://iau.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bgv.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://rfz.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://uai.jiagoushi.top

[G03] 实例属性
来源：http://nuz.mhx1999.top

Py:   self.name = "x"
来源：http://wrl.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://oil.gzhubu.top

JS:   this.name = "x";
来源：http://kri.guannengcc.top

TS:   name: string = "x";
来源：http://poj.ivvv.top

Java: private String name;
来源：http://puo.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bsl.hcnkem.com

Ruby: @name = "x"
来源：http://oex.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://ego.uphjek.com

[G04] 定义方法
来源：http://rae.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://fes.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://slu.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://rfk.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://jjh.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://egp.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://axx.ctjpmb.com

Ruby: def greet; @name; end
来源：http://jfm.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://hug.zycfv.cn

[G05] 继承
来源：http://cqv.aizwys.cn

Py:   class Admin(User): pass
来源：http://ubg.cashguo.top

PHP:  class Admin extends User {}
来源：http://sbe.sysykeji.top

JS:   class Admin extends User {}
来源：http://mxq.ivvv.top

TS:   class Admin extends User {}
来源：http://imq.ydzc1.top

Java: class Admin extends User {}
来源：http://nfu.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vmw.fzhhl.top

Ruby: class Admin < User; end
来源：http://jij.jqgfzy.top

C#:   class Admin : User {}
来源：http://ilo.jinqigufen.top

[G06] 重写方法
来源：http://avp.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://aqy.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://miq.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://kev.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://tzc.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://ejh.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uqf.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://tst.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://hfv.tanke756.top

[G07] 调用父类方法
来源：http://aig.hywenlv.cn

Py:   super().greet()
来源：http://wah.yfazqb.com

PHP:  parent::greet();
来源：http://lmh.ppjwa.cn

JS:   super.greet();
来源：http://jln.uphjek.com

TS:   super.greet();
来源：http://gmi.havefunace.top

Java: super.greet();
来源：http://zir.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://trr.chenzaomai.com

Ruby: super
来源：http://ppt.52xcode.cn

C#:   base.Greet();
来源：http://tiz.yanxiufei.cn

[G08] 静态方法与属性
来源：http://jgh.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gju.316326.xyz

PHP:  public static function f() {}
来源：http://nok.yongpay.top

JS:   static f() {}
来源：http://jkm.zdqjudy.top

TS:   static f(): void {}
来源：http://zts.hnqzz.top

Java: static void f() {}
来源：http://fxq.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tcw.cdnleiting.top

Ruby: def self.f; end
来源：http://xdq.316326.xyz

C#:   public static void F() {}
来源：http://gbm.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://hca.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://sgh.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lyb.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://azr.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://waj.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://lzm.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://uty.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jih.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://qgk.gotoacloud.top

[G10] 访问控制
来源：http://ygq.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://jxv.hcnkem.com

PHP:  public / protected / private
来源：http://jnp.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://iyp.hnqzz.top

TS:   public / protected / private
来源：http://qvj.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://tqw.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qcb.sweek.top

Ruby: public / protected / private
来源：http://gie.52xcode.cn

C#:   public / protected / private / internal
来源：http://zex.haohaochexian.top

[G11] getter / setter
来源：http://for.iojbl.cn

Py:   @property 与 @x.setter
来源：http://ftt.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pgw.fengsongda.top

JS:   get name() { return this._name; }
来源：http://vfj.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://unh.vehdjk.com

Java: public String getName() { return name; }
来源：http://tai.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hlu.fengsongda.top


<!-- 参考信息 -->