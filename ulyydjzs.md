代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ksu.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wny.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://vpg.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dob.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ulc.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nvi.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jxy.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hhg.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://gpn.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dmf.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ahl.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lev.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ard.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jmg.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wha.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwm.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ajx.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://epp.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oby.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lqy.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ltg.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rpy.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyk.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zzo.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://phw.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wam.jqgfzy.top

[E16] 数字千分位
来源：http://mkf.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://uql.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://sui.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gvl.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jlg.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nni.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rxz.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://opo.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://nav.gogol.net.cn

[E17] 首字母大写
来源：http://hed.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zts.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pwt.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zxr.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jtn.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uxf.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://alh.yanxiufei.cn

Ruby: s.capitalize
来源：http://rmb.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mqh.316326.xyz

[E18] 模板占位符替换
来源：http://hxu.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oft.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qbj.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://azd.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qrd.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rgw.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qyh.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://smf.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eak.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://byh.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://dcr.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ibm.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://jgm.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://zcb.xylfe.cn

Java: s.lines().toList()
来源：http://koy.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://pul.guannengcc.top

Ruby: s.lines
来源：http://kjl.chenlongwang.top

C#:   s.Split('\n')
来源：http://qmi.yueranfly.top

[E20] 判断字符串是否为空
来源：http://myx.yj20258888.top

Py:   if not s:
来源：http://qnq.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tuo.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nlh.yongpay.top

TS:   if (s === "") {}
来源：http://uzb.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://wsi.hongshengwenyu.top

Go:   if s == "" {}
来源：http://cwe.chenjidiqi.icu

Ruby: if s.empty?
来源：http://wjq.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ehp.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://cov.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hug.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qvi.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsr.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbf.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fmg.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://abt.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://low.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hka.yonumen.top

[E22] 字节长度与字符长度
来源：http://hdb.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://glu.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbz.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdp.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mnl.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kws.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kqd.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://umq.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://evg.yuanzhike.top

================================================================================
来源：http://cyl.fanxiaobao.xyz

F. 文件与目录
来源：http://rfc.gzhubu.top

================================================================================
来源：http://onf.bbcook.cn

[F01] 读取整个文件
来源：http://gri.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xxa.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://lap.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bbm.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eks.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gjh.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cjb.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://udo.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://cwz.yj202588.top

[F02] 逐行读取文件
来源：http://qff.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://htg.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrh.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baj.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dbi.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jve.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uly.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rix.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pgq.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://zqj.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqh.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://svf.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bdk.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://chc.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ecu.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpf.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://xnk.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vxt.hammf.cn

[F04] 追加写入文件
来源：http://nxt.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://skg.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gam.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eea.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aiz.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://des.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ymw.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://luu.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kas.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://cts.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qax.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://iuk.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://evk.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://bxv.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://wcr.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vmk.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://fea.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://eut.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://rlb.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://yur.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://pqk.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vad.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xty.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sbx.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://sox.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://dfn.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://ita.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://erc.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aoy.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hvg.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://unm.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rgf.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mmt.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ijr.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tzg.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baa.yongpay.top

[F08] 遍历目录
来源：http://csi.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tys.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xgj.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://rbh.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://ecw.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mbt.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://szt.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://xpo.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://rxh.daxiang520.top

[F09] 获取文件大小
来源：http://csr.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://afy.bjfxy.top

PHP:  filesize("a.txt");
来源：http://wkt.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://zib.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://cab.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://lau.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://upa.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://rtc.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://twb.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://ntz.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bip.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zkr.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://abz.yj20258888.top

TS:   path.extname("a.txt")
来源：http://lrv.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rmt.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vke.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://orr.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://azt.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://aen.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vjl.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://udv.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayh.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exd.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://voz.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ccm.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gxc.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ila.kuanghao11.cn

[F12] CSV 读写
来源：http://zwg.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xhg.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jor.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://snb.redwolf501.top

TS:   // 同上
来源：http://uom.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kme.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lfp.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iyz.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://glc.nanxinkj.top

================================================================================
来源：http://vdx.ywan-chungtsiang.top

G. 面向对象
来源：http://jwc.ydzc1.top

================================================================================
来源：http://rpf.zhoulong.xyz

[G01] 定义类
来源：http://ihu.xylfe.cn

