代发 wailian999

Py:   for ch in s: print(ch)
来源：http://zzv.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://glm.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qne.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wsn.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vnd.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://odl.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ayb.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://shb.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://mxv.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://izo.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://naq.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ske.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cto.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hhh.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bcr.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://heq.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lli.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://nsq.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://trp.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ovs.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fuf.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://edy.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yjv.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sdx.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hwy.jiagoushi.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pdd.jlsjyb.cn

[E16] 数字千分位
来源：http://sxg.fktsv.cn

Py:   f"{1234567:,}"
来源：http://ybm.ivvv.top

PHP:  number_format(1234567);
来源：http://pcw.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://lia.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lsy.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vou.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zau.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ang.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://rco.epnwcf.com

[E17] 首字母大写
来源：http://bry.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uyg.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dvg.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fsw.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zmn.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jgb.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iqs.chenjidiqi.icu

Ruby: s.capitalize
来源：http://sdx.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wyr.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://wpn.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oqw.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ses.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wmb.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://psl.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nye.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://myb.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yvb.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dlx.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://vjh.xziqi.cn

Py:   s.splitlines()
来源：http://afo.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fmv.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://bdb.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://emg.sxryk.cn

Java: s.lines().toList()
来源：http://ads.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://dus.sweek.top

Ruby: s.lines
来源：http://amx.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://omn.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://dqd.xuanzx.com

Py:   if not s:
来源：http://mge.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://net.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ydp.daxiang520.top

TS:   if (s === "") {}
来源：http://cmn.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://wpt.pengpengdd.cyou

Go:   if s == "" {}
来源：http://ssc.dianchejie.cn

Ruby: if s.empty?
来源：http://qqr.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebq.9152youxi.cn

[E21] 超长截断加省略号
来源：http://cbo.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://njq.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rpt.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zcg.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbu.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://usj.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://wyu.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fwq.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qkn.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://mgz.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xhe.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://buy.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkg.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nuv.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ipo.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kzz.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://hht.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fjx.52xcode.cn

================================================================================
来源：http://noo.mhx1999.top

F. 文件与目录
来源：http://udt.epnwcf.com

================================================================================
来源：http://fon.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://xei.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://obv.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://ugg.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pvx.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eaw.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mkz.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ewu.tian-w.cn

Ruby: File.read("a.txt")
来源：http://vcm.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://xfq.kuanghao11.cn

[F02] 逐行读取文件
来源：http://bcl.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mjo.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sld.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lad.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://can.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjx.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mex.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bqy.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgm.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://bdy.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mat.mhx1999.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://des.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ulf.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffd.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ucu.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mzy.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://ccf.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jxb.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://tjd.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tam.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://olo.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aeh.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cie.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ayv.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tmu.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mkp.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rdq.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://rpq.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nov.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://yre.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://ypb.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://cnz.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://oeu.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dku.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://dks.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://dbn.pycfn.com

[F06] 删除文件
来源：http://ezw.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://xmj.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://gwd.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://gww.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://fjf.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jkh.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://wdp.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://fwo.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://kfc.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://arb.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nwa.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sly.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrk.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://knu.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rim.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ttv.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pqj.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pxx.hywenlv.cn

[F08] 遍历目录
来源：http://ghy.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qso.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zyu.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://kli.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://qjh.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gcc.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://fsh.cheryme.top

Ruby: Dir.children("dir")
来源：http://aag.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://obp.yuxming.cn

[F09] 获取文件大小
来源：http://sqa.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://bdn.sxryk.cn

PHP:  filesize("a.txt");
来源：http://wjp.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://pdy.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://fpc.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://pwk.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://idy.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://kbm.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://xtu.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://fan.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gtq.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ldy.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ilv.xuanzx.com

TS:   path.extname("a.txt")
来源：http://ouj.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lpq.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kti.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://beg.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://icr.yfazqb.com

[F11] 复制与移动文件
来源：http://ntr.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://izx.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rsy.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npi.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cik.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fnq.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uia.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufa.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqu.fanxiaobao.xyz

[F12] CSV 读写
来源：http://eso.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfv.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mlx.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kze.zhoulong.xyz

TS:   // 同上
来源：http://zyn.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gpu.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zck.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qot.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tpi.sweek.top

