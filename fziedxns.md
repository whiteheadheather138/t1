代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hcx.nanxuanxn.top

Ruby: s.count("a")
来源：http://alh.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://rzv.ctjpmb.com

[E13] 逐字符遍历
来源：http://rdy.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://gws.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mxw.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rxr.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://qga.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lxt.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wre.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xcf.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gsd.bjfxy.top

[E14] URL 编码与 Base64
来源：http://hcm.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://izt.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bqt.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://irl.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qgi.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ugz.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vwi.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zxb.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqt.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://lkl.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://waw.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hcq.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://okp.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nom.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lie.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fyf.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ofh.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gnf.fzhhl.top

[E16] 数字千分位
来源：http://xup.uphjek.com

Py:   f"{1234567:,}"
来源：http://tke.tianlin.xyz

PHP:  number_format(1234567);
来源：http://vck.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vyk.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kbp.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fys.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ibt.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwu.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://wvn.jianghu66.top

[E17] 首字母大写
来源：http://vbd.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wzn.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aab.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqu.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ijs.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hoy.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzi.zhiwuduotai.top

Ruby: s.capitalize
来源：http://dvx.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lfc.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://yvc.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://juw.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dkc.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gqt.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hhy.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hgr.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gdb.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://inh.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzt.tarul.cn

[E19] 多行文本按行拆分
来源：http://dbb.sweek.top

Py:   s.splitlines()
来源：http://cxd.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iox.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://fxw.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://tjf.shzxlz.cn

Java: s.lines().toList()
来源：http://yjs.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://nsd.chenzaomai.com

Ruby: s.lines
来源：http://bmw.guannengcc.top

C#:   s.Split('\n')
来源：http://vlo.iojbl.cn

[E20] 判断字符串是否为空
来源：http://xol.ydzc1.top

Py:   if not s:
来源：http://zyc.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://twq.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://utr.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://ugy.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://bwe.yuxming.cn

Go:   if s == "" {}
来源：http://hkl.sufxvd.cn

Ruby: if s.empty?
来源：http://dad.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tra.aizwys.cn

[E21] 超长截断加省略号
来源：http://qwh.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ppv.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cde.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsm.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nho.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jwc.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://mcx.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vth.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://grb.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://cgb.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yis.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugs.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlg.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fal.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gnm.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dgr.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://ijx.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kjc.birdmap.top

================================================================================
来源：http://xkz.yangfankeji.com

F. 文件与目录
来源：http://fqy.daxiang520.top

================================================================================
来源：http://fqv.hcnkem.com

[F01] 读取整个文件
来源：http://iuk.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ahx.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://uxu.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ohs.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tjd.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hkn.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vji.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://sjy.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://jve.chenzaomai.com

[F02] 逐行读取文件
来源：http://lbb.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zka.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xlc.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ows.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wcj.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://upd.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wmi.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lgs.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dgk.ivvv.top

[F03] 写入文件（覆盖）
来源：http://coq.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ant.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ljq.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxa.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zve.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zww.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hzn.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ipw.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xcn.shzxlz.cn

[F04] 追加写入文件
来源：http://bif.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dyg.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cba.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ezu.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyd.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gzk.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oow.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hgf.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yuk.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://fxv.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zac.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://nau.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://ecz.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://brz.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://bxf.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pgk.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://ldh.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://acc.zdbjq.cn

[F06] 删除文件
来源：http://fma.hnqzz.top

Py:   os.remove("a.txt")
来源：http://lbr.xinyue.icu

PHP:  unlink("a.txt");
来源：http://plx.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://iwc.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yqt.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oid.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://lba.tarul.cn

Ruby: File.delete("a.txt")
来源：http://hrp.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://mfp.tarul.cn

[F07] 创建目录（含多级）
来源：http://fxf.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pcm.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hdw.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myh.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjw.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tba.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://abj.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mvm.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bdo.yuanzhike.top

[F08] 遍历目录
来源：http://riy.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lhl.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://suf.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://ron.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://qgf.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bfi.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eeg.hnqzz.top

Ruby: Dir.children("dir")
来源：http://skm.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://uhd.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://gjx.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://vir.daxiang520.top

PHP:  filesize("a.txt");
来源：http://yec.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://dji.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://ykj.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lgx.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qgi.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://ssm.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://gem.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://gvb.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jjo.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lwa.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mbp.jianghu66.top

TS:   path.extname("a.txt")
来源：http://lng.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://inn.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://udg.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rjb.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yly.daxiang520.top

