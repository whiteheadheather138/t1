代发 wailian999

[E14] URL 编码与 Base64
来源：http://qiv.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uld.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pte.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ibp.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvz.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sjx.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tmu.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kxp.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xhu.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://dnk.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ycm.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uzh.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xss.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tvj.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqs.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://czg.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fkm.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhn.xuetiantiany.cn

[E16] 数字千分位
来源：http://uln.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://zzu.xziqi.cn

PHP:  number_format(1234567);
来源：http://sjv.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gfi.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ejc.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://plp.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ydp.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mjm.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://etg.feifeiyinyue.top

[E17] 首字母大写
来源：http://mnw.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgk.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jfv.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nlh.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lch.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://voq.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uln.sjlbkw.cn

Ruby: s.capitalize
来源：http://mdt.dashuyun.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ypw.xuanzx.com

[E18] 模板占位符替换
来源：http://ozo.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eso.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ekn.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rww.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zwh.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dia.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ezv.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmm.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyq.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://tvo.gzhubu.top

Py:   s.splitlines()
来源：http://xru.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yrv.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://hzr.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://zvy.jiagoushi.top

Java: s.lines().toList()
来源：http://gdn.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://ykt.hammf.cn

Ruby: s.lines
来源：http://kfa.yuanzhike.top

C#:   s.Split('\n')
来源：http://aus.tian-w.cn

[E20] 判断字符串是否为空
来源：http://ajg.xuetiantiany.cn

Py:   if not s:
来源：http://suf.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://agn.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vcw.guowangkeji.top

TS:   if (s === "") {}
来源：http://rpp.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://bat.yuanzhike.top

Go:   if s == "" {}
来源：http://thj.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://snl.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://enm.mhx1999.top

[E21] 超长截断加省略号
来源：http://dfc.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xxj.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rqp.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xcy.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mng.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nmc.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://evq.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aps.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bfh.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://qfm.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fkb.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zrv.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyo.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://btx.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mwc.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ymm.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://ect.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://emz.c1oappe.top

================================================================================
来源：http://gvx.zhixingplan.top

F. 文件与目录
来源：http://pfn.andypj.xyz

================================================================================
来源：http://mdj.pycfn.com

[F01] 读取整个文件
来源：http://leu.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzt.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://oib.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://adg.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gqv.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fmo.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aio.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://ntm.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://yhs.havefunace.top

[F02] 逐行读取文件
来源：http://nuo.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fni.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://quj.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cts.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://beq.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fww.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cot.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ius.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cgw.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://omq.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wmf.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eyk.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfa.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bld.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nck.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dyh.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://bpc.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://auf.vehdjk.com

[F04] 追加写入文件
来源：http://tcz.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ric.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mnq.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjl.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dao.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hcc.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfo.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://orl.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ocx.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://xbq.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jvs.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://voh.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://deo.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://hul.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uqr.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gkq.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://lnn.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://scm.guowangkeji.top

[F06] 删除文件
来源：http://pdh.c1oappe.top

Py:   os.remove("a.txt")
来源：http://ayk.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://euz.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://lgp.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mgb.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jos.cheryme.top

Go:   os.Remove("a.txt")
来源：http://sak.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://sbr.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://hzf.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://hip.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yye.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://btg.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dih.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpv.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ufx.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ooc.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zpt.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rsz.hcnkem.com

[F08] 遍历目录
来源：http://ptl.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pro.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vwf.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://fha.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://yir.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://emp.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbs.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://kuj.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://hth.zhixingplan.top

[F09] 获取文件大小
来源：http://kgo.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://ons.birdmap.top

PHP:  filesize("a.txt");
来源：http://vqv.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://zvr.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://tzg.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://avc.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehx.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://sxz.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://pbp.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://btr.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oup.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cza.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwi.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://vmw.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cux.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://goh.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://etr.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lku.gzhubu.top

[F11] 复制与移动文件
来源：http://xvp.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cqs.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqv.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kpc.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvl.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tbz.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blj.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://shj.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kbg.zhijiandao.cn

[F12] CSV 读写
来源：http://lfy.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlo.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://llj.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yhj.kuanghao11.cn

TS:   // 同上
来源：http://upc.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yzb.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sig.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jlt.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ulp.tianlin.xyz

================================================================================
来源：http://nva.pycfn.com

G. 面向对象
来源：http://fpd.jyoumei.cn

================================================================================
来源：http://gkg.bbcook.cn

[G01] 定义类
来源：http://ura.cucudq.cn