================================================================================
来源：http://nns.svipenyu.cn

G. 面向对象
来源：http://qpk.tarul.cn

================================================================================
来源：http://ugr.0kj1m.cn

[G01] 定义类
来源：http://siu.iojbl.cn

Py:   class User: pass
来源：http://adp.316326.xyz

PHP:  class User {}
来源：http://aky.tarul.cn

JS:   class User {}
来源：http://rrz.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://cva.vehdjk.com

Java: class User {}
来源：http://gti.yonumen.top

Go:   type User struct { Name string }
来源：http://jcl.jiagoushi.top

Ruby: class User; end
来源：http://ydx.daxiang520.top

C#:   class User {}
来源：http://uyi.cashguo.top

[G02] 构造函数
来源：http://cyb.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://nfb.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://tkr.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://auv.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://asi.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://dlk.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oej.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://viv.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://bqp.bjfxy.top

[G03] 实例属性
来源：http://ljg.jiagoushi.top

Py:   self.name = "x"
来源：http://njl.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://jer.sjlbkw.cn

JS:   this.name = "x";
来源：http://hzl.yueranfly.top

TS:   name: string = "x";
来源：http://xhc.shuidangran.top

Java: private String name;
来源：http://pek.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pbo.0kj1m.cn

Ruby: @name = "x"
来源：http://jij.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://dmr.jinqigufen.top

[G04] 定义方法
来源：http://ayr.aizwys.cn

Py:   def greet(self): return self.name
来源：http://lzr.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wfz.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://yyl.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://inn.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://gsa.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmy.zdbjq.cn

Ruby: def greet; @name; end
来源：http://lph.gzhubu.top

C#:   public string Greet() => Name;
来源：http://kqa.meibo888.top

[G05] 继承
来源：http://etl.52xcode.cn

Py:   class Admin(User): pass
来源：http://tei.zycfv.cn

PHP:  class Admin extends User {}
来源：http://gmg.tarul.cn

JS:   class Admin extends User {}
来源：http://usg.guowangkeji.top

TS:   class Admin extends User {}
来源：http://dfv.cqqwz.cn

Java: class Admin extends User {}
来源：http://yqq.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lql.iojbl.cn

Ruby: class Admin < User; end
来源：http://bbu.yfazqb.com

C#:   class Admin : User {}
来源：http://iru.chenzaomai.com

[G06] 重写方法
来源：http://jqu.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://jaj.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zoi.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://opw.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://qjc.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://tbc.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqk.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://swn.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://zir.gotoacloud.top

[G07] 调用父类方法
来源：http://ear.zhiwuduotai.top

Py:   super().greet()
来源：http://zjs.shangyingyoupin.top

PHP:  parent::greet();
来源：http://rvy.birdmap.top

JS:   super.greet();
来源：http://frk.xuanzx.com

TS:   super.greet();
来源：http://zny.c1oappe.top

Java: super.greet();
来源：http://vnt.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://szf.svipenyu.cn

Ruby: super
来源：http://dix.jlsjyb.cn

C#:   base.Greet();
来源：http://rpr.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://gva.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hjf.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://xwt.ctjpmb.com

JS:   static f() {}
来源：http://vfh.guannengcc.top

TS:   static f(): void {}
来源：http://ifg.snrcjt.cn

Java: static void f() {}
来源：http://fop.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dmj.wangshuangyany.cn

Ruby: def self.f; end
来源：http://kyg.wangdashe.top

C#:   public static void F() {}
来源：http://ovk.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://hyc.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://okc.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://auu.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jcd.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://tam.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://pnm.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://pvf.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yqv.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://maj.shuidangran.top

[G10] 访问控制
来源：http://jnr.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://itw.nanxuanxn.top

PHP:  public / protected / private
来源：http://czy.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://emh.ivvv.top

TS:   public / protected / private
来源：http://lib.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://hlk.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://orh.hcnkem.com

Ruby: public / protected / private
来源：http://ebe.tian-w.cn

C#:   public / protected / private / internal
来源：http://jmx.shanyushiyangtech.top

[G11] getter / setter
来源：http://twy.yj202588.top

Py:   @property 与 @x.setter
来源：http://yix.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jhi.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://apn.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://wwe.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://dkz.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nlj.cqqwz.cn


<!-- 参考信息 -->