代发 wailian999

PHP:  substr_count($s, "a");
来源：http://pkp.52xcode.cn

JS:   s.split("a").length - 1
来源：http://mmq.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://gtu.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ril.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://kgi.uphjek.com

Ruby: s.count("a")
来源：http://wfw.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://fbj.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://xmr.ivvv.top

Py:   for ch in s: print(ch)
来源：http://ned.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgn.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tar.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ijz.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wmv.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://avm.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kco.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://prt.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://hgz.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gds.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fsr.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nuc.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://brr.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsy.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ags.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fvs.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fms.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://gll.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qgh.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uou.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bhd.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://npx.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yhf.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uat.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jbo.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xdz.yuxming.cn

[E16] 数字千分位
来源：http://uta.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://evg.gzhubu.top

PHP:  number_format(1234567);
来源：http://jaz.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vtr.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ymg.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ftp.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://exf.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qnr.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://qcm.kuanghao11.cn

[E17] 首字母大写
来源：http://bsg.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xgx.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://omj.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hem.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://whv.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fji.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jwt.yanxiufei.cn

Ruby: s.capitalize
来源：http://oiy.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://efh.fengsongda.top

[E18] 模板占位符替换
来源：http://fxk.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lbf.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://igo.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qrx.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qtc.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://txq.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wzo.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ftt.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://epo.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://pqj.zhongyouzk.top

Py:   s.splitlines()
来源：http://udo.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bhc.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://iyo.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://ice.epnwcf.com

Java: s.lines().toList()
来源：http://dja.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://dtm.0kj1m.cn

Ruby: s.lines
来源：http://egs.wangdashe.top

C#:   s.Split('\n')
来源：http://ozh.sxryk.cn

[E20] 判断字符串是否为空
来源：http://quc.chenzaomai.com

Py:   if not s:
来源：http://yle.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lcu.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zyo.chenzaomai.com

TS:   if (s === "") {}
来源：http://iom.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://zft.snrcjt.cn

Go:   if s == "" {}
来源：http://skv.ehwqpu.com

Ruby: if s.empty?
来源：http://koz.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wdu.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://jpj.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jkh.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ovc.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qte.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lkn.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fhn.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://oyv.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fik.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ziz.52xcode.cn

[E22] 字节长度与字符长度
来源：http://cnr.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dya.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjo.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxh.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhd.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqg.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zqo.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://xlf.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gyh.svipenyu.cn

================================================================================
来源：http://ckb.zdbjq.cn

F. 文件与目录
来源：http://jfb.zhiwuduotai.top

================================================================================
来源：http://ure.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://fyr.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mmb.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://faz.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dfe.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iuh.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zdz.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hwy.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://dpw.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://hfv.snrcjt.cn

[F02] 逐行读取文件
来源：http://ghx.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qcw.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lmz.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://plo.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://knz.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvd.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jct.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hzk.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uud.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://dee.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hbs.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vln.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpa.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxw.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zns.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uyt.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://pre.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rrm.aibaodan.cn

[F04] 追加写入文件
来源：http://ger.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pub.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gkm.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vng.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tci.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gms.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xav.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nyg.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hpn.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://uip.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jhc.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://itv.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://eoz.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://ggn.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nrv.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eea.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://tbb.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://ktg.yuanzhike.top

[F06] 删除文件
来源：http://sat.mhx1999.top

Py:   os.remove("a.txt")
来源：http://cpz.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://imj.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://vfk.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dnj.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wcl.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://rpm.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://tyr.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://cdc.hesvh.cn

[F07] 创建目录（含多级）
来源：http://xid.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ybi.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://boq.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stq.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://acy.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gur.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://isx.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://chr.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lsz.kuanghao11.cn

[F08] 遍历目录
来源：http://zeo.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ksr.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ide.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://tet.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://zgy.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rvp.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fnl.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://wbd.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://sjd.sxryk.cn

[F09] 获取文件大小
来源：http://aqm.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://kfc.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://djs.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://dpr.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://hve.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://uhe.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sge.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://feh.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://adz.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://ldl.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://khv.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tnr.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eim.mhx1999.top

TS:   path.extname("a.txt")
来源：http://umf.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pcb.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fnh.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ova.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ubv.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://fut.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aks.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://did.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zpe.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://afi.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aom.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://byv.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wra.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rfk.xuetiantiany.cn

