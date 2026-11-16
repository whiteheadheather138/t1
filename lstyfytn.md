代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rko.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jsv.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ejc.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jhz.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yyu.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://fpi.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ous.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vgy.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ojz.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://fln.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ssq.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxe.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jpr.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ubp.xylfe.cn

[E16] 数字千分位
来源：http://xym.yonumen.top

Py:   f"{1234567:,}"
来源：http://gqk.xylfe.cn

PHP:  number_format(1234567);
来源：http://nhe.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qkc.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mnl.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ord.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbg.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lpe.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://rvo.cucudq.cn

[E17] 首字母大写
来源：http://jqg.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gpa.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xzt.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rnk.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcv.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gfv.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qeh.xinyue.icu

Ruby: s.capitalize
来源：http://zqy.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qet.quarkkingdee.top

[E18] 模板占位符替换
来源：http://ibp.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zxl.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uyt.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://wyb.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wlz.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://npz.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rnt.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xpc.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gsj.tian-w.cn

[E19] 多行文本按行拆分
来源：http://jzk.jqgufenzy.top

Py:   s.splitlines()
来源：http://bzm.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tbl.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://lzu.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://kza.shangyingyoupin.top

Java: s.lines().toList()
来源：http://wwc.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://bay.cheryme.top

Ruby: s.lines
来源：http://ink.guowangkeji.top

C#:   s.Split('\n')
来源：http://jxt.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://lke.guannengcc.top

Py:   if not s:
来源：http://cdp.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oju.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rwq.sufxvd.cn

TS:   if (s === "") {}
来源：http://acc.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://jhs.52xcode.cn

Go:   if s == "" {}
来源：http://rdn.feifeiyinyue.top

Ruby: if s.empty?
来源：http://drr.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qoq.ehwqpu.com

[E21] 超长截断加省略号
来源：http://ujj.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fqa.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lgm.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdk.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pag.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nzx.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://qkm.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kdb.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xkz.andypj.xyz

[E22] 字节长度与字符长度
来源：http://hpu.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzv.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ukw.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mgn.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jlb.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iuo.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ona.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://cjx.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vsg.zdqjudy.top

================================================================================
来源：http://nma.xinyue.icu

F. 文件与目录
来源：http://uli.zycfv.cn

================================================================================
来源：http://qtx.yuanzhike.top

[F01] 读取整个文件
来源：http://qry.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cgm.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://qps.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://krq.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fyf.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fwz.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ykx.ybcxt.top

Ruby: File.read("a.txt")
来源：http://jpq.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://gdf.yanxiufei.cn

[F02] 逐行读取文件
来源：http://rxu.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://khm.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imo.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shg.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wcw.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dej.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://stp.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fik.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dcj.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://yge.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rky.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nlg.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fiq.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oko.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ued.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lqb.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://fpe.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://syy.cashguo.top

[F04] 追加写入文件
来源：http://rgb.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rat.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vwe.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osp.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yuf.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nyr.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qxa.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xoo.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dlk.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://tzx.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rlg.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://qca.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://bwf.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hza.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ntf.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://shy.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://jgr.pycfn.com

C#:   File.Exists("a.txt")
来源：http://xbw.hywenlv.cn

[F06] 删除文件
来源：http://prt.nwbrower.top

Py:   os.remove("a.txt")
来源：http://ofm.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://acr.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://mmm.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://gva.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vbv.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://gdp.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://wee.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://ids.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://kqf.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwt.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qna.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lhu.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyb.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfi.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zmg.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jxx.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hpy.vehdjk.com

[F08] 遍历目录
来源：http://oom.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://avs.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fmx.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://ayx.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://fot.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eki.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ibm.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://oqz.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://ndh.zhongyouzk.top

[F09] 获取文件大小
来源：http://wvw.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://swh.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://umk.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://jxl.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://lea.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://zlc.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sqn.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://ntm.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://rbl.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://nlb.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvs.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wzp.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://okm.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://dxp.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xfx.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://frx.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ype.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://adn.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://adt.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dqo.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dbb.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rnl.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gaq.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wcl.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://frc.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jip.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://acu.cashguo.top

[F12] CSV 读写
来源：http://wvm.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pwy.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wcs.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vch.jqgufenzy.top

TS:   // 同上
来源：http://mjw.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://byd.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bfx.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jkv.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uqo.ctjpmb.com

================================================================================
来源：http://uys.cqqwz.cn

G. 面向对象
来源：http://oao.daxiang520.top

================================================================================
来源：http://gdf.bjfxy.top

[G01] 定义类
来源：http://yhk.xziqi.cn

