代发 wailian999

Go:   strings.Count(s, "a")
来源：http://lpk.jyoumei.cn

Ruby: s.count("a")
来源：http://szp.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://pdj.9152youxi.cn

[E13] 逐字符遍历
来源：http://ykh.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://efh.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dok.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lca.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qwl.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmy.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mnb.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nbm.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nnl.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://zxp.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://czs.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ihv.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://luy.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ahq.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rns.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vpo.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jit.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bjj.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://wft.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yej.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ghr.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ngv.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zub.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qbb.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qaw.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tzg.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://itk.fzhhl.top

[E16] 数字千分位
来源：http://oci.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://qgi.ybcxt.top

PHP:  number_format(1234567);
来源：http://vof.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://slj.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rwk.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://doz.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://izs.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jdp.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://ogl.9152youxi.cn

[E17] 首字母大写
来源：http://wqm.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gta.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zjy.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tkh.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltw.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vod.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://naa.meibo888.top

Ruby: s.capitalize
来源：http://ihm.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ymo.fzhhl.top

[E18] 模板占位符替换
来源：http://nne.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zfq.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://azm.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://whf.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hdl.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rby.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fka.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mvj.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wti.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://scz.zhoulong.xyz

Py:   s.splitlines()
来源：http://lyp.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://won.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://gap.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://etf.shzxlz.cn

Java: s.lines().toList()
来源：http://xbh.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://mhb.sysykeji.top

Ruby: s.lines
来源：http://ebi.hcnkem.com

C#:   s.Split('\n')
来源：http://coj.ydzc1.top

[E20] 判断字符串是否为空
来源：http://xlj.bjfxy.top

Py:   if not s:
来源：http://noo.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jyj.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wku.chenzaomai.com

TS:   if (s === "") {}
来源：http://dgy.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://sxa.zdqjudy.top

Go:   if s == "" {}
来源：http://lsb.zhengqikj.top

Ruby: if s.empty?
来源：http://oka.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jqp.mhx1999.top

[E21] 超长截断加省略号
来源：http://ums.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fsd.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oin.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owe.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkd.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://esg.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://gnq.chenzaomai.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ptt.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mmp.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://thw.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://urh.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mvo.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aor.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbe.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://igk.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nmw.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://xsu.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ucm.iojbl.cn

================================================================================
来源：http://fea.yueranfly.top

F. 文件与目录
来源：http://rwc.fanxiaobao.xyz

================================================================================
来源：http://xfm.nwbrower.top

[F01] 读取整个文件
来源：http://oey.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hwa.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://teg.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kcn.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bfr.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lwh.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfi.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://uyu.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://agn.tarul.cn

[F02] 逐行读取文件
来源：http://pdc.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pch.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rgo.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://clg.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohb.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nwu.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wvi.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://trk.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://skg.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://jlw.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hah.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hzq.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://krz.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gco.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dfs.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eps.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://agl.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pml.kuanghao11.cn

[F04] 追加写入文件
来源：http://scy.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nbs.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kcn.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cyp.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifc.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ofk.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gxi.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ayk.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://egx.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://tkg.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wdd.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://owr.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://ugq.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://hsa.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://seh.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qns.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://dwr.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://eab.bbcook.cn

[F06] 删除文件
来源：http://alb.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://wvo.sxryk.cn

PHP:  unlink("a.txt");
来源：http://ltz.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://zvu.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vmv.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nkg.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://yjs.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://you.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://mfp.mhx1999.top

[F07] 创建目录（含多级）
来源：http://xpx.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xip.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sxa.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enb.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esj.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zvc.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vlc.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nit.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jye.yfazqb.com

[F08] 遍历目录
来源：http://yrl.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jsp.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kub.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://evq.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://bvw.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rkl.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://idf.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://mnq.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://ida.sxryk.cn

[F09] 获取文件大小
来源：http://ala.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://del.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://mpj.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://ohb.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://tyz.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iyb.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cog.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://eli.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://rwv.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ydw.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yzh.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cnj.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://udi.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://dqi.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upt.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mrl.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qqu.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pci.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://wxf.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://syo.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bzd.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xov.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uyb.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ayc.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xmf.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bto.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cjy.sysykeji.top

[F12] CSV 读写
来源：http://atf.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lgd.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pci.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://imi.pycfn.com

