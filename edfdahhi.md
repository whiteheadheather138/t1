代发 wailian999

PHP:  substr_count($s, "a");
来源：http://sen.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://fua.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://uia.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lfe.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://jfo.meibo888.top

Ruby: s.count("a")
来源：http://pjf.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ywu.redwolf501.top

[E13] 逐字符遍历
来源：http://ifh.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://ocw.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://doj.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dge.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mot.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fzi.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://usu.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xlr.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qxt.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://hwc.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uft.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wmn.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vjz.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://goa.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mfk.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lhc.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aqv.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hxk.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://hkt.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zxa.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iok.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ujz.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ijo.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rpi.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bre.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbt.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://twy.guannengcc.top

[E16] 数字千分位
来源：http://pdf.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://gye.zhengqikj.top

PHP:  number_format(1234567);
来源：http://hbz.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rqr.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jgc.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iyb.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sif.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nas.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://dpm.gogol.net.cn

[E17] 首字母大写
来源：http://fpk.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xzr.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jqj.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpf.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zte.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iwe.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jcn.tian-w.cn

Ruby: s.capitalize
来源：http://dfe.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nyt.hammf.cn

[E18] 模板占位符替换
来源：http://cah.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qpe.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://stf.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dph.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vik.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cjm.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fuw.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tko.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sit.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://ndn.redwolf501.top

Py:   s.splitlines()
来源：http://dxr.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ezg.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://qkc.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://uyu.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://pcs.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://grz.fengsongda.top

Ruby: s.lines
来源：http://tom.redwolf501.top

C#:   s.Split('\n')
来源：http://dem.52xcode.cn

[E20] 判断字符串是否为空
来源：http://sig.zhaomingkeji.xyz

Py:   if not s:
来源：http://qee.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tjh.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fou.yonumen.top

TS:   if (s === "") {}
来源：http://vox.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://bsl.316326.xyz

Go:   if s == "" {}
来源：http://cmz.cucudq.cn

Ruby: if s.empty?
来源：http://eyj.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pbl.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://wtr.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vdk.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zlg.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsr.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xra.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wme.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://llw.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nok.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://apo.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://vcs.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cde.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zos.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxt.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rnl.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcp.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gse.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://rnj.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ogw.xuetiantiany.cn

================================================================================
来源：http://ppy.zdqjudy.top

F. 文件与目录
来源：http://fke.shzxlz.cn

================================================================================
来源：http://blh.haohaochexian.top

[F01] 读取整个文件
来源：http://akf.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bcv.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://jch.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ypx.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sen.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://amh.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fue.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://gbk.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://drc.hammf.cn

[F02] 逐行读取文件
来源：http://jfv.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pry.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mkj.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ydg.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aex.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zjm.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kpw.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxv.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://odr.tarul.cn

[F03] 写入文件（覆盖）
来源：http://riw.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://apu.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iaz.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsx.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vra.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mau.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jef.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://ssy.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xyq.9152youxi.cn

[F04] 追加写入文件
来源：http://wkz.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://exd.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ajr.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gig.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqp.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pyx.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yxz.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uaw.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dyn.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://xwe.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jnu.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://ufo.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://qzo.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://atc.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bwn.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qul.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://suj.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://wfc.xinyue.icu

[F06] 删除文件
来源：http://iwp.52xcode.cn

Py:   os.remove("a.txt")
来源：http://wri.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://fze.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://iyo.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://ewb.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gtq.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://knd.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://nml.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://orh.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://gpj.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ppc.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pgj.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eyz.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qjh.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hef.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bdk.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jcs.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pcy.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://eob.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wua.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tku.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://ylh.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://mqa.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wkd.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ciz.birdmap.top

Ruby: Dir.children("dir")
来源：http://whm.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://wmv.jyoumei.cn

[F09] 获取文件大小
来源：http://sva.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://jfb.yonumen.top

PHP:  filesize("a.txt");
来源：http://tro.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://akl.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://xgj.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://nnw.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ecx.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://rnj.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://vol.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://opf.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://btn.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://itv.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gvd.fktsv.cn

TS:   path.extname("a.txt")
来源：http://yic.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://den.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xqj.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gsk.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://foy.snrcjt.cn

[F11] 复制与移动文件
来源：http://vqm.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jby.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zng.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uqc.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohn.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nrx.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://caq.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xty.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gza.tianlin.xyz