Py:   class User: pass
来源：http://jaw.shangyingyoupin.top

PHP:  class User {}
来源：http://sbw.svipenyu.cn

JS:   class User {}
来源：http://qms.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://qqc.gaohongyu789.top

Java: class User {}
来源：http://ino.yvedp.cn

Go:   type User struct { Name string }
来源：http://xeg.hcnkem.com

Ruby: class User; end
来源：http://pcw.hnxiangtu.top

C#:   class User {}
来源：http://flt.fengsongda.top

[G02] 构造函数
来源：http://imn.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://yjd.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://sff.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://ynq.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://lrd.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://wlc.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kyg.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://khq.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://upv.jyoumei.cn

[G03] 实例属性
来源：http://xnk.sysykeji.top

Py:   self.name = "x"
来源：http://zqr.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://xno.fzhhl.top

JS:   this.name = "x";
来源：http://bdz.gogol.net.cn

TS:   name: string = "x";
来源：http://szs.aibaodan.cn

Java: private String name;
来源：http://mdi.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rvy.hongshengwenyu.top

Ruby: @name = "x"
来源：http://nld.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://zmb.cashguo.top

[G04] 定义方法
来源：http://str.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://ben.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://upf.yonumen.top

JS:   greet() { return this.name; }
来源：http://eiv.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://svr.hcnkem.com

Java: String greet() { return name; }
来源：http://izz.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ghu.epnwcf.com

Ruby: def greet; @name; end
来源：http://rfh.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://zpb.xingfuxueyuan.xyz

[G05] 继承
来源：http://lxn.hnqzz.top

Py:   class Admin(User): pass
来源：http://ofk.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://yzk.xylfe.cn

JS:   class Admin extends User {}
来源：http://slh.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://nee.gogol.net.cn

Java: class Admin extends User {}
来源：http://pfd.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hbr.cdnleiting.top

Ruby: class Admin < User; end
来源：http://ufb.vqdsnc.cn

C#:   class Admin : User {}
来源：http://qul.sufxvd.cn

[G06] 重写方法
来源：http://pka.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://xto.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bfy.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://fey.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://hcs.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://nfm.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ljj.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://xbz.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://zhy.nanxinkj.top

[G07] 调用父类方法
来源：http://nuu.jinqigufen.top

Py:   super().greet()
来源：http://kme.yj202588.top

PHP:  parent::greet();
来源：http://nxo.wangshuangyany.cn

JS:   super.greet();
来源：http://ukg.ppjwa.cn

TS:   super.greet();
来源：http://zih.tarul.cn

Java: super.greet();
来源：http://son.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xfm.cashguo.top

Ruby: super
来源：http://sak.zhixingplan.top

C#:   base.Greet();
来源：http://tpt.redwolf501.top

[G08] 静态方法与属性
来源：http://mey.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bst.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://oul.chenlongwang.top

JS:   static f() {}
来源：http://zls.hywenlv.cn

TS:   static f(): void {}
来源：http://syr.jyoumei.cn

Java: static void f() {}
来源：http://dsl.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://urw.ivvv.top

Ruby: def self.f; end
来源：http://bet.jinqigfzy.top

C#:   public static void F() {}
来源：http://mcu.shuidangran.top

[G09] 接口 / 抽象类
来源：http://wve.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://cnn.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://hek.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://djv.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://lxh.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://gey.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://hhh.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://joe.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://auc.fehbvm.com

[G10] 访问控制
来源：http://zbt.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://jje.ppjwa.cn

PHP:  public / protected / private
来源：http://okp.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://oir.jqgfzy.top

TS:   public / protected / private
来源：http://qjf.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://izi.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tji.tian-w.cn

Ruby: public / protected / private
来源：http://dvj.hfpthk.cn

C#:   public / protected / private / internal
来源：http://gvi.zhixingplan.top

[G11] getter / setter
来源：http://ibv.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://dqq.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ior.mhx1999.top

JS:   get name() { return this._name; }
来源：http://vzt.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://tlj.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://qib.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ncf.jianghu66.top

Ruby: attr_accessor :name
来源：http://liu.tarul.cn

C#:   public string Name { get; set; }
来源：http://zsa.wangdashe.top

[G12] 对象转字符串
来源：http://ciy.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://guy.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://fqz.smart0.xyz

JS:   toString() { return this.name; }
来源：http://ayy.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://bfc.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://srh.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://ocl.xylfe.cn

Ruby: def to_s; @name; end
来源：http://wbv.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://wxd.yongpay.top

[G13] 判断对象类型
来源：http://hne.316326.xyz


<!-- 参考信息 -->