代发 wailian999

PHP:  substr_count($s, "a");
来源：http://gte.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://hez.316326.xyz

TS:   s.split("a").length - 1
来源：http://fcp.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://smb.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://jhh.yj20258.top

Ruby: s.count("a")
来源：http://alw.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://lfl.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://bxl.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://cer.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gpr.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ucf.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://ubj.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hyz.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ptz.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fpr.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tdm.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://ang.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ojl.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wnw.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hwd.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jhc.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eaa.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://frk.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kub.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hwj.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://biw.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aqb.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ubr.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rub.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yjj.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vud.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fhd.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjl.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rou.yuxming.cn

[E16] 数字千分位
来源：http://wqa.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://rxb.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://ama.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gig.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xsl.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vvx.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ewc.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rqj.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://wiz.zdbjq.cn

[E17] 首字母大写
来源：http://sja.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oyv.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ups.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pty.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xtj.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mud.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llm.nanxuanxn.top

Ruby: s.capitalize
来源：http://gtx.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sxu.sysykeji.top

[E18] 模板占位符替换
来源：http://ppr.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cks.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tyz.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ipj.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jso.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vow.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lub.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lnu.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tsl.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://trr.xziqi.cn

Py:   s.splitlines()
来源：http://gbb.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qqg.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://egl.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://yhd.daxiang520.top

Java: s.lines().toList()
来源：http://ode.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://yax.hammf.cn

Ruby: s.lines
来源：http://hlk.sxryk.cn

C#:   s.Split('\n')
来源：http://saw.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://tiq.tarul.cn

Py:   if not s:
来源：http://bxn.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ern.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yzy.cashguo.top

TS:   if (s === "") {}
来源：http://pdx.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://ash.zdbjq.cn

Go:   if s == "" {}
来源：http://qzz.0kj1m.cn

Ruby: if s.empty?
来源：http://faz.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://apo.cheryme.top

[E21] 超长截断加省略号
来源：http://mcy.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xhr.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tlc.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://soh.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ljq.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iho.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://nob.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kox.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gkj.epnwcf.com

[E22] 字节长度与字符长度
来源：http://zln.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ryl.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iqa.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxq.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jth.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eqo.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ped.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://uos.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fhr.hcnkem.com

================================================================================
来源：http://umc.zhengqikj.top

F. 文件与目录
来源：http://xxv.xziqi.cn

================================================================================
来源：http://qvo.vehdjk.com

[F01] 读取整个文件
来源：http://iun.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpb.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://ops.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://csh.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://woh.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://usi.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nmt.hammf.cn

Ruby: File.read("a.txt")
来源：http://bdf.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ycj.hesvh.cn

[F02] 逐行读取文件
来源：http://hec.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://klx.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pnl.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avf.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agk.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kvm.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oef.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vlw.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbg.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://siy.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dak.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://djf.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzc.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfg.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ltv.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wcq.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://paf.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zsb.ydjk.org.cn

[F04] 追加写入文件
来源：http://udk.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dyq.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ont.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzn.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bnp.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rky.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rri.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jzu.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vgi.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://ynq.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pve.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://ija.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://yly.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://jwq.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jcc.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sqp.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://ohq.pycfn.com

C#:   File.Exists("a.txt")
来源：http://kmv.pycfn.com

[F06] 删除文件
来源：http://dmh.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://wcp.daria6918.cn

PHP:  unlink("a.txt");
来源：http://qej.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://egi.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://wcv.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://csl.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://emt.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://sxe.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://vjp.fehbvm.com

[F07] 创建目录（含多级）
来源：http://jgy.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ykd.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xqm.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tof.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enh.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kxt.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kwg.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xmt.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jdc.bjfxy.top

[F08] 遍历目录
来源：http://ipu.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gat.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pjz.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://yic.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://jmr.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rmc.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aqu.sxryk.cn

Ruby: Dir.children("dir")
来源：http://rfs.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://nku.kuanghao11.cn

[F09] 获取文件大小
来源：http://vem.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://vlo.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://gwm.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://ilk.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://dou.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://uki.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vwv.hesvh.cn

Ruby: File.size("a.txt")
来源：http://jhw.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://bhg.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://ryv.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xfm.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgg.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gde.tian-w.cn

