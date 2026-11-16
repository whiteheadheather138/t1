代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndf.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gqw.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kut.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ale.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://jjo.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gxk.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ljp.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ocj.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ign.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gho.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cxl.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tzz.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wjn.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://nky.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gwx.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cnf.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ars.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gkl.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eoa.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rjc.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lwi.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cwv.feifeiyinyue.top

[E16] 数字千分位
来源：http://wgw.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://fbz.epnwcf.com

PHP:  number_format(1234567);
来源：http://imj.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cwx.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://czf.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bjy.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xyd.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rdn.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://wyi.zycfv.cn

[E17] 首字母大写
来源：http://mvv.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ftw.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kyh.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikr.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akn.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://udp.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gzn.yj20258.top

Ruby: s.capitalize
来源：http://ftx.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rya.nanxinkj.top

[E18] 模板占位符替换
来源：http://qcw.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wnh.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fpe.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://sgx.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://uog.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tgt.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jsc.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dtp.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lrp.yongpay.top

[E19] 多行文本按行拆分
来源：http://gbi.gaohongyu789.top

Py:   s.splitlines()
来源：http://yjv.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyt.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://wrv.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://ita.yj202588.top

Java: s.lines().toList()
来源：http://ecm.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://itb.zdqjudy.top

Ruby: s.lines
来源：http://xel.yvedp.cn

C#:   s.Split('\n')
来源：http://rug.tarul.cn

[E20] 判断字符串是否为空
来源：http://has.vehdjk.com

Py:   if not s:
来源：http://kzb.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uzd.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ezw.c1oappe.top

TS:   if (s === "") {}
来源：http://ekq.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://tzh.yj202588.top

Go:   if s == "" {}
来源：http://wea.chenlongwang.top

Ruby: if s.empty?
来源：http://bqf.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ftg.meibo888.top

[E21] 超长截断加省略号
来源：http://avh.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hsq.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yms.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agu.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hnt.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yvm.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://edq.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yno.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kfo.aizwys.cn

[E22] 字节长度与字符长度
来源：http://dmu.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rmy.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwj.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdb.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mjq.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rsu.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://icx.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://ujk.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhr.vehdjk.com

================================================================================
来源：http://ize.yvedp.cn

F. 文件与目录
来源：http://pto.redwolf501.top

================================================================================
来源：http://xvb.zdbjq.cn

[F01] 读取整个文件
来源：http://ojm.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cqm.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://iov.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://igp.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qeb.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://pdl.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ymk.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://gsr.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://ohb.aibaodan.cn

[F02] 逐行读取文件
来源：http://igj.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mkn.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fyd.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xbd.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyf.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://urz.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://djf.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mkx.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zbc.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://drq.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fbt.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aus.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ujd.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxf.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://btq.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lka.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://khg.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gjj.vehdjk.com

[F04] 追加写入文件
来源：http://yeb.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yyu.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://naz.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvb.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixl.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yos.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://itj.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://amj.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xrs.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://miu.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hfk.tarul.cn

PHP:  file_exists("a.txt");
来源：http://eul.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://wtc.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://rak.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xpg.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pto.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://bvw.yj202588.top

C#:   File.Exists("a.txt")
来源：http://hnp.jianghu66.top

[F06] 删除文件
来源：http://rpx.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://lil.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://rjy.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://xde.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://wzg.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rpk.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://ybk.havefunace.top

Ruby: File.delete("a.txt")
来源：http://nvo.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://loz.redwolf501.top

[F07] 创建目录（含多级）
来源：http://esn.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sdg.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jox.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzk.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejy.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hci.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uhi.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kmy.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jcd.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://nrn.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bmp.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ojk.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://xew.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://lzi.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tir.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aqi.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://pbi.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://asm.wangshuangyany.cn

[F09] 获取文件大小
来源：http://qxl.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://dtk.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://edx.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://fqn.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://zpt.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xae.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jnd.fktsv.cn

Ruby: File.size("a.txt")
来源：http://hgz.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://nft.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://kgu.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tbv.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://unp.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://anc.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://byn.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nfc.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://npg.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dfo.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhc.cheryme.top

[F11] 复制与移动文件
来源：http://vfe.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rsa.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oem.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmj.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sps.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aag.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ote.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xyy.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vkd.andypj.xyz

[F12] CSV 读写
来源：http://ieg.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ycn.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qcc.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hie.chenlongwang.top

TS:   // 同上
来源：http://ihi.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://idg.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ocr.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nxh.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xqh.sysykeji.top

================================================================================
来源：http://mhh.hfpthk.cn

G. 面向对象
来源：http://tln.xuetiantiany.cn

