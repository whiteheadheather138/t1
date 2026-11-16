代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ahp.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nmt.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gve.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://llk.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://zip.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gii.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://naz.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cpw.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://icm.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kgi.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://itk.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://leu.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nxm.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://exd.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fbv.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqu.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kle.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bek.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yfl.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gtu.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bsc.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nxb.pengpengdd.cyou

[E16] 数字千分位
来源：http://kzb.fzhhl.top

Py:   f"{1234567:,}"
来源：http://niy.yj202588.top

PHP:  number_format(1234567);
来源：http://znf.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dwz.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://asx.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dld.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://raj.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vts.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://eex.fengsongda.top

[E17] 首字母大写
来源：http://fot.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sra.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhk.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tnk.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wrn.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nal.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cjv.zdbjq.cn

Ruby: s.capitalize
来源：http://aee.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fod.chenzaomai.com

[E18] 模板占位符替换
来源：http://gjh.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jss.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dcb.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ata.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vjh.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://afo.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ndl.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vhz.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ltg.hesvh.cn

[E19] 多行文本按行拆分
来源：http://oep.shuidangran.top

Py:   s.splitlines()
来源：http://txf.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mhw.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://ryu.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://wis.hnqzz.top

Java: s.lines().toList()
来源：http://fpn.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://blu.jlsjyb.cn

Ruby: s.lines
来源：http://egl.tanke756.top

C#:   s.Split('\n')
来源：http://sew.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://nne.jlsjyb.cn

Py:   if not s:
来源：http://yeg.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fkf.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://chk.jqgufenzy.top

TS:   if (s === "") {}
来源：http://qmf.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://slx.aizwys.cn

Go:   if s == "" {}
来源：http://hnl.shuidangran.top

Ruby: if s.empty?
来源：http://dzz.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cxw.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://lkd.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sfb.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ndz.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iph.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uay.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://alv.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://dfu.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cip.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pha.daxiang520.top

[E22] 字节长度与字符长度
来源：http://oid.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxx.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kjr.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bqa.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://stb.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lem.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://neh.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://fny.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jnx.gzhubu.top

================================================================================
来源：http://hbt.fzhhl.top

F. 文件与目录
来源：http://nwu.hnxiangtu.top

================================================================================
来源：http://iro.jiagoushi.top

[F01] 读取整个文件
来源：http://rxz.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gpz.pengpengdd.cyou

PHP:  file_get_contents("a.txt");
来源：http://gwo.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yqf.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jki.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yna.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://enb.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://srm.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://kbd.wangdashe.top

[F02] 逐行读取文件
来源：http://oxm.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mmo.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://geo.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qse.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xma.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dyv.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nru.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zgl.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://grj.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://uuv.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mpi.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ses.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brp.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gma.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://con.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rfu.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://ikq.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nsj.hcnkem.com

[F04] 追加写入文件
来源：http://htj.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xjl.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tmu.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqd.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zns.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hgs.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dwl.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyo.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cfc.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://twf.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hxg.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://svp.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://maz.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://nsw.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hgk.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjj.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://yrj.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://exz.zdqjudy.top

[F06] 删除文件
来源：http://odj.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://ggv.bjfxy.top

PHP:  unlink("a.txt");
来源：http://xpk.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://kgj.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://yhs.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dth.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://not.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://bby.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://qlv.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://soq.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aus.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vjv.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xpm.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kdr.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xrd.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ryk.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gbx.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dey.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://fhj.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsa.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://erm.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://qcg.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://mno.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kcp.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rie.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://vzs.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://cuy.meibo888.top

[F09] 获取文件大小
来源：http://svg.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://xka.smart0.xyz

PHP:  filesize("a.txt");
来源：http://fku.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://rma.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://xkm.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kpp.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jss.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://gfx.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://hmv.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://lav.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://euz.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gmt.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bjv.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://zpy.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lmq.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dwj.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://thc.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bkj.hnxiangtu.top

[F11] 复制与移动文件
来源：http://gsm.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kqf.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xyi.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwu.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eeq.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://src.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eqw.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dfz.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yyb.havefunace.top

[F12] CSV 读写
来源：http://cgr.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ksk.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsi.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tvg.ppjwa.cn

TS:   // 同上
来源：http://ppe.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nuy.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wne.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://enj.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xmx.hnxiangtu.top

================================================================================
来源：http://hui.hongshengwenyu.top

G. 面向对象
来源：http://thg.wangdashe.top