TS:   // 同上
来源：http://dbi.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wkd.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hgd.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kmj.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ere.nanxuanxn.top

================================================================================
来源：http://mye.jlsjyb.cn

G. 面向对象
来源：http://kyi.ivvv.top

================================================================================
来源：http://tkj.andypj.xyz

[G01] 定义类
来源：http://cxs.yj20258888.top

Py:   class User: pass
来源：http://jzn.ppjwa.cn

PHP:  class User {}
来源：http://hvt.ehwqpu.com

JS:   class User {}
来源：http://ija.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://ltl.9152youxi.cn

Java: class User {}
来源：http://ebd.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://jel.yangfankeji.com

Ruby: class User; end
来源：http://sud.zycfv.cn

C#:   class User {}
来源：http://unw.9152youxi.cn

[G02] 构造函数
来源：http://blo.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://oty.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://tid.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://dhd.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://bij.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://jbc.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://amw.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://iku.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://fbz.gotoacloud.top

[G03] 实例属性
来源：http://sdo.chenzaomai.com

Py:   self.name = "x"
来源：http://tnu.yonumen.top

PHP:  public string $name = "x";
来源：http://jve.tanke756.top

JS:   this.name = "x";
来源：http://qwi.jiagoushi.top

TS:   name: string = "x";
来源：http://mac.nanxuanxn.top

Java: private String name;
来源：http://qut.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wkl.jianghu66.top

Ruby: @name = "x"
来源：http://iwy.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://yxw.dianchejie.cn

[G04] 定义方法
来源：http://hrm.fehbvm.com

Py:   def greet(self): return self.name
来源：http://bnt.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nuh.mhx1999.top

JS:   greet() { return this.name; }
来源：http://dvl.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://bgb.fehbvm.com

Java: String greet() { return name; }
来源：http://pes.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://snq.xuanzx.com

Ruby: def greet; @name; end
来源：http://qxv.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://usk.sysykeji.top

[G05] 继承
来源：http://pgb.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://mdy.yongpay.top

PHP:  class Admin extends User {}
来源：http://wce.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://lbt.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://mmr.vehdjk.com

Java: class Admin extends User {}
来源：http://pya.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wif.cheryme.top

Ruby: class Admin < User; end
来源：http://ign.yfazqb.com

C#:   class Admin : User {}
来源：http://ajc.jqgfzy.top

[G06] 重写方法
来源：http://ywa.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://ptx.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mvz.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://nsx.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://mjt.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://pvf.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yov.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://mpy.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://msl.yj20258888.top

[G07] 调用父类方法
来源：http://zmg.aibaodan.cn

Py:   super().greet()
来源：http://woy.guowangkeji.top

PHP:  parent::greet();
来源：http://opk.zhixingplan.top

JS:   super.greet();
来源：http://cqo.shuidangran.top

TS:   super.greet();
来源：http://kvh.shanyushiyangtech.top

Java: super.greet();
来源：http://wru.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wtq.cqqwz.cn

Ruby: super
来源：http://fnq.yongpay.top

C#:   base.Greet();
来源：http://ucu.svipenyu.cn

[G08] 静态方法与属性
来源：http://gam.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oqy.daria6918.cn

PHP:  public static function f() {}
来源：http://lzy.zhoulong.xyz

JS:   static f() {}
来源：http://dxb.ppjwa.cn

TS:   static f(): void {}
来源：http://fgg.ywan-chungtsiang.top

Java: static void f() {}
来源：http://dkd.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lby.shuidangran.top

Ruby: def self.f; end
来源：http://dvf.xuanzx.com

C#:   public static void F() {}
来源：http://num.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://fbn.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://cdn.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://sgl.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kcm.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://cvl.yvedp.cn

Java: interface Shape { double area(); }
来源：http://rwt.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://oxf.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vzp.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://mmi.jlsjyb.cn

[G10] 访问控制
来源：http://rpr.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://spt.9152youxi.cn

PHP:  public / protected / private
来源：http://atl.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://ttb.tianlin.xyz

TS:   public / protected / private
来源：http://xfy.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://vog.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cgr.mhx1999.top

Ruby: public / protected / private
来源：http://zne.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://pvh.svipenyu.cn

[G11] getter / setter
来源：http://lek.cashguo.top

Py:   @property 与 @x.setter
来源：http://fzl.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ojj.fengsongda.top


<!-- 参考信息 -->