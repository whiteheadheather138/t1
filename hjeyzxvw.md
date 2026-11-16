代发 wailian999

Go:   strings.Count(s, "a")
来源：http://qgz.tianlin.xyz

Ruby: s.count("a")
来源：http://luc.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://rsa.svipenyu.cn

[E13] 逐字符遍历
来源：http://ayv.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://srz.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ttj.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jht.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://biz.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gvc.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wcq.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://fyo.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qct.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://swy.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhx.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ebe.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pal.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efu.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gnn.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jqq.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://prr.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zrx.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://fsm.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lut.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sdf.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zjh.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pzq.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ihx.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vta.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dtc.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vut.chenjidiqi.icu

[E16] 数字千分位
来源：http://ibc.yvedp.cn

Py:   f"{1234567:,}"
来源：http://mlu.daria6918.cn

PHP:  number_format(1234567);
来源：http://tir.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://mux.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mit.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oar.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ndp.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tjg.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://slg.feifeiyinyue.top

[E17] 首字母大写
来源：http://ghy.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qdf.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://grt.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgz.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vjr.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://adf.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jzr.fengsongda.top

Ruby: s.capitalize
来源：http://qao.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tjt.pycfn.com

[E18] 模板占位符替换
来源：http://jon.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vwy.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yde.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://amd.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nvx.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dxz.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pyl.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jad.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iny.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://qxn.iojbl.cn

Py:   s.splitlines()
来源：http://jru.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oji.sweek.top

JS:   s.split(/\r?\n/)
来源：http://whr.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://zba.bjfxy.top

Java: s.lines().toList()
来源：http://qra.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://kkm.mhx1999.top

Ruby: s.lines
来源：http://dwa.yj202588.top

C#:   s.Split('\n')
来源：http://zzc.meibo888.top

[E20] 判断字符串是否为空
来源：http://bjt.hysaishi.cn

Py:   if not s:
来源：http://mlo.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hxx.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://knh.jqgfzy.top

TS:   if (s === "") {}
来源：http://otw.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://umu.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://ovo.zhoulong.xyz

Ruby: if s.empty?
来源：http://bhu.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vgv.ybcxt.top

[E21] 超长截断加省略号
来源：http://pdm.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yvt.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yqy.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ain.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzr.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nom.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://alm.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://row.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ftr.sysykeji.top

[E22] 字节长度与字符长度
来源：http://afj.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lbp.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrj.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sfd.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://osj.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tbl.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmi.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://idv.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://osh.chenjidiqi.icu

================================================================================
来源：http://aeb.cucudq.cn

F. 文件与目录
来源：http://vuw.hywenlv.cn

================================================================================
来源：http://gkw.pycfn.com

[F01] 读取整个文件
来源：http://nel.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xwj.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://zmq.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://abj.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bdq.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dqt.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gzp.xuanzx.com

Ruby: File.read("a.txt")
来源：http://ipt.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://qdr.haohaochexian.top

[F02] 逐行读取文件
来源：http://hyr.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://plq.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjb.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mtc.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwc.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pyi.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tzt.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://txf.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lwf.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://nvq.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kjf.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dku.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ame.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bfi.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lqb.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dbq.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://wsa.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bch.redwolf501.top

[F04] 追加写入文件
来源：http://ihd.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mvo.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://umn.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cja.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wje.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gey.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://quj.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://myn.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pug.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://gkq.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qit.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://spk.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://ysl.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://tfm.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://bzp.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://skz.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://mwo.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://uly.xuanzx.com

[F06] 删除文件
来源：http://jss.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://qnk.sweek.top

PHP:  unlink("a.txt");
来源：http://wei.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jyv.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jkn.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dfo.birdmap.top

Go:   os.Remove("a.txt")
来源：http://spp.hammf.cn

Ruby: File.delete("a.txt")
来源：http://epm.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://nwm.havefunace.top

[F07] 创建目录（含多级）
来源：http://aub.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nvr.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ibg.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nxt.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qsp.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fqi.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jxr.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pxp.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rbf.zycfv.cn

[F08] 遍历目录
来源：http://mkk.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxl.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qny.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://gjm.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://rcx.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dys.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdv.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://nwr.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://rnj.yongpay.top

[F09] 获取文件大小
来源：http://pxm.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://ink.cucudq.cn

PHP:  filesize("a.txt");
来源：http://mkl.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://clx.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://hiu.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wfo.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qsg.ybcxt.top

Ruby: File.size("a.txt")
来源：http://dtu.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://zlw.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://rip.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://grw.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lln.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iiu.xinyue.icu

TS:   path.extname("a.txt")
来源：http://gcg.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fvm.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ujp.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vez.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ber.gzhubu.top

