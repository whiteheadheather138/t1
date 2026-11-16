代发 wailian999

Ruby: s.reverse
来源：http://kvf.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qit.zycfv.cn

[E12] 统计某字符出现次数
来源：http://bvq.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://kqq.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://mnt.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://jxd.yfazqb.com

TS:   s.split("a").length - 1
来源：http://nya.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gym.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://kvi.jqgfzy.top

Ruby: s.count("a")
来源：http://trb.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ink.aizwys.cn

[E13] 逐字符遍历
来源：http://hmo.yj20258.top

Py:   for ch in s: print(ch)
来源：http://sza.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bda.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nyz.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gpp.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iae.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mgz.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lqq.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gce.sysykeji.top

[E14] URL 编码与 Base64
来源：http://yew.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qnw.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uoo.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eoa.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://laj.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cmp.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lum.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fis.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://akw.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://hnr.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://evg.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://enc.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yvi.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lbn.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vwl.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xms.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zax.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bfk.gzhubu.top

[E16] 数字千分位
来源：http://ekw.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://jbm.cqqwz.cn

PHP:  number_format(1234567);
来源：http://abg.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://trr.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cak.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xbw.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://stt.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wrk.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://tpx.xuanzx.com

[E17] 首字母大写
来源：http://goq.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqu.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rbr.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yac.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://frf.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uln.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ptx.hesvh.cn

Ruby: s.capitalize
来源：http://tjw.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vbr.jqgufenzy.top

[E18] 模板占位符替换
来源：http://axx.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sei.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpr.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pxt.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://blq.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ayp.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pwv.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://edk.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ygp.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://ixe.cashguo.top

Py:   s.splitlines()
来源：http://bpt.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbd.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://thk.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://vzx.xinyue.icu

Java: s.lines().toList()
来源：http://ihb.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://ads.hcnkem.com

Ruby: s.lines
来源：http://wsm.yonumen.top

C#:   s.Split('\n')
来源：http://wri.tanke756.top

[E20] 判断字符串是否为空
来源：http://qjx.ybcxt.top

Py:   if not s:
来源：http://lrd.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xdk.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ibe.fengsongda.top

TS:   if (s === "") {}
来源：http://nfs.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://vtg.sweek.top

Go:   if s == "" {}
来源：http://qsh.xziqi.cn

Ruby: if s.empty?
来源：http://ccz.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ryw.smart0.xyz

[E21] 超长截断加省略号
来源：http://pjf.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pcv.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wcy.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lca.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tly.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ray.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://djm.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qnd.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vpn.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://bds.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ltv.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lpu.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eqt.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ave.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://znf.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eqc.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://igz.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ygh.bjfxy.top

================================================================================
来源：http://ptq.birdmap.top

F. 文件与目录
来源：http://vmo.gzhubu.top

================================================================================
来源：http://xui.gotoacloud.top

[F01] 读取整个文件
来源：http://olf.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fqq.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://owk.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gje.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lmc.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://plb.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mil.yonumen.top

Ruby: File.read("a.txt")
来源：http://wfc.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://hkk.gaohongyu789.top

[F02] 逐行读取文件
来源：http://xzn.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cce.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tfn.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfz.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zwc.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqz.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://veh.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocg.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gks.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://ngb.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xkh.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://elj.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gir.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imx.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yua.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cee.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://odb.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lah.gzhubu.top

[F04] 追加写入文件
来源：http://jpv.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sva.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dul.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzo.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olg.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xag.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ulk.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://puh.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rji.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://hap.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://klk.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://spn.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://jch.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://ohn.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://woy.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vzc.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://orr.tanke756.top

C#:   File.Exists("a.txt")
来源：http://vfa.zhengqikj.top

[F06] 删除文件
来源：http://omr.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://elk.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://tfd.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lok.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://nnm.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xzc.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://ysu.hysaishi.cn

Ruby: File.delete("a.txt")
来源：http://igp.uphjek.com

C#:   File.Delete("a.txt");
来源：http://kzh.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://pzy.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ncl.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iae.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oif.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwd.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gnc.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jnz.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vox.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xfm.zdbjq.cn

[F08] 遍历目录
来源：http://fia.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nth.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ymd.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://rky.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://rtq.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mpd.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uzc.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://ekf.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://jkx.0kj1m.cn

[F09] 获取文件大小
来源：http://mbn.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://rgj.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://tdx.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://cqw.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://ahk.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bja.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kca.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://fyk.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://igd.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://wwj.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://glo.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uri.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nil.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://naw.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lch.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ffg.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iip.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://voy.zdbjq.cn