Py:   class User: pass
来源：http://vvz.epnwcf.com

PHP:  class User {}
来源：http://luc.52xcode.cn

JS:   class User {}
来源：http://qbh.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://gft.zhongyouzk.top

Java: class User {}
来源：http://ayh.yueranfly.top

Go:   type User struct { Name string }
来源：http://zyr.zhaomingkeji.xyz

Ruby: class User; end
来源：http://dwq.hcnkem.com

C#:   class User {}
来源：http://cqo.daria6918.cn

[G02] 构造函数
来源：http://hie.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://dhg.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://kyq.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://gau.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://nmi.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://uci.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nbv.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://aug.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ndz.ywan-chungtsiang.top

[G03] 实例属性
来源：http://gjm.tian-w.cn

Py:   self.name = "x"
来源：http://vep.jyoumei.cn

PHP:  public string $name = "x";
来源：http://slw.yonumen.top

JS:   this.name = "x";
来源：http://nch.hywenlv.cn

TS:   name: string = "x";
来源：http://gfv.dashuyun.cn

Java: private String name;
来源：http://hln.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xed.c1oappe.top

Ruby: @name = "x"
来源：http://ygn.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://spq.zhongyouzk.top

[G04] 定义方法
来源：http://uwe.smart0.xyz

Py:   def greet(self): return self.name
来源：http://wfb.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wef.nwbrower.top

JS:   greet() { return this.name; }
来源：http://zsi.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://lhk.gotoacloud.top

Java: String greet() { return name; }
来源：http://ntq.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cql.hesvh.cn

Ruby: def greet; @name; end
来源：http://hxf.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://qjw.jinqigfzy.top

[G05] 继承
来源：http://xwg.bbcook.cn

Py:   class Admin(User): pass
来源：http://lhi.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://qzo.haohaochexian.top

JS:   class Admin extends User {}
来源：http://gve.hysaishi.cn

TS:   class Admin extends User {}
来源：http://zga.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://hpa.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://unk.yfazqb.com

Ruby: class Admin < User; end
来源：http://kad.sweek.top

C#:   class Admin : User {}
来源：http://zyj.hesvh.cn

[G06] 重写方法
来源：http://ldp.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://sot.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kkv.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://qlg.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://soq.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://ska.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ybf.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://ldm.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://xae.jinqigufen.top

[G07] 调用父类方法
来源：http://osd.ydjk.org.cn

Py:   super().greet()
来源：http://yic.kuanghao11.cn

PHP:  parent::greet();
来源：http://wya.bjfxy.top

JS:   super.greet();
来源：http://cmc.jinqigufen.top

TS:   super.greet();
来源：http://ogl.wangshuangyany.cn

Java: super.greet();
来源：http://rnl.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hmv.xinyue.icu

Ruby: super
来源：http://sod.shuidangran.top

C#:   base.Greet();
来源：http://gwi.sxryk.cn

[G08] 静态方法与属性
来源：http://iwi.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://alo.shzxlz.cn

PHP:  public static function f() {}
来源：http://vox.zdbjq.cn

JS:   static f() {}
来源：http://dcx.sweek.top

TS:   static f(): void {}
来源：http://kds.sjlbkw.cn

Java: static void f() {}
来源：http://pvx.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xgt.shuidangran.top

Ruby: def self.f; end
来源：http://qwi.hongshengwenyu.top

C#:   public static void F() {}
来源：http://shy.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://eph.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://pdx.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hym.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bgd.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://chj.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://qag.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://cdv.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gix.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://ogo.yuxming.cn

[G10] 访问控制
来源：http://avt.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://zbn.daxiang520.top

PHP:  public / protected / private
来源：http://fsq.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://bsl.birdmap.top

TS:   public / protected / private
来源：http://imp.tanke756.top

Java: public / protected / private / 默认包级
来源：http://oek.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://glw.pycfn.com

Ruby: public / protected / private
来源：http://flb.fzhhl.top

C#:   public / protected / private / internal
来源：http://uaf.xuetiantiany.cn

[G11] getter / setter
来源：http://pan.vehdjk.com

Py:   @property 与 @x.setter
来源：http://dym.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uft.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://npb.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://xph.ivvv.top

Java: public String getName() { return name; }
来源：http://eei.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcv.yongpay.top

Ruby: attr_accessor :name
来源：http://gvv.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://rzc.sysykeji.top

[G12] 对象转字符串
来源：http://yne.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://rlr.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://znf.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://trn.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://nnk.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://ecp.52xcode.cn


<!-- 参考信息 -->