================================================================================
来源：http://ose.jinqigufen.top

[G01] 定义类
来源：http://wyp.sxryk.cn

Py:   class User: pass
来源：http://zdi.jqgfzy.top

PHP:  class User {}
来源：http://muw.xingfuxueyuan.xyz

JS:   class User {}
来源：http://wia.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://lgi.zdbjq.cn

Java: class User {}
来源：http://ezb.sufxvd.cn

Go:   type User struct { Name string }
来源：http://njp.ydzc1.top

Ruby: class User; end
来源：http://qno.yfazqb.com

C#:   class User {}
来源：http://lra.vqdsnc.cn

[G02] 构造函数
来源：http://dru.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://hhe.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://mzr.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://kba.hammf.cn

TS:   constructor(public name: string) {}
来源：http://osb.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://nwr.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qtg.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://xjc.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://jwp.jyoumei.cn

[G03] 实例属性
来源：http://ttj.epnwcf.com

Py:   self.name = "x"
来源：http://xko.zdbjq.cn

PHP:  public string $name = "x";
来源：http://hqs.hammf.cn

JS:   this.name = "x";
来源：http://dsb.9152youxi.cn

TS:   name: string = "x";
来源：http://fbt.xziqi.cn

Java: private String name;
来源：http://uzc.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hey.zhoulong.xyz

Ruby: @name = "x"
来源：http://jvs.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://qlq.hysaishi.cn

[G04] 定义方法
来源：http://lmn.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://uuq.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://slp.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://tcy.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://kqd.yvedp.cn

Java: String greet() { return name; }
来源：http://kpr.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zvg.yvedp.cn

Ruby: def greet; @name; end
来源：http://pmc.hcnkem.com

C#:   public string Greet() => Name;
来源：http://vll.guowangkeji.top

[G05] 继承
来源：http://mec.cqqwz.cn

Py:   class Admin(User): pass
来源：http://xrn.xinyue.icu

PHP:  class Admin extends User {}
来源：http://zgz.jqgfzy.top

JS:   class Admin extends User {}
来源：http://wro.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://wvk.yj20258.top

Java: class Admin extends User {}
来源：http://iit.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cpw.yonumen.top

Ruby: class Admin < User; end
来源：http://xmu.cheryme.top

C#:   class Admin : User {}
来源：http://ril.guowangkeji.top

[G06] 重写方法
来源：http://xdr.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://ute.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ozx.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://ayv.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://pto.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://crl.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rhr.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://ejl.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://rlb.sufxvd.cn

[G07] 调用父类方法
来源：http://gda.jqgufenzy.top

Py:   super().greet()
来源：http://dnt.yj202588.top

PHP:  parent::greet();
来源：http://fxe.jlsjyb.cn

JS:   super.greet();
来源：http://kjd.fengsongda.top

TS:   super.greet();
来源：http://enp.xuetiantiany.cn

Java: super.greet();
来源：http://mff.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mtg.shzxlz.cn

Ruby: super
来源：http://wcb.bjfxy.top

C#:   base.Greet();
来源：http://xvd.xinyue.icu

[G08] 静态方法与属性
来源：http://gej.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://neo.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://qfd.dashuyun.cn

JS:   static f() {}
来源：http://gqp.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://ljj.redwolf501.top

Java: static void f() {}
来源：http://hdh.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rpl.hesvh.cn

Ruby: def self.f; end
来源：http://uip.cashguo.top

C#:   public static void F() {}
来源：http://gbe.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://rol.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://faj.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://ymy.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xsw.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://png.hcnkem.com

Java: interface Shape { double area(); }
来源：http://uqv.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://sss.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://agz.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://cpc.gotoacloud.top

[G10] 访问控制
来源：http://uco.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://qnb.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://zzb.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://mfb.havefunace.top

TS:   public / protected / private
来源：http://qwn.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://vfd.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://msv.c1oappe.top

Ruby: public / protected / private
来源：http://esk.tarul.cn

C#:   public / protected / private / internal
来源：http://mrc.gotoacloud.top

[G11] getter / setter
来源：http://vbs.fzhhl.top

Py:   @property 与 @x.setter
来源：http://rre.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wra.fzhhl.top

JS:   get name() { return this._name; }
来源：http://emh.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://kgg.fzhhl.top

Java: public String getName() { return name; }
来源：http://tgj.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://djd.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://frl.vehdjk.com

C#:   public string Name { get; set; }
来源：http://zcs.redwolf501.top

[G12] 对象转字符串
来源：http://owd.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://ygt.zhoulong.xyz


<!-- 参考信息 -->