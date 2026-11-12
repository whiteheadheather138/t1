代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ocb.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oce.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://dkx.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ktl.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kwg.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wzh.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kca.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ihd.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://wjf.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jjp.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lds.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gqu.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xfh.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fzw.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zjk.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mrz.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bea.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://pmz.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ayc.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wai.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mzj.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://stf.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qiu.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aou.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://smu.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nhr.yj20258888.top

[E16] 数字千分位
来源：http://isx.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://ifl.tianlin.xyz

PHP:  number_format(1234567);
来源：http://dcj.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://niw.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hbt.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vmv.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rvi.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mat.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://oow.tarul.cn

[E17] 首字母大写
来源：http://diw.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qth.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dqp.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbo.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zvq.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fht.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://msc.daria6918.cn

Ruby: s.capitalize
来源：http://bph.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wrz.zhixingplan.top

[E18] 模板占位符替换
来源：http://thl.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ixn.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ezk.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wqw.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jqv.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bdk.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pqk.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://opm.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hol.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://bcb.mhx1999.top

Py:   s.splitlines()
来源：http://cez.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ngc.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://zga.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://tsg.nanxinkj.top

Java: s.lines().toList()
来源：http://rhh.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://qkl.redwolf501.top

Ruby: s.lines
来源：http://sjl.guowangkeji.top

C#:   s.Split('\n')
来源：http://ssz.sweek.top

[E20] 判断字符串是否为空
来源：http://oxp.sxryk.cn

Py:   if not s:
来源：http://gtg.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vtf.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xkf.jlsjyb.cn

TS:   if (s === "") {}
来源：http://jfw.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://tqn.hywenlv.cn

Go:   if s == "" {}
来源：http://qcd.quarkkingdee.top

Ruby: if s.empty?
来源：http://sek.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vwm.yongpay.top

[E21] 超长截断加省略号
来源：http://xoi.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfb.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fql.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qhs.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xen.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wsh.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://cfr.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mrl.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqm.sxryk.cn

[E22] 字节长度与字符长度
来源：http://pih.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ljg.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zxu.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zpy.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hsp.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cjb.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://apc.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://blx.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izj.yongpay.top

================================================================================
来源：http://dvr.chenjidiqi.icu

F. 文件与目录
来源：http://vwg.hesvh.cn

================================================================================
来源：http://cyq.fehbvm.com

[F01] 读取整个文件
来源：http://plt.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ohy.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://zrw.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ccg.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tgp.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cch.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pit.hammf.cn

Ruby: File.read("a.txt")
来源：http://lfr.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://mne.zhixingplan.top

[F02] 逐行读取文件
来源：http://oid.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nqt.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ssb.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kmb.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nsn.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzl.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqg.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ljw.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lgz.meibo888.top

[F03] 写入文件（覆盖）
来源：http://btv.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eie.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsr.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tev.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ltt.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jef.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://edo.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://oib.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qdp.pengpengdd.cyou

[F04] 追加写入文件
来源：http://dvf.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tck.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bdu.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wsf.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kov.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pxt.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hap.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dik.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qhb.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://fif.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tys.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://ywx.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://lev.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://upb.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xcb.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bnu.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://xfa.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://bed.aibaodan.cn

[F06] 删除文件
来源：http://mye.redwolf501.top

Py:   os.remove("a.txt")
来源：http://luj.52xcode.cn

PHP:  unlink("a.txt");
来源：http://lns.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://sfv.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://swy.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uvp.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://wxv.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://kor.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://htt.bbcook.cn

[F07] 创建目录（含多级）
来源：http://sey.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jvf.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nhc.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pbo.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yni.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ouk.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://duc.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lch.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://plq.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://oeo.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://qvd.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dna.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://bxo.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://fzc.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://elq.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xgr.iojbl.cn

Ruby: Dir.children("dir")
来源：http://osh.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://cqf.jinqigfzy.top

[F09] 获取文件大小
来源：http://uqd.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://beh.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://ovf.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://gxi.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://lzs.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://nqh.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://drn.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://xlm.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://cfs.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zjl.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fel.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sib.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vlk.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://ziz.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://arv.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rhu.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dzq.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://czl.fktsv.cn

[F11] 复制与移动文件
来源：http://fbw.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xzj.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wpd.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ltq.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jdh.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nyd.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lea.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zhw.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://epd.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://ehp.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yuw.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvk.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://clq.cdnleiting.top

TS:   // 同上
来源：http://zbj.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rdi.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xfu.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oyv.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tka.nwbrower.top

================================================================================
来源：http://ilv.xylfe.cn

G. 面向对象
来源：http://qew.jyoumei.cn