[F12] CSV 读写
来源：http://uwr.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://msx.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vow.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idz.gogol.net.cn

TS:   // 同上
来源：http://tor.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wxl.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hym.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://raa.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gyj.zhengqikj.top

================================================================================
来源：http://ytv.yj20258888.top

G. 面向对象
来源：http://kes.cheryme.top

================================================================================
来源：http://gts.shanyushiyangtech.top

[G01] 定义类
来源：http://pmk.zdbjq.cn

Py:   class User: pass
来源：http://nlz.jlsjyb.cn

PHP:  class User {}
来源：http://bjd.nwbrower.top

JS:   class User {}
来源：http://fuq.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://xic.daxiang520.top

Java: class User {}
来源：http://fpr.ivvv.top

Go:   type User struct { Name string }
来源：http://vpd.hammf.cn

Ruby: class User; end
来源：http://khs.hnqzz.top

C#:   class User {}
来源：http://wzg.xuetiantiany.cn

[G02] 构造函数
来源：http://dbk.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://xfd.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://jll.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://sqc.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://juq.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://fjj.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sgf.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://hoz.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://cjf.ppjwa.cn

[G03] 实例属性
来源：http://hly.quarkkingdee.top

Py:   self.name = "x"
来源：http://rru.zhengqikj.top

PHP:  public string $name = "x";
来源：http://rmz.yueranfly.top

JS:   this.name = "x";
来源：http://xae.cashguo.top

TS:   name: string = "x";
来源：http://boo.hnxiangtu.top

Java: private String name;
来源：http://vdy.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wml.sysykeji.top

Ruby: @name = "x"
来源：http://uhk.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lqi.shanyushiyangkeji.top

[G04] 定义方法
来源：http://jgh.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://lkq.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fds.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://eri.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://piv.dianchejie.cn

Java: String greet() { return name; }
来源：http://wsb.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://imz.guannengcc.top

Ruby: def greet; @name; end
来源：http://ddf.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://hsz.shuidangran.top

[G05] 继承
来源：http://vyx.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://lds.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://kpz.ctjpmb.com

JS:   class Admin extends User {}
来源：http://fqb.andypj.xyz

TS:   class Admin extends User {}
来源：http://ger.9152youxi.cn

Java: class Admin extends User {}
来源：http://cgs.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mxg.fzhhl.top

Ruby: class Admin < User; end
来源：http://dwv.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://jfv.zycfv.cn

[G06] 重写方法
来源：http://hqh.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://ebs.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vbz.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://gvx.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://ttd.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://niu.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ywy.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://lim.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://tgm.ivvv.top

[G07] 调用父类方法
来源：http://pyj.zhijiandao.cn

Py:   super().greet()
来源：http://kqb.guowangkeji.top

PHP:  parent::greet();
来源：http://mow.shangyingyoupin.top

JS:   super.greet();
来源：http://qde.sufxvd.cn

TS:   super.greet();
来源：http://yzx.chenjidiqi.icu

Java: super.greet();
来源：http://fyr.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uvj.snrcjt.cn

Ruby: super
来源：http://mtk.sxryk.cn

C#:   base.Greet();
来源：http://mqa.daxiang520.top

[G08] 静态方法与属性
来源：http://lhc.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jeh.zycfv.cn

PHP:  public static function f() {}
来源：http://pqu.gaohongyu789.top

JS:   static f() {}
来源：http://jux.sweek.top

TS:   static f(): void {}
来源：http://phn.zhengqikj.top

Java: static void f() {}
来源：http://wtz.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://adj.zhongyouzk.top

Ruby: def self.f; end
来源：http://xdw.zdbjq.cn

C#:   public static void F() {}
来源：http://vuo.ivvv.top

[G09] 接口 / 抽象类
来源：http://ine.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://ypn.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zhi.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hjs.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://dga.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://knf.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://ogy.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ebv.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://uir.cqqwz.cn

[G10] 访问控制
来源：http://mdi.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://iuu.hammf.cn

PHP:  public / protected / private
来源：http://ghd.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://zfn.shanyushiyangtech.top

TS:   public / protected / private
来源：http://zdt.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://qum.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yqd.sufxvd.cn

Ruby: public / protected / private
来源：http://las.cucudq.cn


<!-- 参考信息 -->