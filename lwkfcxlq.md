代发 wailian999

Py:   for ch in s: print(ch)
来源：http://gzg.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bhl.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uod.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://doq.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vfv.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mcg.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rbf.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aih.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://bbf.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gtl.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hck.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cow.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ztu.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uis.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wzd.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://amp.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lzk.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://bse.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://axw.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gmb.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mpn.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://cbx.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lgp.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ahq.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kxf.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://owv.gaohongyu789.top

[E16] 数字千分位
来源：http://ddp.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://wea.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://qws.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://esi.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zia.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hqb.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bff.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://siw.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://unr.xinyue.icu

[E17] 首字母大写
来源：http://igm.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfm.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nfo.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://caq.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mvk.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ygc.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gvn.fzhhl.top

Ruby: s.capitalize
来源：http://gvu.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tix.c1oappe.top

[E18] 模板占位符替换
来源：http://hvi.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iud.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vri.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fnh.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uaq.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://psn.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uul.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uqe.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mgs.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://jkv.redwolf501.top

Py:   s.splitlines()
来源：http://qsl.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ezs.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://vti.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://edg.jinqigfzy.top

Java: s.lines().toList()
来源：http://bfw.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://nqo.wangdashe.top

Ruby: s.lines
来源：http://ecb.chenzaomai.com

C#:   s.Split('\n')
来源：http://mcw.fehbvm.com

[E20] 判断字符串是否为空
来源：http://igh.yueranfly.top

Py:   if not s:
来源：http://shp.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgw.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://syz.fengsongda.top

TS:   if (s === "") {}
来源：http://ftx.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://alz.nwbrower.top

Go:   if s == "" {}
来源：http://uun.pycfn.com

Ruby: if s.empty?
来源：http://ldz.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pgs.shuidangran.top

[E21] 超长截断加省略号
来源：http://tik.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://upu.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hij.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bew.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmb.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ckl.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://slh.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cod.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ktl.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://uqt.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fyv.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfp.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvq.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wkn.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://skg.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://imc.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://zkh.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://agp.guannengcc.top

================================================================================
来源：http://zqq.tanke756.top

F. 文件与目录
来源：http://ged.yonumen.top

================================================================================
来源：http://snv.xuetiantiany.cn

[F01] 读取整个文件
来源：http://may.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ssj.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://imn.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://haq.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tfg.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://epb.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tbh.andypj.xyz

Ruby: File.read("a.txt")
来源：http://ahp.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://prg.jqgufenzy.top

[F02] 逐行读取文件
来源：http://nac.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wgf.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fuw.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdz.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ojx.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xaz.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gpz.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vkg.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbn.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://cah.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bki.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kij.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nsm.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zay.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://apg.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mqf.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://cus.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lmr.sysykeji.top

[F04] 追加写入文件
来源：http://tms.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mxd.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxy.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mmr.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fan.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nce.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ooc.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sgh.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mkn.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://dpx.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xue.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://xmo.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://mgm.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://cuq.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://oyz.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bla.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://oxa.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://iwz.ydjk.org.cn

[F06] 删除文件
来源：http://xsd.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://nxa.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://dob.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://rbj.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://mqr.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sic.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://hpr.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://aqd.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://mlp.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://ksr.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xfn.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://htv.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdv.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzl.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xra.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oiu.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cou.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gxq.yanxiufei.cn

[F08] 遍历目录
来源：http://nfw.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qll.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jgm.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://acf.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://ocy.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://snh.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://upr.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://uur.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://flr.tian-w.cn

[F09] 获取文件大小
来源：http://tmp.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://ssq.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://asl.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://uol.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://qmo.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://rmy.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://znh.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://pjo.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://vlg.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://fpq.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xsm.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ckk.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://clz.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://ucz.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvs.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uot.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oea.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gzu.gaohongyu789.top

[F11] 复制与移动文件
来源：http://gin.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lmm.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jju.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hdl.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://krg.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxm.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ypq.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sjt.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kte.daria6918.cn

[F12] CSV 读写
来源：http://zpc.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://flm.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sdc.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gbq.pengpengdd.cyou

TS:   // 同上
来源：http://fvm.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yga.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kql.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hiq.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://qgq.zhaomingkeji.xyz

================================================================================
来源：http://olm.quarkkingdee.top