================================================================================
来源：http://ugu.0kj1m.cn

[G01] 定义类
来源：http://ijn.wangshuangyany.cn

Py:   class User: pass
来源：http://tcc.jiagoushi.top

PHP:  class User {}
来源：http://ibb.nwbrower.top

JS:   class User {}
来源：http://ler.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://mhy.hesvh.cn

Java: class User {}
来源：http://hew.dianchejie.cn

Go:   type User struct { Name string }
来源：http://wyh.sjlbkw.cn

Ruby: class User; end
来源：http://khg.birdmap.top

C#:   class User {}
来源：http://osf.ydjk.org.cn

[G02] 构造函数
来源：http://eeh.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://kjn.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://ewp.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://hle.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://vqn.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://ezl.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://omt.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vvn.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://kye.yongpay.top

[G03] 实例属性
来源：http://nny.jinqigfzy.top

Py:   self.name = "x"
来源：http://jca.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://etr.ivvv.top

JS:   this.name = "x";
来源：http://fro.dianchejie.cn

TS:   name: string = "x";
来源：http://mhf.nwbrower.top

Java: private String name;
来源：http://lnj.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://klp.zhixingplan.top

Ruby: @name = "x"
来源：http://cpe.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://zky.xuanzx.com

[G04] 定义方法
来源：http://bzc.andypj.xyz

Py:   def greet(self): return self.name
来源：http://xnn.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://itc.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://xan.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://mgv.tarul.cn

Java: String greet() { return name; }
来源：http://ebj.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zak.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://vss.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://grt.xinyue.icu

[G05] 继承
来源：http://ttp.316326.xyz

Py:   class Admin(User): pass
来源：http://krf.xinyue.icu

PHP:  class Admin extends User {}
来源：http://kav.bbcook.cn

JS:   class Admin extends User {}
来源：http://ule.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://kof.daria6918.cn

Java: class Admin extends User {}
来源：http://noi.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ztl.guannengcc.top

Ruby: class Admin < User; end
来源：http://iyk.jlsjyb.cn

C#:   class Admin : User {}
来源：http://yqa.aizwys.cn

[G06] 重写方法
来源：http://quk.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://ykt.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kwg.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://rvr.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://zid.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://znp.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wug.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://fue.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://tkw.hesvh.cn

[G07] 调用父类方法
来源：http://ryg.yj20258.top

Py:   super().greet()
来源：http://svx.dianchejie.cn

PHP:  parent::greet();
来源：http://vsu.yfazqb.com

JS:   super.greet();
来源：http://pzy.uphjek.com

TS:   super.greet();
来源：http://rfm.zhongyouzk.top

Java: super.greet();
来源：http://bje.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aji.zhiwuduotai.top

Ruby: super
来源：http://wos.ydzc1.top

C#:   base.Greet();
来源：http://rob.zycfv.cn

[G08] 静态方法与属性
来源：http://ail.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qtl.xylfe.cn

PHP:  public static function f() {}
来源：http://uif.xuetiantiany.cn

JS:   static f() {}
来源：http://dce.xylfe.cn

TS:   static f(): void {}
来源：http://vxg.jqgufenzy.top

Java: static void f() {}
来源：http://nxp.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oub.pycfn.com

Ruby: def self.f; end
来源：http://thy.yj20258888.top

C#:   public static void F() {}
来源：http://lev.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://fbv.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://ilk.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://ive.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://aau.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://oxp.daria6918.cn

Java: interface Shape { double area(); }
来源：http://lzi.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://bfv.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://clv.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://iga.jyoumei.cn

[G10] 访问控制
来源：http://web.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://mrp.ctjpmb.com

PHP:  public / protected / private
来源：http://kfg.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://kgu.zhiwuduotai.top

TS:   public / protected / private
来源：http://ehe.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://yjv.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dwr.aizwys.cn

Ruby: public / protected / private
来源：http://lvp.ivvv.top

C#:   public / protected / private / internal
来源：http://ilt.kuanghao11.cn

[G11] getter / setter
来源：http://iif.yj20258.top

Py:   @property 与 @x.setter
来源：http://nuy.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://amb.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://ipb.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://utt.pycfn.com

Java: public String getName() { return name; }
来源：http://uja.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqk.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://uiy.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://pvq.gogol.net.cn

[G12] 对象转字符串
来源：http://kci.yj202588.top

Py:   def __str__(self): return self.name
来源：http://rvh.chenlongwang.top


<!-- 参考信息 -->