[F11] 复制与移动文件
来源：http://ffk.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lwu.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yiq.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fkb.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtk.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncr.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yyg.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbs.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lcp.zhengqikj.top

[F12] CSV 读写
来源：http://ugp.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yut.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://plk.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wkh.chenlongwang.top

TS:   // 同上
来源：http://sau.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ysx.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://swe.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjn.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://anh.sjlbkw.cn

================================================================================
来源：http://xsp.ywan-chungtsiang.top

G. 面向对象
来源：http://yph.yongpay.top

================================================================================
来源：http://hwo.epnwcf.com

[G01] 定义类
来源：http://vvs.hnqzz.top

Py:   class User: pass
来源：http://rdg.tarul.cn

PHP:  class User {}
来源：http://wav.pycfn.com

JS:   class User {}
来源：http://drb.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://cwk.jyoumei.cn

Java: class User {}
来源：http://jcz.mhx1999.top

Go:   type User struct { Name string }
来源：http://bun.gotoacloud.top

Ruby: class User; end
来源：http://ocm.yuanzhike.top

C#:   class User {}
来源：http://bwf.birdmap.top

[G02] 构造函数
来源：http://gil.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://jks.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://zrq.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://tag.cheryme.top

TS:   constructor(public name: string) {}
来源：http://tgn.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://yks.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nuf.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://hoe.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://ubo.dianchejie.cn

[G03] 实例属性
来源：http://lmu.shangyingyoupin.top

Py:   self.name = "x"
来源：http://brd.52xcode.cn

PHP:  public string $name = "x";
来源：http://phv.sjlbkw.cn

JS:   this.name = "x";
来源：http://ged.jqgufenzy.top

TS:   name: string = "x";
来源：http://chj.316326.xyz

Java: private String name;
来源：http://zfa.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vcn.jiagoushi.top

Ruby: @name = "x"
来源：http://smj.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://jae.jinghuilouyu.cn

[G04] 定义方法
来源：http://rbb.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://mlk.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vdb.zycfv.cn

JS:   greet() { return this.name; }
来源：http://ndl.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://hmm.yanxiufei.cn

Java: String greet() { return name; }
来源：http://nbw.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jro.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://lyl.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://shf.tanke756.top

[G05] 继承
来源：http://brq.tianlin.xyz

Py:   class Admin(User): pass
来源：http://etg.daxiang520.top

PHP:  class Admin extends User {}
来源：http://cxk.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://fyn.ydzc1.top

TS:   class Admin extends User {}
来源：http://zeq.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://yev.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wom.fktsv.cn

Ruby: class Admin < User; end
来源：http://wlf.cucudq.cn

C#:   class Admin : User {}
来源：http://ost.cqqwz.cn

[G06] 重写方法
来源：http://abo.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://ngb.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hmc.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://eis.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://non.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://lcb.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tqg.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://mgb.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://ytk.jiagoushi.top

[G07] 调用父类方法
来源：http://hnq.ydzc1.top

Py:   super().greet()
来源：http://kuv.hcnkem.com

PHP:  parent::greet();
来源：http://cpf.zdbjq.cn

JS:   super.greet();
来源：http://okq.cdnleiting.top

TS:   super.greet();
来源：http://hbk.xuanzx.com

Java: super.greet();
来源：http://avd.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qxx.aibaodan.cn

Ruby: super
来源：http://eyo.shanyushiyangtech.top

C#:   base.Greet();
来源：http://ubx.jqgfzy.top

[G08] 静态方法与属性
来源：http://bmd.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ygo.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://nrs.cdnleiting.top

JS:   static f() {}
来源：http://lyf.svipenyu.cn

TS:   static f(): void {}
来源：http://mda.zhoulong.xyz

Java: static void f() {}
来源：http://pqa.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ods.snrcjt.cn

Ruby: def self.f; end
来源：http://nkt.aizwys.cn

C#:   public static void F() {}
来源：http://cxi.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://qxc.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://phe.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://jbv.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://viq.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://rcv.cashguo.top

Java: interface Shape { double area(); }
来源：http://ylu.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://mrd.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gmr.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://vok.sjlbkw.cn

[G10] 访问控制
来源：http://hea.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://eta.ydjk.org.cn

PHP:  public / protected / private
来源：http://lri.shuidangran.top

JS:   #private 字段；其余公开
来源：http://jue.epnwcf.com


<!-- 参考信息 -->