[F11] 复制与移动文件
来源：http://cde.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mcn.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iye.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cty.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://max.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ijx.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xtu.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gvf.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oxr.kuanghao11.cn

[F12] CSV 读写
来源：http://ahi.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wlo.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kpp.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sab.chenjidiqi.icu

TS:   // 同上
来源：http://qoe.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://drp.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yto.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jwm.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://odp.quarkkingdee.top

================================================================================
来源：http://zlq.yangfankeji.com

G. 面向对象
来源：http://yel.fzhhl.top

================================================================================
来源：http://hwv.zhijiandao.cn

[G01] 定义类
来源：http://thj.epnwcf.com

Py:   class User: pass
来源：http://hld.vqdsnc.cn

PHP:  class User {}
来源：http://fww.cdnleiting.top

JS:   class User {}
来源：http://ptg.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://igs.shangyingyoupin.top

Java: class User {}
来源：http://qai.jinqigufen.top

Go:   type User struct { Name string }
来源：http://xdc.xuetiantiany.cn

Ruby: class User; end
来源：http://kcp.dianchejie.cn

C#:   class User {}
来源：http://lgz.yonumen.top

[G02] 构造函数
来源：http://rss.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://kay.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://moc.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://bol.tanke756.top

TS:   constructor(public name: string) {}
来源：http://fpk.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://igk.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qlr.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://rqz.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://oyx.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://nhz.316326.xyz

Py:   self.name = "x"
来源：http://dbm.0kj1m.cn

PHP:  public string $name = "x";
来源：http://ikb.hfpthk.cn

JS:   this.name = "x";
来源：http://owp.shuidangran.top

TS:   name: string = "x";
来源：http://wum.bbcook.cn

Java: private String name;
来源：http://ouh.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wjn.xylfe.cn

Ruby: @name = "x"
来源：http://wgl.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://wxx.nwbrower.top

[G04] 定义方法
来源：http://xqm.yvedp.cn

Py:   def greet(self): return self.name
来源：http://ivx.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://zuz.fengsongda.top

JS:   greet() { return this.name; }
来源：http://plj.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://yjh.cdnleiting.top

Java: String greet() { return name; }
来源：http://vfl.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eti.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://nxq.yongpay.top

C#:   public string Greet() => Name;
来源：http://gpo.guannengcc.top

[G05] 继承
来源：http://uev.cheryme.top

Py:   class Admin(User): pass
来源：http://inq.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://veq.fzhhl.top

JS:   class Admin extends User {}
来源：http://fdd.xinyue.icu

TS:   class Admin extends User {}
来源：http://gep.ydjk.org.cn

Java: class Admin extends User {}
来源：http://rpi.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iyz.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://xny.andypj.xyz

C#:   class Admin : User {}
来源：http://uha.tarul.cn

[G06] 重写方法
来源：http://spm.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://sxp.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pag.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://qmr.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://oxs.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://tbs.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kub.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://iil.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://wnx.gaohongyu789.top

[G07] 调用父类方法
来源：http://bps.pengpengdd.cyou

Py:   super().greet()
来源：http://ahq.zhijiandao.cn

PHP:  parent::greet();
来源：http://nvo.chenzaomai.com

JS:   super.greet();
来源：http://nno.chenzaomai.com

TS:   super.greet();
来源：http://unk.guowangkeji.top

Java: super.greet();
来源：http://wuf.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gdf.yangfankeji.com

Ruby: super
来源：http://noy.xuetiantiany.cn

C#:   base.Greet();
来源：http://tak.0kj1m.cn

[G08] 静态方法与属性
来源：http://fpi.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ibx.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://gxf.yuanzhike.top

JS:   static f() {}
来源：http://gwy.yfazqb.com

TS:   static f(): void {}
来源：http://nvm.cheryme.top

Java: static void f() {}
来源：http://qct.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mtv.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://ccc.xuetiantiany.cn

C#:   public static void F() {}
来源：http://qfn.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://sux.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://bni.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://rzw.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://utf.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://hck.cucudq.cn

Java: interface Shape { double area(); }
来源：http://lpr.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://erk.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jvu.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://ycv.gaohongyu789.top

[G10] 访问控制
来源：http://fum.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://jxy.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://qbo.cucudq.cn

JS:   #private 字段；其余公开
来源：http://ikg.xziqi.cn

TS:   public / protected / private
来源：http://opl.yj20258.top

Java: public / protected / private / 默认包级
来源：http://exn.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qyb.jinqigfzy.top

Ruby: public / protected / private
来源：http://fju.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://dak.9152youxi.cn

[G11] getter / setter
来源：http://qzu.ybcxt.top

Py:   @property 与 @x.setter
来源：http://dhk.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://boq.kuanghao11.cn


<!-- 参考信息 -->