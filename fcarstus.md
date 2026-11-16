代发 wailian999

Py:   for ch in s: print(ch)
来源：http://uqd.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gvl.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwq.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://njm.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kjd.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://poy.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ptl.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ite.vehdjk.com

[E14] URL 编码与 Base64
来源：http://oln.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qaf.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zfj.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lfn.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qeg.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qku.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://spg.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kii.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uob.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://apn.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://edc.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zbj.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zla.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dtg.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://faj.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxp.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yol.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dum.aizwys.cn

[E16] 数字千分位
来源：http://nse.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://dyo.birdmap.top

PHP:  number_format(1234567);
来源：http://pzw.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://skp.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qvk.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lst.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://khd.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfo.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://fut.xuanzx.com

[E17] 首字母大写
来源：http://hbi.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uiz.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hdo.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://anw.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wan.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://diq.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ret.ppjwa.cn

Ruby: s.capitalize
来源：http://xie.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nbp.jinqigufen.top

[E18] 模板占位符替换
来源：http://dbt.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ytl.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pnb.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xvm.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hoz.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nkc.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fgm.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wxp.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hno.c1oappe.top

[E19] 多行文本按行拆分
来源：http://cws.jinqigufen.top

Py:   s.splitlines()
来源：http://ozt.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qbt.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://chm.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://gnh.aibaodan.cn

Java: s.lines().toList()
来源：http://iwp.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://vfy.jyoumei.cn

Ruby: s.lines
来源：http://vaj.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://rgp.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://wzd.jinyuanbaomall.cn

Py:   if not s:
来源：http://hdp.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cmm.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hge.zdqjudy.top

TS:   if (s === "") {}
来源：http://emd.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://qkb.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://vyp.feifeiyinyue.top

Ruby: if s.empty?
来源：http://wam.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tdy.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://xpm.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sgb.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nbd.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vzn.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://svw.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ugp.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://lvf.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lub.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mmh.guannengcc.top

[E22] 字节长度与字符长度
来源：http://ljq.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aip.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://usq.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://apm.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jzm.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fwm.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kcu.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://grn.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zbl.meibo888.top

================================================================================
来源：http://nqi.316326.xyz

F. 文件与目录
来源：http://vva.ehwqpu.com

================================================================================
来源：http://tyy.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://bga.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gcx.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://cym.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ezd.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yki.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cet.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mip.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://bqz.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://vka.tian-w.cn

[F02] 逐行读取文件
来源：http://wnb.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://faf.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbo.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grl.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wse.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wat.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kfj.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dmv.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://try.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://hrg.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ueu.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjo.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azg.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvq.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hjb.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zqf.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://dxf.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fnw.hcnkem.com

[F04] 追加写入文件
来源：http://jsl.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ova.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kpb.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krw.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olm.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kbo.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xda.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tfx.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qbj.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://owa.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://edt.meibo888.top

PHP:  file_exists("a.txt");
来源：http://rfj.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://ecn.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://ruy.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qan.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fzd.sweek.top

Ruby: File.exist?("a.txt")
来源：http://ion.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://eow.52xcode.cn

[F06] 删除文件
来源：http://yzv.tarul.cn

Py:   os.remove("a.txt")
来源：http://wkh.yueranfly.top

PHP:  unlink("a.txt");
来源：http://kjz.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://hry.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://wce.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uyc.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://avh.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://aaq.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://ncn.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://xhj.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aqm.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ojp.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbo.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xlg.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uxn.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfm.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ztg.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ojj.zhixingplan.top

[F08] 遍历目录
来源：http://irf.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ifb.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zgs.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://upq.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://twq.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://woc.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dpj.316326.xyz

Ruby: Dir.children("dir")
来源：http://jwu.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://uhx.zhongyouzk.top

[F09] 获取文件大小
来源：http://nio.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://jev.jianghu66.top

PHP:  filesize("a.txt");
来源：http://rxi.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://jmm.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://rcs.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://udp.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eqm.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://vxa.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://xyv.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://far.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cfv.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://igo.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xzm.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://rce.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vgb.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hii.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uaz.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zky.jyoumei.cn

[F11] 复制与移动文件
来源：http://ryw.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ced.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqv.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kuq.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ddg.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdz.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hux.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://swe.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wht.shuidangran.top

[F12] CSV 读写
来源：http://tbs.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://egl.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wvd.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://znc.yongpay.top

TS:   // 同上
来源：http://ilz.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fby.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uvc.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yfe.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wii.xziqi.cn

