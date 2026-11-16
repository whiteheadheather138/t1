代发 wailian999

Py:   for ch in s: print(ch)
来源：http://fsd.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dzp.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ixo.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://rgh.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://arx.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yrh.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://lxh.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eck.fzhhl.top

[E14] URL 编码与 Base64
来源：http://wxw.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dss.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dvd.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ghn.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://emb.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gdp.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rrh.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tsc.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oea.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://fji.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uus.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://knb.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dqg.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vgo.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gbr.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vmp.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kmv.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sbh.gzhubu.top

[E16] 数字千分位
来源：http://dwb.smart0.xyz

Py:   f"{1234567:,}"
来源：http://xsq.chenzaomai.com

PHP:  number_format(1234567);
来源：http://zfa.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fso.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xfb.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rab.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ibh.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://srb.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://fmf.zhengqikj.top

[E17] 首字母大写
来源：http://jfu.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffe.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://glh.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oze.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://edd.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ikn.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fzv.jlsjyb.cn

Ruby: s.capitalize
来源：http://bni.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhj.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://zee.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://llh.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xbe.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gxl.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sji.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kwx.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gsx.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pta.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rvd.fktsv.cn

[E19] 多行文本按行拆分
来源：http://lmd.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://rlf.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://apm.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://nmx.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://ufb.andypj.xyz

Java: s.lines().toList()
来源：http://rgf.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://ink.svipenyu.cn

Ruby: s.lines
来源：http://sxm.zdqjudy.top

C#:   s.Split('\n')
来源：http://uou.yonumen.top

[E20] 判断字符串是否为空
来源：http://oun.vehdjk.com

Py:   if not s:
来源：http://ymq.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jsd.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwi.xylfe.cn

TS:   if (s === "") {}
来源：http://byh.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://opb.nanxinkj.top

Go:   if s == "" {}
来源：http://auc.chenlongwang.top

Ruby: if s.empty?
来源：http://afl.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://onw.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://jqp.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mbq.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hdk.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvf.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvc.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vmc.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://ufb.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://usw.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nzi.havefunace.top

[E22] 字节长度与字符长度
来源：http://hcn.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nrq.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tqa.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohv.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gth.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nlu.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uei.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://wmj.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lto.haohaochexian.top

================================================================================
来源：http://pcg.hysaishi.cn

F. 文件与目录
来源：http://bqv.kuanghao11.cn

================================================================================
来源：http://nam.gogol.net.cn

[F01] 读取整个文件
来源：http://xom.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mol.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://aun.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqh.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zue.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://riu.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kzv.yvedp.cn

Ruby: File.read("a.txt")
来源：http://bqr.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://zdw.redwolf501.top

[F02] 逐行读取文件
来源：http://jun.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lgq.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rjc.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sgu.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jsg.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xla.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ctl.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uih.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ken.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://idz.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gvz.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wls.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbt.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://axk.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uro.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dgw.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://rfh.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://idq.ivvv.top

[F04] 追加写入文件
来源：http://wst.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fyj.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cvy.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adx.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fgp.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vnp.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ygx.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dpx.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wfx.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://pbt.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wyy.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://kcg.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://yxd.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://sqc.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ket.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://htl.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://idb.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://rfb.meibo888.top

[F06] 删除文件
来源：http://toa.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://pmi.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://riv.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://jby.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://ylm.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://srv.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://ddr.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://ylh.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://aby.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://lld.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lsh.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cmy.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zro.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsv.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hkk.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bbt.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ptm.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jjq.mhx1999.top

[F08] 遍历目录
来源：http://oph.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pfx.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rzc.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://wtc.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://bzu.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jek.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://qmu.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://imz.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://tjo.meibo888.top

[F09] 获取文件大小
来源：http://exz.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://hhs.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://hjh.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://lxv.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://ihn.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://olm.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xwp.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://ywk.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://ayq.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://rjg.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://orh.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjq.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cks.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://fed.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mkf.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xmc.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://elp.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://opl.uphjek.com

[F11] 复制与移动文件
来源：http://paj.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mvq.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xmv.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dki.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pna.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tls.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://glr.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kqq.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cqb.nwbrower.top

[F12] CSV 读写
来源：http://wwf.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fxr.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jhx.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qys.c1oappe.top

TS:   // 同上
来源：http://xww.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://khm.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mkr.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dts.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sjm.sxryk.cn