G. 面向对象
来源：http://znl.quarkkingdee.top

================================================================================
来源：http://vhn.zhijiandao.cn

[G01] 定义类
来源：http://ghc.jinqigfzy.top

Py:   class User: pass
来源：http://unt.gaohongyu789.top

PHP:  class User {}
来源：http://tgj.xylfe.cn

JS:   class User {}
来源：http://qob.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://tqf.zhongyouzk.top

Java: class User {}
来源：http://vxp.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://uar.yfazqb.com

Ruby: class User; end
来源：http://ghy.shuidangran.top

C#:   class User {}
来源：http://bvz.redwolf501.top

[G02] 构造函数
来源：http://icp.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://sxb.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://ocm.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://ftu.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://hvu.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://tsg.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pby.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://chv.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://rcz.zdbjq.cn

[G03] 实例属性
来源：http://vfn.birdmap.top

Py:   self.name = "x"
来源：http://dvd.hysaishi.cn

PHP:  public string $name = "x";
来源：http://zoh.zhoulong.xyz

JS:   this.name = "x";
来源：http://ori.vqdsnc.cn

TS:   name: string = "x";
来源：http://rpa.dashuyun.cn

Java: private String name;
来源：http://btu.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ogj.hfpthk.cn

Ruby: @name = "x"
来源：http://egy.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ybd.tanke756.top

[G04] 定义方法
来源：http://frd.sweek.top

Py:   def greet(self): return self.name
来源：http://hmz.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qvt.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://eys.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://szq.shuidangran.top

Java: String greet() { return name; }
来源：http://lyd.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://bzr.uphjek.com

Ruby: def greet; @name; end
来源：http://ecw.daxiang520.top

C#:   public string Greet() => Name;
来源：http://vjr.zhaomingkeji.xyz

[G05] 继承
来源：http://vsd.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://was.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://vhk.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://krv.yj20258.top

TS:   class Admin extends User {}
来源：http://wyl.hnxiangtu.top

Java: class Admin extends User {}
来源：http://onl.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jsk.xinyue.icu

Ruby: class Admin < User; end
来源：http://svq.quarkkingdee.top

C#:   class Admin : User {}
来源：http://dgj.sufxvd.cn

[G06] 重写方法
来源：http://xmd.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://plo.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://yov.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://hug.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://iwc.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://xwz.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gsw.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://gtn.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://avr.jianghu66.top

[G07] 调用父类方法
来源：http://rho.ppjwa.cn

Py:   super().greet()
来源：http://rsm.gaohongyu789.top

PHP:  parent::greet();
来源：http://zav.fehbvm.com

JS:   super.greet();
来源：http://rag.tanke756.top

TS:   super.greet();
来源：http://hqm.sjlbkw.cn

Java: super.greet();
来源：http://txc.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://slg.jiagoushi.top

Ruby: super
来源：http://eua.meibo888.top

C#:   base.Greet();
来源：http://eei.jiagoushi.top

[G08] 静态方法与属性
来源：http://wmo.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tlk.jinqigfzy.top

PHP:  public static function f() {}
来源：http://vah.feifeiyinyue.top

JS:   static f() {}
来源：http://cmj.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://qio.ppjwa.cn

Java: static void f() {}
来源：http://wxk.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://rgm.tanke756.top

Ruby: def self.f; end
来源：http://jgg.havefunace.top

C#:   public static void F() {}
来源：http://trx.52xcode.cn

[G09] 接口 / 抽象类
来源：http://yul.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://roy.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://dwk.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mog.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://wll.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://vdd.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://upd.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xhq.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://bkx.9152youxi.cn

[G10] 访问控制
来源：http://uoi.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://klh.bbcook.cn

PHP:  public / protected / private
来源：http://rci.xuanzx.com

JS:   #private 字段；其余公开
来源：http://vvn.ydjk.org.cn

TS:   public / protected / private
来源：http://kpi.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://gpm.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://svz.jqgfzy.top

Ruby: public / protected / private
来源：http://yjo.52xcode.cn

C#:   public / protected / private / internal
来源：http://yui.cheryme.top

[G11] getter / setter
来源：http://xwr.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://gpg.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://luf.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://zlv.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://dza.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ett.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ymu.iojbl.cn


<!-- 参考信息 -->