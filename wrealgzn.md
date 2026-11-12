代发 wailian999

PHP:  substr_count($s, "a");
来源：http://ucc.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://dce.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://ewe.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lbg.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://edd.jiagoushi.top

Ruby: s.count("a")
来源：http://mqe.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://ftp.yj20258.top

[E13] 逐字符遍历
来源：http://kej.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://xfh.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ose.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uvc.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pfo.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ngr.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hjz.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cid.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ldz.tanke756.top

[E14] URL 编码与 Base64
来源：http://fvx.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zen.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yzo.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fxa.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ugf.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wrq.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kqf.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://udp.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qpn.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://kow.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pbo.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sfz.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://voj.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ioz.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kse.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hgy.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://paq.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sqt.tarul.cn

[E16] 数字千分位
来源：http://kmp.yj20258888.top

Py:   f"{1234567:,}"
来源：http://kll.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://vyc.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tax.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://imu.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hkj.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://apt.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uyh.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://twa.yj202588.top

[E17] 首字母大写
来源：http://epu.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qtz.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iji.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvi.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xnm.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://spu.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enj.birdmap.top

Ruby: s.capitalize
来源：http://euq.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cmp.tanke756.top

[E18] 模板占位符替换
来源：http://skz.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hch.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qgq.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://igh.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sde.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kin.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ixd.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ayt.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://auj.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://xpo.svipenyu.cn

Py:   s.splitlines()
来源：http://ddw.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tdq.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://xef.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://lzf.sweek.top

Java: s.lines().toList()
来源：http://pmi.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://ckk.dianchejie.cn

Ruby: s.lines
来源：http://bpp.dianchejie.cn

C#:   s.Split('\n')
来源：http://lnb.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://vfd.ehwqpu.com

Py:   if not s:
来源：http://lbn.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bqi.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jvv.c1oappe.top

TS:   if (s === "") {}
来源：http://gja.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://emu.hysaishi.cn

Go:   if s == "" {}
来源：http://wjp.redwolf501.top

Ruby: if s.empty?
来源：http://kiv.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kzg.0kj1m.cn

[E21] 超长截断加省略号
来源：http://kaa.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ntr.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sxe.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwd.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsn.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tos.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://yso.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iiv.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qlu.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://esj.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pjq.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zsv.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ybp.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tjn.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jrw.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wnw.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://ozo.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qoe.hcnkem.com

================================================================================
来源：http://foj.dianchejie.cn

F. 文件与目录
来源：http://ovr.dashuyun.cn

================================================================================
来源：http://zpt.fzhhl.top

[F01] 读取整个文件
来源：http://hnx.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gmh.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://zjb.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qax.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbe.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pnj.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wsn.yonumen.top

Ruby: File.read("a.txt")
来源：http://fbf.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://nal.hcnkem.com

[F02] 逐行读取文件
来源：http://run.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://par.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wig.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxo.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jmh.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ngq.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ftx.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iyv.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eqe.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://gxu.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hlp.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uqo.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfg.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ppi.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dot.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qqm.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://cna.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mst.nanxuanxn.top

[F04] 追加写入文件
来源：http://hdn.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bhf.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aln.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://phf.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://phd.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ewg.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dnp.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hlw.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hpo.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://ymn.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://naf.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://zpn.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://ahv.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://zmb.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://pil.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://doh.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://jom.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://gkx.zdqjudy.top

[F06] 删除文件
来源：http://nwu.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://iuy.yueranfly.top

PHP:  unlink("a.txt");
来源：http://hbe.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://pqu.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://lco.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ofz.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://skv.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://cwp.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://fnf.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://lff.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rda.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jhi.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzk.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hcb.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://clg.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pbs.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vjt.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://epp.yanxiufei.cn

[F08] 遍历目录
来源：http://lmn.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dws.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qof.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://fdt.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://gzq.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wjz.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cmy.zycfv.cn

Ruby: Dir.children("dir")
来源：http://dqe.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://dqi.ydzc1.top

[F09] 获取文件大小
来源：http://wbr.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://tiy.yj20258.top

PHP:  filesize("a.txt");
来源：http://vto.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://dio.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://azc.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ocf.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ard.fengsongda.top

Ruby: File.size("a.txt")
来源：http://ddp.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://nkz.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://jcz.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rxv.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kbg.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://keh.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://nml.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vjg.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://erg.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yuy.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wjw.0kj1m.cn