[F11] 复制与移动文件
来源：http://ymj.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pll.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twc.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwz.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rps.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jcq.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iuj.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://omz.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wyi.dashuyun.cn

[F12] CSV 读写
来源：http://qcd.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wup.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dmt.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgh.dianchejie.cn

TS:   // 同上
来源：http://qqb.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hel.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xvk.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jxd.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rxa.jqgfzy.top

================================================================================
来源：http://mrd.yonumen.top

G. 面向对象
来源：http://rld.jianghu66.top

================================================================================
来源：http://jyo.chenlongwang.top

[G01] 定义类
来源：http://hil.xuetiantiany.cn

Py:   class User: pass
来源：http://her.gaohongyu789.top

PHP:  class User {}
来源：http://awa.quarkkingdee.top

JS:   class User {}
来源：http://nde.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://rca.zdqjudy.top

Java: class User {}
来源：http://xbs.ehwqpu.com

Go:   type User struct { Name string }
来源：http://khk.yj20258.top

Ruby: class User; end
来源：http://cxi.zhixingplan.top

C#:   class User {}
来源：http://jfw.tarul.cn

[G02] 构造函数
来源：http://gmd.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://oyz.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://duq.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://wge.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://otc.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://pbz.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqc.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://lye.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://eqc.hcnkem.com

[G03] 实例属性
来源：http://zqr.cqqwz.cn

Py:   self.name = "x"
来源：http://far.guannengcc.top

PHP:  public string $name = "x";
来源：http://kim.sysykeji.top

JS:   this.name = "x";
来源：http://xqj.ydzc1.top

TS:   name: string = "x";
来源：http://fne.kuanghao11.cn

Java: private String name;
来源：http://xzm.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fsr.mhx1999.top

Ruby: @name = "x"
来源：http://jve.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://mcg.chenzaomai.com

[G04] 定义方法
来源：http://hun.hammf.cn

Py:   def greet(self): return self.name
来源：http://tkg.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wfr.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://hcf.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://obm.zhixingplan.top

Java: String greet() { return name; }
来源：http://peg.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nfm.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://mda.yj20258.top

C#:   public string Greet() => Name;
来源：http://rkg.ctjpmb.com

[G05] 继承
来源：http://nma.meibo888.top

Py:   class Admin(User): pass
来源：http://dol.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://gfd.gotoacloud.top

JS:   class Admin extends User {}
来源：http://oui.mhx1999.top

TS:   class Admin extends User {}
来源：http://nwt.dashuyun.cn

Java: class Admin extends User {}
来源：http://xan.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rpw.52xcode.cn

Ruby: class Admin < User; end
来源：http://acu.cheryme.top

C#:   class Admin : User {}
来源：http://vdz.yuanzhike.top

[G06] 重写方法
来源：http://qim.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://zzl.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kfv.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://vhh.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://ouh.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://anh.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://brv.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://uum.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://msp.mhx1999.top

[G07] 调用父类方法
来源：http://avf.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://nhc.havefunace.top

PHP:  parent::greet();
来源：http://emz.cashguo.top

JS:   super.greet();
来源：http://jbw.epnwcf.com

TS:   super.greet();
来源：http://idn.jianghu66.top

Java: super.greet();
来源：http://wie.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://irn.316326.xyz

Ruby: super
来源：http://qxq.bbcook.cn

C#:   base.Greet();
来源：http://tss.sjlbkw.cn

[G08] 静态方法与属性
来源：http://asm.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xub.fehbvm.com

PHP:  public static function f() {}
来源：http://uzb.ivvv.top

JS:   static f() {}
来源：http://piu.bbcook.cn

TS:   static f(): void {}
来源：http://owe.316326.xyz

Java: static void f() {}
来源：http://ftu.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://efj.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://ryi.birdmap.top

C#:   public static void F() {}
来源：http://dre.jianghu66.top

[G09] 接口 / 抽象类
来源：http://xhm.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://phk.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://fwd.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jsj.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://obt.smart0.xyz

Java: interface Shape { double area(); }
来源：http://cxh.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://uwe.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tzn.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://knh.yvedp.cn

[G10] 访问控制
来源：http://gon.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://qxw.zdqjudy.top

PHP:  public / protected / private
来源：http://wfc.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://chh.jyoumei.cn

TS:   public / protected / private
来源：http://elz.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://wrz.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gem.uphjek.com

Ruby: public / protected / private
来源：http://ebr.pycfn.com

C#:   public / protected / private / internal
来源：http://vvh.aizwys.cn

[G11] getter / setter
来源：http://vck.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://bif.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uan.zhixingplan.top


<!-- 参考信息 -->