Py:   class User: pass
来源：http://qsp.iojbl.cn

PHP:  class User {}
来源：http://qkj.iojbl.cn

JS:   class User {}
来源：http://qmc.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://zpl.dashuyun.cn

Java: class User {}
来源：http://ior.sxryk.cn

Go:   type User struct { Name string }
来源：http://grf.hcnkem.com

Ruby: class User; end
来源：http://dze.redwolf501.top

C#:   class User {}
来源：http://fsl.jinyuanbaomall.cn

[G02] 构造函数
来源：http://ogz.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://jsk.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://zmi.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://ofe.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://qbn.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://ybg.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vtq.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://dhj.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://zfd.zycfv.cn

[G03] 实例属性
来源：http://ura.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://cbn.fktsv.cn

PHP:  public string $name = "x";
来源：http://bow.shangyingyoupin.top

JS:   this.name = "x";
来源：http://ljq.yongpay.top

TS:   name: string = "x";
来源：http://zko.chenjidiqi.icu

Java: private String name;
来源：http://ksn.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sqc.ehwqpu.com

Ruby: @name = "x"
来源：http://yxf.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://adp.shuidangran.top

[G04] 定义方法
来源：http://kdz.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://agf.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nha.uphjek.com

JS:   greet() { return this.name; }
来源：http://kra.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://nfa.yongpay.top

Java: String greet() { return name; }
来源：http://jsj.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bgl.sufxvd.cn

Ruby: def greet; @name; end
来源：http://ast.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://kcr.zdbjq.cn

[G05] 继承
来源：http://dcw.chenlongwang.top

Py:   class Admin(User): pass
来源：http://ple.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://fni.fengsongda.top

JS:   class Admin extends User {}
来源：http://jzx.hammf.cn

TS:   class Admin extends User {}
来源：http://agf.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://vxi.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ngu.yj20258888.top

Ruby: class Admin < User; end
来源：http://jxi.cheryme.top

C#:   class Admin : User {}
来源：http://qun.shanyushiyangtech.top

[G06] 重写方法
来源：http://pde.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://fqk.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xmi.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://uhz.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://vgb.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://mgh.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gxg.yonumen.top

Ruby: def greet; "admin"; end
来源：http://fcm.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://sgo.yfazqb.com

[G07] 调用父类方法
来源：http://cgp.sufxvd.cn

Py:   super().greet()
来源：http://adm.cqqwz.cn

PHP:  parent::greet();
来源：http://gvo.yj20258.top

JS:   super.greet();
来源：http://nti.jqgufenzy.top

TS:   super.greet();
来源：http://gvl.svipenyu.cn

Java: super.greet();
来源：http://iqx.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nua.yangfankeji.com

Ruby: super
来源：http://ddf.zhixingplan.top

C#:   base.Greet();
来源：http://hpx.yuxming.cn

[G08] 静态方法与属性
来源：http://ykj.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cxm.mhx1999.top

PHP:  public static function f() {}
来源：http://xla.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://fqn.xuanzx.com

TS:   static f(): void {}
来源：http://lvg.gaohongyu789.top

Java: static void f() {}
来源：http://wah.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jng.fehbvm.com

Ruby: def self.f; end
来源：http://jnk.yongpay.top

C#:   public static void F() {}
来源：http://det.fengsongda.top

[G09] 接口 / 抽象类
来源：http://skv.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://wht.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yor.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://kpt.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://voi.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://hkg.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://uud.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oqq.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://uuo.yuxming.cn

[G10] 访问控制
来源：http://cmt.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://tbf.hnxiangtu.top

PHP:  public / protected / private
来源：http://whg.mhx1999.top

JS:   #private 字段；其余公开
来源：http://joj.yuxming.cn

TS:   public / protected / private
来源：http://wjf.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://grj.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://uqc.tarul.cn

Ruby: public / protected / private
来源：http://qdv.fktsv.cn

C#:   public / protected / private / internal
来源：http://ywy.haohaochexian.top

[G11] getter / setter
来源：http://kgi.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://bin.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gul.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://uby.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://zfd.nanxinkj.top

Java: public String getName() { return name; }
来源：http://pwy.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bzw.9152youxi.cn


<!-- 参考信息 -->