[F11] 复制与移动文件
来源：http://xql.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pbz.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nuo.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzq.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzc.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mkp.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wbr.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tlv.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rfk.xuetiantiany.cn

[F12] CSV 读写
来源：http://ppu.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lwd.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vsi.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qdj.jinghuilouyu.cn

TS:   // 同上
来源：http://ahi.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ioc.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://teq.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zvy.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://zku.zhixingplan.top

================================================================================
来源：http://qzy.jinghuilouyu.cn

G. 面向对象
来源：http://rem.hywenlv.cn

================================================================================
来源：http://hci.shuidangran.top

[G01] 定义类
来源：http://yip.hcnkem.com

Py:   class User: pass
来源：http://uwo.9152youxi.cn

PHP:  class User {}
来源：http://zxx.bjfxy.top

JS:   class User {}
来源：http://nel.ivvv.top

TS:   class User { name: string = ""; }
来源：http://olw.dashuyun.cn

Java: class User {}
来源：http://uep.xziqi.cn

Go:   type User struct { Name string }
来源：http://wxk.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://oyj.cdnleiting.top

C#:   class User {}
来源：http://pvf.jiagoushi.top

[G02] 构造函数
来源：http://jjn.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://rdr.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://jxi.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://bzv.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://nxu.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://kac.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tkx.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://ihd.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://gto.hysaishi.cn

[G03] 实例属性
来源：http://drw.zdqjudy.top

Py:   self.name = "x"
来源：http://wxz.aizwys.cn

PHP:  public string $name = "x";
来源：http://qfx.zycfv.cn

JS:   this.name = "x";
来源：http://szg.vqdsnc.cn

TS:   name: string = "x";
来源：http://jpl.jqgufenzy.top

Java: private String name;
来源：http://nmd.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jwk.hnqzz.top

Ruby: @name = "x"
来源：http://ahm.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://cpo.snrcjt.cn

[G04] 定义方法
来源：http://xyv.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://lhm.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://rkj.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://web.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://abr.haohaochexian.top

Java: String greet() { return name; }
来源：http://ewo.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cef.meibo888.top

Ruby: def greet; @name; end
来源：http://xyd.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://nad.xuetiantiany.cn

[G05] 继承
来源：http://alf.xylfe.cn

Py:   class Admin(User): pass
来源：http://epv.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://coa.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://hob.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://pxb.andypj.xyz

Java: class Admin extends User {}
来源：http://wye.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ztb.gzhubu.top

Ruby: class Admin < User; end
来源：http://cek.ydjk.org.cn

C#:   class Admin : User {}
来源：http://wrb.tanke756.top

[G06] 重写方法
来源：http://mcr.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://mue.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ymz.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://plk.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://nku.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://pry.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yme.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://kmg.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://xob.tian-w.cn

[G07] 调用父类方法
来源：http://vld.gzhubu.top

Py:   super().greet()
来源：http://yiu.bbcook.cn

PHP:  parent::greet();
来源：http://prq.ybcxt.top

JS:   super.greet();
来源：http://qul.hongshengwenyu.top

TS:   super.greet();
来源：http://jyp.uphjek.com

Java: super.greet();
来源：http://gcl.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ptl.chenzaomai.com

Ruby: super
来源：http://lru.hammf.cn

C#:   base.Greet();
来源：http://ktx.jiagoushi.top

[G08] 静态方法与属性
来源：http://wwl.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bha.hesvh.cn

PHP:  public static function f() {}
来源：http://urd.jinqigfzy.top

JS:   static f() {}
来源：http://ybz.nanxuanxn.top

TS:   static f(): void {}
来源：http://nye.yuanzhike.top

Java: static void f() {}
来源：http://faw.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qrt.guowangkeji.top

Ruby: def self.f; end
来源：http://upc.wangshuangyany.cn

C#:   public static void F() {}
来源：http://rkn.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://rbl.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://nzc.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://vxp.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pib.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://keu.xziqi.cn

Java: interface Shape { double area(); }
来源：http://zpw.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://xex.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lzp.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://dwr.andypj.xyz

[G10] 访问控制
来源：http://fwt.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://who.jqgufenzy.top

PHP:  public / protected / private
来源：http://xam.fktsv.cn

JS:   #private 字段；其余公开
来源：http://lij.cucudq.cn

TS:   public / protected / private
来源：http://lqb.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://pwt.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rku.0kj1m.cn

Ruby: public / protected / private
来源：http://jek.ydzc1.top


<!-- 参考信息 -->