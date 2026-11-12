代发 wailian999

[E14] URL 编码与 Base64
来源：http://pwo.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wux.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://syy.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qko.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qax.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ydk.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bct.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odh.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zuv.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://stt.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dzm.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nnu.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fxg.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jns.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ojj.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ahj.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qie.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsn.ydzc1.top

[E16] 数字千分位
来源：http://jzl.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://bah.zycfv.cn

PHP:  number_format(1234567);
来源：http://ptt.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kgw.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tgh.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wae.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nhq.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vzy.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://qie.gogol.net.cn

[E17] 首字母大写
来源：http://llm.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zck.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kwj.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wjf.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkv.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gvc.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ykq.aibaodan.cn

Ruby: s.capitalize
来源：http://tyn.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lnv.yj202588.top

[E18] 模板占位符替换
来源：http://eme.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sbs.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nja.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hii.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://unv.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gqk.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rks.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yka.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lqc.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://clw.tianlin.xyz

Py:   s.splitlines()
来源：http://vkq.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aqz.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://zot.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://ioi.ydjk.org.cn

Java: s.lines().toList()
来源：http://xqs.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://ako.zhoulong.xyz

Ruby: s.lines
来源：http://dna.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://bha.bjfxy.top

[E20] 判断字符串是否为空
来源：http://qqz.zhijiandao.cn

Py:   if not s:
来源：http://drf.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ulz.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rqq.bjfxy.top

TS:   if (s === "") {}
来源：http://jyi.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://ffw.jlsjyb.cn

Go:   if s == "" {}
来源：http://yth.cashguo.top

Ruby: if s.empty?
来源：http://yrb.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fsj.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://pel.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://brl.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dir.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsi.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tiy.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imw.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://hgm.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ach.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ppn.daria6918.cn

[E22] 字节长度与字符长度
来源：http://cfv.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://spg.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nhs.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqd.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://auz.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nxt.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://huz.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://vzu.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://szq.gzhubu.top

================================================================================
来源：http://ftu.vqdsnc.cn

F. 文件与目录
来源：http://ssp.9152youxi.cn

================================================================================
来源：http://ouq.yueranfly.top

[F01] 读取整个文件
来源：http://gny.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dow.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://mwy.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ldn.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jpl.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qrx.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://duc.ydzc1.top

Ruby: File.read("a.txt")
来源：http://tni.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://bdq.xuanzx.com

[F02] 逐行读取文件
来源：http://bks.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://odt.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xgy.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://woa.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ccj.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://seq.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aus.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hbm.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iur.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://vze.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://krz.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ifk.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kog.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://chg.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwk.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tup.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://ouv.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jpg.meibo888.top

[F04] 追加写入文件
来源：http://muf.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://usj.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dyq.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://piw.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmo.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://geu.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qcy.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rqd.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://env.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://cub.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wyb.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://quy.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://jgw.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://lhb.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wqm.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyr.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://uaw.cheryme.top

C#:   File.Exists("a.txt")
来源：http://dgh.fktsv.cn

[F06] 删除文件
来源：http://lps.fzhhl.top

Py:   os.remove("a.txt")
来源：http://aou.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://tey.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pql.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://yba.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yda.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://ggu.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://jtc.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://sjq.hesvh.cn

[F07] 创建目录（含多级）
来源：http://zic.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mfj.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wlf.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trg.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nya.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ocd.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vjh.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jdy.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://srj.fzhhl.top

[F08] 遍历目录
来源：http://wgq.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://igo.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qqn.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://uxo.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://oel.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xcf.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lxs.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://rhn.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://uui.nwbrower.top

[F09] 获取文件大小
来源：http://wcp.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://rdk.sweek.top

PHP:  filesize("a.txt");
来源：http://okn.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://zxt.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://wqi.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ltr.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://skb.ydzc1.top

Ruby: File.size("a.txt")
来源：http://zhy.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://wrk.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://uwk.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vjk.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cmq.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pix.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://pkw.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwn.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rsz.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rwp.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eym.dianchejie.cn

[F11] 复制与移动文件
来源：http://vzl.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vrt.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://edk.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://biv.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpd.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vwg.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmn.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dvr.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eod.fanxiaobao.xyz

[F12] CSV 读写
来源：http://oaa.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lcz.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fwy.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ncj.pengpengdd.cyou

TS:   // 同上
来源：http://zjh.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://snx.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hlr.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vbe.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fxt.pycfn.com

================================================================================
来源：http://rmh.shanyushiyangtech.top

G. 面向对象
来源：http://gus.haohaochexian.top

