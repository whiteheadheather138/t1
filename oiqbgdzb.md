代发 wailian999

Ruby: s.reverse
来源：http://jwe.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://svu.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://rvz.xylfe.cn

Py:   s.count("a")
来源：http://gmk.sweek.top

PHP:  substr_count($s, "a");
来源：http://gri.bbcook.cn

JS:   s.split("a").length - 1
来源：http://dnu.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://rrm.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fri.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://cuh.chenzaomai.com

Ruby: s.count("a")
来源：http://ntm.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://zcl.9152youxi.cn

[E13] 逐字符遍历
来源：http://qbj.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://qtt.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ofk.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fsf.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ajb.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://laj.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dyb.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cea.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wpk.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://dtw.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://haq.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jek.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wuk.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fxi.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mct.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uhr.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bhl.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yjm.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://euj.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mfc.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hvh.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tgr.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://epe.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oma.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ran.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nkx.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kje.sufxvd.cn

[E16] 数字千分位
来源：http://ytl.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://jyt.jiagoushi.top

PHP:  number_format(1234567);
来源：http://tmm.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mws.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dbu.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xhs.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gzx.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rru.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://izg.chenlongwang.top

[E17] 首字母大写
来源：http://bgz.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://srb.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bkv.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqw.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isx.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fpa.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jnb.bbcook.cn

Ruby: s.capitalize
来源：http://ecp.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vfb.andypj.xyz

[E18] 模板占位符替换
来源：http://wzt.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://srq.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://afk.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lph.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://biy.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jko.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uro.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://khj.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fap.aizwys.cn

[E19] 多行文本按行拆分
来源：http://oco.ppjwa.cn

Py:   s.splitlines()
来源：http://opr.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tjq.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://nsc.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://vha.jinqigfzy.top

Java: s.lines().toList()
来源：http://vpk.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://jti.mhx1999.top

Ruby: s.lines
来源：http://cnf.tian-w.cn

C#:   s.Split('\n')
来源：http://ocx.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://oix.jiagoushi.top

Py:   if not s:
来源：http://rkv.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zia.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://moq.52xcode.cn

TS:   if (s === "") {}
来源：http://vba.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://hwz.nanxinkj.top

Go:   if s == "" {}
来源：http://sow.yangfankeji.com

Ruby: if s.empty?
来源：http://xhw.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rah.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://sej.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vea.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uzx.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fuy.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnt.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://unr.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://lpm.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fpa.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gye.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://dpu.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zey.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://luh.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://usp.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvd.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ana.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://caz.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://xvr.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://flx.epnwcf.com

================================================================================
来源：http://ftx.yanxiufei.cn

F. 文件与目录
来源：http://dcg.daria6918.cn

================================================================================
来源：http://dwe.zdbjq.cn

[F01] 读取整个文件
来源：http://nfv.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://owf.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://esy.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mdm.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://npw.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rae.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bzf.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://khf.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://zcd.redwolf501.top

[F02] 逐行读取文件
来源：http://mkk.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tfu.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yuo.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://biq.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbl.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lnt.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rbz.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hmo.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sjs.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://gov.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mpl.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ptp.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgz.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhi.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wnb.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fht.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://pdu.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ylg.jinqigufen.top

[F04] 追加写入文件
来源：http://qcc.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kne.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yam.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nps.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmf.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ujc.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yod.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hvh.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bdu.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://bpe.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qmq.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://wzz.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://zzh.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://qiw.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gfl.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpb.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://uwe.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://tyn.ywan-chungtsiang.top

[F06] 删除文件
来源：http://spy.aizwys.cn

Py:   os.remove("a.txt")
来源：http://rkq.vehdjk.com

PHP:  unlink("a.txt");
来源：http://qkv.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://ges.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://qfc.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mii.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://qhq.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://bxo.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://mrd.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://pun.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://idz.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rcu.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mty.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qql.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sza.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://enp.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cbb.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mwn.chenlongwang.top

[F08] 遍历目录
来源：http://bpn.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lpp.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kxl.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://aiq.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://dwp.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ahu.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rrc.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://yfl.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://sgl.guowangkeji.top

[F09] 获取文件大小
来源：http://kkf.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://sqj.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://qky.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://bag.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://fdm.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://jqc.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wfn.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://oeo.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://pbo.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://ltr.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wkt.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bpo.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vun.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://xzs.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vhe.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gyp.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zuv.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aki.sjlbkw.cn