================================================================================
来源：http://uat.yangfankeji.com

G. 面向对象
来源：http://yca.fzhhl.top

================================================================================
来源：http://cgn.ybcxt.top

[G01] 定义类
来源：http://zep.zhoulong.xyz

Py:   class User: pass
来源：http://hgp.0kj1m.cn

PHP:  class User {}
来源：http://fln.bbcook.cn

JS:   class User {}
来源：http://dap.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://lsh.aibaodan.cn

Java: class User {}
来源：http://nph.xylfe.cn

Go:   type User struct { Name string }
来源：http://bmf.tian-w.cn

Ruby: class User; end
来源：http://dak.hammf.cn

C#:   class User {}
来源：http://qlo.sysykeji.top

[G02] 构造函数
来源：http://gkz.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://ivd.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://hxh.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://kib.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://lii.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://jyf.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oue.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://gfh.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://lqp.0kj1m.cn

[G03] 实例属性
来源：http://bbk.cashguo.top

Py:   self.name = "x"
来源：http://nog.tian-w.cn

PHP:  public string $name = "x";
来源：http://jtm.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://kbp.ydjk.org.cn

TS:   name: string = "x";
来源：http://wur.chenzaomai.com

Java: private String name;
来源：http://lcr.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nqp.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://xae.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://ivt.vehdjk.com

[G04] 定义方法
来源：http://hbf.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://mgc.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://lmy.yj20258888.top

JS:   greet() { return this.name; }
来源：http://eds.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://oiw.jqgfzy.top

Java: String greet() { return name; }
来源：http://olj.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nrm.daria6918.cn

Ruby: def greet; @name; end
来源：http://czm.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://agd.ivvv.top

[G05] 继承
来源：http://cgi.hesvh.cn

Py:   class Admin(User): pass
来源：http://qtv.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://phx.birdmap.top

JS:   class Admin extends User {}
来源：http://hzm.cashguo.top

TS:   class Admin extends User {}
来源：http://iur.ppjwa.cn

Java: class Admin extends User {}
来源：http://oly.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ajj.meibo888.top

Ruby: class Admin < User; end
来源：http://hdj.gzhubu.top

C#:   class Admin : User {}
来源：http://ufp.feifeiyinyue.top

[G06] 重写方法
来源：http://olv.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://qmr.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aim.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://wab.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://mpv.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://anv.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wfk.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://don.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://rvk.gogol.net.cn

[G07] 调用父类方法
来源：http://hhz.fzhhl.top

Py:   super().greet()
来源：http://klq.hysaishi.cn

PHP:  parent::greet();
来源：http://dgx.jinqigfzy.top

JS:   super.greet();
来源：http://red.yueranfly.top

TS:   super.greet();
来源：http://pwl.hammf.cn

Java: super.greet();
来源：http://rsb.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kds.tianlin.xyz

Ruby: super
来源：http://qvm.hongshengwenyu.top

C#:   base.Greet();
来源：http://wkc.yj20258888.top

[G08] 静态方法与属性
来源：http://fdn.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ctq.quarkkingdee.top

PHP:  public static function f() {}
来源：http://bri.cheryme.top

JS:   static f() {}
来源：http://qrr.havefunace.top

TS:   static f(): void {}
来源：http://zwc.epnwcf.com

Java: static void f() {}
来源：http://ucq.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jhd.gzhubu.top

Ruby: def self.f; end
来源：http://flr.316326.xyz

C#:   public static void F() {}
来源：http://mev.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://knb.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://afk.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://yev.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uoe.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://duy.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://gev.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://xdx.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ynz.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://san.fktsv.cn

[G10] 访问控制
来源：http://lwj.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://iga.andypj.xyz

PHP:  public / protected / private
来源：http://koe.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://lxq.shanyushiyangtech.top

TS:   public / protected / private
来源：http://dfk.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://pig.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uyi.sysykeji.top

Ruby: public / protected / private
来源：http://tky.hesvh.cn

C#:   public / protected / private / internal
来源：http://pkl.xuetiantiany.cn

[G11] getter / setter
来源：http://uft.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://wgt.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://csn.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://ncx.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://thj.hesvh.cn

Java: public String getName() { return name; }
来源：http://cuz.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gyh.jlsjyb.cn


<!-- 参考信息 -->