================================================================================
来源：http://ldh.ydzc1.top

[G01] 定义类
来源：http://ifl.ehwqpu.com

Py:   class User: pass
来源：http://ciq.aizwys.cn

PHP:  class User {}
来源：http://xnl.nwbrower.top

JS:   class User {}
来源：http://xwo.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://zys.jinqigfzy.top

Java: class User {}
来源：http://bbe.hesvh.cn

Go:   type User struct { Name string }
来源：http://uvq.hesvh.cn

Ruby: class User; end
来源：http://uoa.vehdjk.com

C#:   class User {}
来源：http://tin.fengsongda.top

[G02] 构造函数
来源：http://pho.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://vrj.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://pdm.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://jto.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://eck.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://erf.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gfr.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://uru.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://hvk.yongpay.top

[G03] 实例属性
来源：http://zic.jyoumei.cn

Py:   self.name = "x"
来源：http://vqg.epnwcf.com

PHP:  public string $name = "x";
来源：http://tll.aizwys.cn

JS:   this.name = "x";
来源：http://qvw.0kj1m.cn

TS:   name: string = "x";
来源：http://lvu.havefunace.top

Java: private String name;
来源：http://qox.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tcl.aibaodan.cn

Ruby: @name = "x"
来源：http://yhu.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://wxo.gogol.net.cn

[G04] 定义方法
来源：http://nrl.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://xhy.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tuw.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://xag.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://rmg.cashguo.top

Java: String greet() { return name; }
来源：http://feq.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jwb.guannengcc.top

Ruby: def greet; @name; end
来源：http://fyf.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://niq.kuanghao11.cn

[G05] 继承
来源：http://dej.yfazqb.com

Py:   class Admin(User): pass
来源：http://ypx.yongpay.top

PHP:  class Admin extends User {}
来源：http://ntd.hfpthk.cn

JS:   class Admin extends User {}
来源：http://wvl.hesvh.cn

TS:   class Admin extends User {}
来源：http://zgl.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://rgh.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bwt.redwolf501.top

Ruby: class Admin < User; end
来源：http://zhd.cdnleiting.top

C#:   class Admin : User {}
来源：http://tns.daria6918.cn

[G06] 重写方法
来源：http://nvr.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://pyu.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ufi.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://xou.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://tpg.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://psr.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gxa.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://hly.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://iho.dianchejie.cn

[G07] 调用父类方法
来源：http://pfw.ppjwa.cn

Py:   super().greet()
来源：http://ukp.jqgufenzy.top

PHP:  parent::greet();
来源：http://sqw.feifeiyinyue.top

JS:   super.greet();
来源：http://irp.svipenyu.cn

TS:   super.greet();
来源：http://ywp.fktsv.cn

Java: super.greet();
来源：http://njv.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gwj.yj20258.top

Ruby: super
来源：http://xth.gaohongyu789.top

C#:   base.Greet();
来源：http://oqn.daxiang520.top

[G08] 静态方法与属性
来源：http://suk.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ohv.vehdjk.com

PHP:  public static function f() {}
来源：http://uvm.yanxiufei.cn

JS:   static f() {}
来源：http://wte.yj20258888.top

TS:   static f(): void {}
来源：http://jiy.daxiang520.top

Java: static void f() {}
来源：http://edb.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qng.dianchejie.cn

Ruby: def self.f; end
来源：http://mgd.uphjek.com

C#:   public static void F() {}
来源：http://vfe.hcnkem.com

[G09] 接口 / 抽象类
来源：http://xdg.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://bjy.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://fdl.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hvt.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://ros.hnqzz.top

Java: interface Shape { double area(); }
来源：http://iww.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://ddc.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pjd.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://kuz.hesvh.cn

[G10] 访问控制
来源：http://dbr.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://ykg.vqdsnc.cn

PHP:  public / protected / private
来源：http://pkg.yj20258.top

JS:   #private 字段；其余公开
来源：http://ssq.jinghuilouyu.cn

TS:   public / protected / private
来源：http://kar.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://scp.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgp.kuanghao11.cn

Ruby: public / protected / private
来源：http://tom.yfazqb.com

C#:   public / protected / private / internal
来源：http://hlf.vqdsnc.cn

[G11] getter / setter
来源：http://xps.redwolf501.top

Py:   @property 与 @x.setter
来源：http://pwl.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ugo.jianghu66.top

JS:   get name() { return this._name; }
来源：http://kbj.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://jzy.yangfankeji.com

Java: public String getName() { return name; }
来源：http://dyu.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rxe.daxiang520.top


<!-- 参考信息 -->