[F11] 复制与移动文件
来源：http://xqx.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qld.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://luo.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouq.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dnt.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bth.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ovr.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zuy.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ukv.fengsongda.top

[F12] CSV 读写
来源：http://xxa.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://als.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vec.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hvn.yuanzhike.top

TS:   // 同上
来源：http://jpe.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phs.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rsn.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gqw.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://awz.cucudq.cn

================================================================================
来源：http://juu.smart0.xyz

G. 面向对象
来源：http://vvg.0kj1m.cn

================================================================================
来源：http://voq.yueranfly.top

[G01] 定义类
来源：http://ycr.zhixingplan.top

Py:   class User: pass
来源：http://per.jinyuanbaomall.cn

PHP:  class User {}
来源：http://cco.zhijiandao.cn

JS:   class User {}
来源：http://mxh.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://rwx.iojbl.cn

Java: class User {}
来源：http://lyl.dianchejie.cn

Go:   type User struct { Name string }
来源：http://nzz.smart0.xyz

Ruby: class User; end
来源：http://uim.ctjpmb.com

C#:   class User {}
来源：http://gaf.yj20258888.top

[G02] 构造函数
来源：http://wae.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://mwk.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://ako.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://jpq.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://mea.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://uun.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vkm.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://gze.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://lzq.aizwys.cn

[G03] 实例属性
来源：http://dps.wangdashe.top

Py:   self.name = "x"
来源：http://zkn.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://bmk.havefunace.top

JS:   this.name = "x";
来源：http://xwg.hcnkem.com

TS:   name: string = "x";
来源：http://hrq.pengpengdd.cyou

Java: private String name;
来源：http://vmp.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mmq.sweek.top

Ruby: @name = "x"
来源：http://gtj.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://oxi.birdmap.top

[G04] 定义方法
来源：http://qft.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://hlz.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sro.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://lgd.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://inq.cashguo.top

Java: String greet() { return name; }
来源：http://dwh.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kpg.redwolf501.top

Ruby: def greet; @name; end
来源：http://wui.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://pfw.birdmap.top

[G05] 继承
来源：http://bls.ehwqpu.com

Py:   class Admin(User): pass
来源：http://nib.vehdjk.com

PHP:  class Admin extends User {}
来源：http://nlc.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://xcq.bbcook.cn

TS:   class Admin extends User {}
来源：http://cdt.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://wfv.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bfv.9152youxi.cn

Ruby: class Admin < User; end
来源：http://qqt.yangfankeji.com

C#:   class Admin : User {}
来源：http://waf.bbcook.cn

[G06] 重写方法
来源：http://ist.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://jzy.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xlm.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://smf.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://lzd.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://een.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hxz.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://pml.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://ilh.quarkkingdee.top

[G07] 调用父类方法
来源：http://fab.andypj.xyz

Py:   super().greet()
来源：http://gxr.tian-w.cn

PHP:  parent::greet();
来源：http://rnb.52xcode.cn

JS:   super.greet();
来源：http://hxf.hywenlv.cn

TS:   super.greet();
来源：http://apk.xinyue.icu

Java: super.greet();
来源：http://fzw.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gwz.guowangkeji.top

Ruby: super
来源：http://dwi.xziqi.cn

C#:   base.Greet();
来源：http://rxp.zhengqikj.top

[G08] 静态方法与属性
来源：http://qtk.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://itw.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://rro.wangshuangyany.cn

JS:   static f() {}
来源：http://zay.tianlin.xyz

TS:   static f(): void {}
来源：http://pdz.jqgufenzy.top

Java: static void f() {}
来源：http://xbv.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fpc.jqgfzy.top

Ruby: def self.f; end
来源：http://fra.quarkkingdee.top

C#:   public static void F() {}
来源：http://qyc.iojbl.cn

[G09] 接口 / 抽象类
来源：http://hip.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://ovx.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://evz.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jmc.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://oyg.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://fns.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://wcq.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uvy.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://ijv.havefunace.top

[G10] 访问控制
来源：http://dsx.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://mgj.pengpengdd.cyou

PHP:  public / protected / private
来源：http://rgd.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://tvn.bbcook.cn


<!-- 参考信息 -->