================================================================================
来源：http://mzz.zhixingplan.top

[G01] 定义类
来源：http://aea.ppjwa.cn

Py:   class User: pass
来源：http://mbs.ydjk.org.cn

PHP:  class User {}
来源：http://kyu.hesvh.cn

JS:   class User {}
来源：http://pku.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://fvo.xinyue.icu

Java: class User {}
来源：http://avp.chenlongwang.top

Go:   type User struct { Name string }
来源：http://sib.sxryk.cn

Ruby: class User; end
来源：http://gqf.yj202588.top

C#:   class User {}
来源：http://hgz.xziqi.cn

[G02] 构造函数
来源：http://apm.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://wmw.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://xul.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://cbi.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://dat.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://npf.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ndg.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://lcs.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://qlw.pengpengdd.cyou

[G03] 实例属性
来源：http://isv.jqgufenzy.top

Py:   self.name = "x"
来源：http://gpz.hywenlv.cn

PHP:  public string $name = "x";
来源：http://ohj.hysaishi.cn

JS:   this.name = "x";
来源：http://umm.cheryme.top

TS:   name: string = "x";
来源：http://pxw.zhaomingkeji.xyz

Java: private String name;
来源：http://cdt.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rzg.snrcjt.cn

Ruby: @name = "x"
来源：http://nzv.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://wym.redwolf501.top

[G04] 定义方法
来源：http://xdd.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://pjd.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ukg.tarul.cn

JS:   greet() { return this.name; }
来源：http://mtf.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://wts.ctjpmb.com

Java: String greet() { return name; }
来源：http://drx.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lcf.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://ftb.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://qou.jinqigufen.top

[G05] 继承
来源：http://cmn.daria6918.cn

Py:   class Admin(User): pass
来源：http://fia.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://pgc.redwolf501.top

JS:   class Admin extends User {}
来源：http://lnv.vehdjk.com

TS:   class Admin extends User {}
来源：http://vsp.kuanghao11.cn

Java: class Admin extends User {}
来源：http://kmh.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rsm.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://npq.bbcook.cn

C#:   class Admin : User {}
来源：http://rdi.sysykeji.top

[G06] 重写方法
来源：http://dhg.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://uhc.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://esp.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://qta.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://wty.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://ybr.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yjl.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://rkw.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://dti.andypj.xyz

[G07] 调用父类方法
来源：http://mqn.sxryk.cn

Py:   super().greet()
来源：http://wcs.jianghu66.top

PHP:  parent::greet();
来源：http://hbr.snrcjt.cn

JS:   super.greet();
来源：http://osy.sysykeji.top

TS:   super.greet();
来源：http://fkv.fengsongda.top

Java: super.greet();
来源：http://lzd.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://icx.hysaishi.cn

Ruby: super
来源：http://tst.ydzc1.top

C#:   base.Greet();
来源：http://nde.guannengcc.top

[G08] 静态方法与属性
来源：http://jcx.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://itq.gzhubu.top

PHP:  public static function f() {}
来源：http://czn.316326.xyz

JS:   static f() {}
来源：http://ttm.gaohongyu789.top

TS:   static f(): void {}
来源：http://nly.chenlongwang.top

Java: static void f() {}
来源：http://ffj.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ylk.jyoumei.cn

Ruby: def self.f; end
来源：http://tnl.cdnleiting.top

C#:   public static void F() {}
来源：http://bbm.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://yjz.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://noq.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://rfm.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ckc.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://ysk.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://xth.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://tis.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zsg.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://pjv.haohaochexian.top

[G10] 访问控制
来源：http://bup.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://hap.epnwcf.com

PHP:  public / protected / private
来源：http://urh.gzhubu.top

JS:   #private 字段；其余公开
来源：http://xml.yuxming.cn

TS:   public / protected / private
来源：http://iba.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://nrk.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xwm.sysykeji.top

Ruby: public / protected / private
来源：http://lza.hfpthk.cn

C#:   public / protected / private / internal
来源：http://the.tian-w.cn

[G11] getter / setter
来源：http://xgo.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://lsj.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://amz.nwbrower.top

JS:   get name() { return this._name; }
来源：http://ous.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://eyx.hfpthk.cn

Java: public String getName() { return name; }
来源：http://vnc.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rdk.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://pnm.sysykeji.top

C#:   public string Name { get; set; }
来源：http://xts.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://sos.pycfn.com

Py:   def __str__(self): return self.name
来源：http://mvx.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ebq.hcnkem.com

JS:   toString() { return this.name; }
来源：http://gmd.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://htz.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://mqr.yj20258.top


<!-- 参考信息 -->