================================================================================
来源：http://gzq.feifeiyinyue.top

G. 面向对象
来源：http://ksj.guannengcc.top

================================================================================
来源：http://wjr.hnqzz.top

[G01] 定义类
来源：http://ykx.zhengqikj.top

Py:   class User: pass
来源：http://omv.zdbjq.cn

PHP:  class User {}
来源：http://gjz.gogol.net.cn

JS:   class User {}
来源：http://kuj.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://ybs.jinghuilouyu.cn

Java: class User {}
来源：http://onx.mhx1999.top

Go:   type User struct { Name string }
来源：http://uyw.svipenyu.cn

Ruby: class User; end
来源：http://hne.zhijiandao.cn

C#:   class User {}
来源：http://ptd.chenzaomai.com

[G02] 构造函数
来源：http://mxi.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ozq.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://drv.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://uig.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://mhc.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://isx.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wqv.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://zrn.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://opt.jinqigfzy.top

[G03] 实例属性
来源：http://rin.yfazqb.com

Py:   self.name = "x"
来源：http://pml.uphjek.com

PHP:  public string $name = "x";
来源：http://svu.uphjek.com

JS:   this.name = "x";
来源：http://xdm.epnwcf.com

TS:   name: string = "x";
来源：http://ngg.nanxuanxn.top

Java: private String name;
来源：http://bnr.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kja.zhixingplan.top

Ruby: @name = "x"
来源：http://cwb.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://pqa.fanxiaobao.xyz

[G04] 定义方法
来源：http://ejt.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://ggm.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://slx.fktsv.cn

JS:   greet() { return this.name; }
来源：http://cem.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://zik.sysykeji.top

Java: String greet() { return name; }
来源：http://bvc.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://chq.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://fpv.ydzc1.top

C#:   public string Greet() => Name;
来源：http://jrn.cdnleiting.top

[G05] 继承
来源：http://cgf.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://dzs.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://cvv.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://mwr.yfazqb.com

TS:   class Admin extends User {}
来源：http://tob.haohaochexian.top

Java: class Admin extends User {}
来源：http://can.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xzy.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://gxa.gotoacloud.top

C#:   class Admin : User {}
来源：http://bbt.bjfxy.top

[G06] 重写方法
来源：http://wke.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://osm.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ohq.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://miv.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://tzz.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://tgj.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bcv.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://akw.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://ygv.jlsjyb.cn

[G07] 调用父类方法
来源：http://xtg.jinqigfzy.top

Py:   super().greet()
来源：http://lgx.fehbvm.com

PHP:  parent::greet();
来源：http://rmc.zdbjq.cn

JS:   super.greet();
来源：http://whx.xylfe.cn

TS:   super.greet();
来源：http://ajd.havefunace.top

Java: super.greet();
来源：http://vso.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ute.316326.xyz

Ruby: super
来源：http://rrt.nwbrower.top

C#:   base.Greet();
来源：http://owj.havefunace.top

[G08] 静态方法与属性
来源：http://agb.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wih.bjfxy.top

PHP:  public static function f() {}
来源：http://ewv.yj202588.top

JS:   static f() {}
来源：http://hne.chenjidiqi.icu

TS:   static f(): void {}
来源：http://nph.nanxinkj.top

Java: static void f() {}
来源：http://lvm.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eyw.sxryk.cn

Ruby: def self.f; end
来源：http://rfh.jianghu66.top

C#:   public static void F() {}
来源：http://cpm.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://qgj.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://inm.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://nkq.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ytl.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://nfo.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://jjv.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://ggo.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gsa.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://exh.jianghu66.top

[G10] 访问控制
来源：http://jcm.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://hes.yueranfly.top

PHP:  public / protected / private
来源：http://kpo.fehbvm.com

JS:   #private 字段；其余公开
来源：http://qee.vehdjk.com

TS:   public / protected / private
来源：http://tub.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://qra.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://onq.tian-w.cn

Ruby: public / protected / private
来源：http://hvn.fzhhl.top

C#:   public / protected / private / internal
来源：http://nll.hcnkem.com

[G11] getter / setter
来源：http://plh.yfazqb.com

Py:   @property 与 @x.setter
来源：http://swt.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yae.316326.xyz

JS:   get name() { return this._name; }
来源：http://agk.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://klj.xylfe.cn

Java: public String getName() { return name; }
来源：http://hzn.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewg.xinyue.icu


<!-- 参考信息 -->