[F12] CSV 读写
来源：http://clb.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jjm.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cap.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bpg.yueranfly.top

TS:   // 同上
来源：http://svu.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vtm.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wvn.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bpc.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ttm.jinyuanbaomall.cn

================================================================================
来源：http://yvs.pycfn.com

G. 面向对象
来源：http://hlx.snrcjt.cn

================================================================================
来源：http://lvp.dianchejie.cn

[G01] 定义类
来源：http://cpv.vehdjk.com

Py:   class User: pass
来源：http://ahi.yanxiufei.cn

PHP:  class User {}
来源：http://idm.yvedp.cn

JS:   class User {}
来源：http://jxp.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://cty.xuanzx.com

Java: class User {}
来源：http://djo.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://gmq.0kj1m.cn

Ruby: class User; end
来源：http://cdm.ehwqpu.com

C#:   class User {}
来源：http://ehg.sjlbkw.cn

[G02] 构造函数
来源：http://fna.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://qkd.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://ybw.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://bgl.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://cqe.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://wqq.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sup.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://ygn.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://oos.ydjk.org.cn

[G03] 实例属性
来源：http://wta.pycfn.com

Py:   self.name = "x"
来源：http://iar.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://ltb.zhijiandao.cn

JS:   this.name = "x";
来源：http://lwd.yanxiufei.cn

TS:   name: string = "x";
来源：http://mhd.sufxvd.cn

Java: private String name;
来源：http://hvq.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kvl.hysaishi.cn

Ruby: @name = "x"
来源：http://slx.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://jfn.svipenyu.cn

[G04] 定义方法
来源：http://yww.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://fnl.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mco.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://vlm.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://frc.zhengqikj.top

Java: String greet() { return name; }
来源：http://dns.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://duz.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://ezt.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://hcl.daria6918.cn

[G05] 继承
来源：http://nkp.zhixingplan.top

Py:   class Admin(User): pass
来源：http://zdx.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://iww.tian-w.cn

JS:   class Admin extends User {}
来源：http://owa.jyoumei.cn

TS:   class Admin extends User {}
来源：http://wop.jqgufenzy.top

Java: class Admin extends User {}
来源：http://bql.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxz.jiagoushi.top

Ruby: class Admin < User; end
来源：http://mwi.nanxinkj.top

C#:   class Admin : User {}
来源：http://xhe.zhoulong.xyz

[G06] 重写方法
来源：http://age.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://sro.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gjd.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://abn.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://dur.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://hwp.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yup.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://xcm.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://gfc.jinqigfzy.top

[G07] 调用父类方法
来源：http://whv.zycfv.cn

Py:   super().greet()
来源：http://dst.cucudq.cn

PHP:  parent::greet();
来源：http://doa.pengpengdd.cyou

JS:   super.greet();
来源：http://uec.feifeiyinyue.top

TS:   super.greet();
来源：http://nfg.meibo888.top

Java: super.greet();
来源：http://afc.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qvi.kuanghao11.cn

Ruby: super
来源：http://xqr.mhx1999.top

C#:   base.Greet();
来源：http://pgr.zhengqikj.top

[G08] 静态方法与属性
来源：http://jeo.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vin.fzhhl.top

PHP:  public static function f() {}
来源：http://auc.tianlin.xyz

JS:   static f() {}
来源：http://rno.cqqwz.cn

TS:   static f(): void {}
来源：http://gzu.kuanghao11.cn

Java: static void f() {}
来源：http://tlb.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lfh.quarkkingdee.top

Ruby: def self.f; end
来源：http://tyb.hysaishi.cn

C#:   public static void F() {}
来源：http://fvn.havefunace.top

[G09] 接口 / 抽象类
来源：http://lll.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://rlo.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://jbo.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uua.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://hyu.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://lsv.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://csa.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kbd.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://dyq.zycfv.cn

[G10] 访问控制
来源：http://soa.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://bzr.xuanzx.com

PHP:  public / protected / private
来源：http://wdz.uphjek.com

JS:   #private 字段；其余公开
来源：http://ndp.nanxinkj.top

TS:   public / protected / private
来源：http://wwb.yongpay.top

Java: public / protected / private / 默认包级
来源：http://tgb.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pps.yj20258888.top

Ruby: public / protected / private
来源：http://ebd.svipenyu.cn


<!-- 参考信息 -->