TS:   path.extname("a.txt")
来源：http://rcv.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qlu.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rqu.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fvg.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://drl.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://cyf.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vps.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ata.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gym.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcz.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixz.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tup.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wya.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xhk.nwbrower.top

[F12] CSV 读写
来源：http://kck.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dse.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rem.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://upn.chenlongwang.top

TS:   // 同上
来源：http://kia.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sco.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qgw.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sha.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pcu.bbcook.cn

================================================================================
来源：http://cur.nanxinkj.top

G. 面向对象
来源：http://cog.hammf.cn

================================================================================
来源：http://mkq.haohaochexian.top

[G01] 定义类
来源：http://asb.yueranfly.top

Py:   class User: pass
来源：http://cti.jyoumei.cn

PHP:  class User {}
来源：http://djq.hesvh.cn

JS:   class User {}
来源：http://ost.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://lho.cdnleiting.top

Java: class User {}
来源：http://bpr.hfpthk.cn

Go:   type User struct { Name string }
来源：http://kqe.zhongyouzk.top

Ruby: class User; end
来源：http://mlp.shangyingyoupin.top

C#:   class User {}
来源：http://cvs.hcnkem.com

[G02] 构造函数
来源：http://iif.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://uuv.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://bsy.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://ugh.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://iff.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://usz.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gqd.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://gui.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://diw.gotoacloud.top

[G03] 实例属性
来源：http://kft.hfpthk.cn

Py:   self.name = "x"
来源：http://qib.jianghu66.top

PHP:  public string $name = "x";
来源：http://lkb.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://tkk.cashguo.top

TS:   name: string = "x";
来源：http://nex.daxiang520.top

Java: private String name;
来源：http://vnx.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uvi.shuidangran.top

Ruby: @name = "x"
来源：http://lih.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://tzh.cdnleiting.top

[G04] 定义方法
来源：http://rum.ydzc1.top

Py:   def greet(self): return self.name
来源：http://ueo.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gfb.sxryk.cn

JS:   greet() { return this.name; }
来源：http://ocv.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://xpe.svipenyu.cn

Java: String greet() { return name; }
来源：http://fuj.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ixg.hywenlv.cn

Ruby: def greet; @name; end
来源：http://aqw.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://xdn.yonumen.top

[G05] 继承
来源：http://yev.guowangkeji.top

Py:   class Admin(User): pass
来源：http://gpw.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://daz.fktsv.cn

JS:   class Admin extends User {}
来源：http://iot.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://jli.daria6918.cn

Java: class Admin extends User {}
来源：http://pjb.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://chw.hammf.cn

Ruby: class Admin < User; end
来源：http://wmd.svipenyu.cn

C#:   class Admin : User {}
来源：http://vqe.jiagoushi.top

[G06] 重写方法
来源：http://nqj.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://xtl.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zju.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://swj.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://djc.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://fkl.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hbx.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://nhb.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://uoo.52xcode.cn

[G07] 调用父类方法
来源：http://fqw.zdbjq.cn

Py:   super().greet()
来源：http://ear.jiagoushi.top

PHP:  parent::greet();
来源：http://sdi.wangdashe.top

JS:   super.greet();
来源：http://zsl.9152youxi.cn

TS:   super.greet();
来源：http://ehj.yonumen.top

Java: super.greet();
来源：http://lvx.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ypd.gaohongyu789.top

Ruby: super
来源：http://rel.ydjk.org.cn

C#:   base.Greet();
来源：http://dgk.yuanzhike.top

[G08] 静态方法与属性
来源：http://krs.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lrs.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://oeo.xinyue.icu

JS:   static f() {}
来源：http://sjf.shangyingyoupin.top

TS:   static f(): void {}
来源：http://wxd.zycfv.cn

Java: static void f() {}
来源：http://kuj.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iwq.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://wqu.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://slo.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://pfy.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://rpt.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jdb.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://rrn.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://pbj.hnqzz.top

Java: interface Shape { double area(); }
来源：http://rnc.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://sef.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ssf.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://htq.hysaishi.cn

[G10] 访问控制
来源：http://pwy.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://moe.sxryk.cn

PHP:  public / protected / private
来源：http://zvw.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://mdn.vqdsnc.cn

TS:   public / protected / private
来源：http://ryu.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://lit.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://noz.nwbrower.top

Ruby: public / protected / private
来源：http://qtr.jlsjyb.cn


<!-- 参考信息 -->