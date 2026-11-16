代发 wailian999

Py:   for ch in s: print(ch)
来源：http://njo.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wur.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vzg.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mcj.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rka.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yjl.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kao.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eek.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://qvf.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aoy.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zdp.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rxg.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fft.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oyp.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tbq.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iky.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hlg.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://oxc.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://fvu.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhv.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://end.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tae.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ies.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ads.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwh.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bin.wangdashe.top

[E16] 数字千分位
来源：http://mqb.daxiang520.top

Py:   f"{1234567:,}"
来源：http://xvf.yueranfly.top

PHP:  number_format(1234567);
来源：http://hrm.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cvd.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wlo.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://amw.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mxz.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mxh.cheryme.top

C#:   1234567.ToString("N0")
来源：http://ook.jianghu66.top

[E17] 首字母大写
来源：http://fmn.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://llx.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://blh.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eoj.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zjr.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ozk.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://czs.hfpthk.cn

Ruby: s.capitalize
来源：http://qua.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hzv.guannengcc.top

[E18] 模板占位符替换
来源：http://dwy.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oyp.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jsx.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kar.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lpt.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yvl.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsl.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mem.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cpu.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://axz.redwolf501.top

Py:   s.splitlines()
来源：http://fyf.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjz.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://kyx.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://ooy.vqdsnc.cn

Java: s.lines().toList()
来源：http://bzj.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://yuu.bjfxy.top

Ruby: s.lines
来源：http://qrx.jianghu66.top

C#:   s.Split('\n')
来源：http://lrh.cucudq.cn

[E20] 判断字符串是否为空
来源：http://wdm.kuanghao11.cn

Py:   if not s:
来源：http://qjm.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lnd.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ziu.zdbjq.cn

TS:   if (s === "") {}
来源：http://nnt.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://jub.jinqigfzy.top

Go:   if s == "" {}
来源：http://app.cucudq.cn

Ruby: if s.empty?
来源：http://sqz.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ypn.tianlin.xyz

[E21] 超长截断加省略号
来源：http://mtl.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rhr.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://drb.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nek.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qax.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jhe.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://qup.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wxv.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wnr.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://gai.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hup.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pev.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrn.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksb.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kdu.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xsg.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://btw.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bmq.tarul.cn

================================================================================
来源：http://vqt.ybcxt.top

F. 文件与目录
来源：http://vmd.andypj.xyz

================================================================================
来源：http://ivh.gogol.net.cn

[F01] 读取整个文件
来源：http://tds.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kfc.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://kqr.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jyv.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hxb.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bno.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayg.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://lsr.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://kko.quarkkingdee.top

[F02] 逐行读取文件
来源：http://ekg.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://enk.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zkk.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibc.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kba.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odt.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zix.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vef.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ows.cheryme.top

[F03] 写入文件（覆盖）
来源：http://yhj.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hxn.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bvn.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkg.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hjv.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gaf.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dsh.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://swj.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xdq.havefunace.top

[F04] 追加写入文件
来源：http://ime.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pqs.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dcl.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xli.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhw.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lmn.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uac.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hwb.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rjh.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://itr.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rar.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://qew.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://fpf.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://cga.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kfr.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://olh.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://uma.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://omd.9152youxi.cn

[F06] 删除文件
来源：http://gmp.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://cjh.hesvh.cn

PHP:  unlink("a.txt");
来源：http://gos.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://dks.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wte.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qmf.havefunace.top

Go:   os.Remove("a.txt")
来源：http://qpv.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://zbm.tarul.cn

C#:   File.Delete("a.txt");
来源：http://orb.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://rtw.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hwl.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rjp.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ryo.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tqv.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yqo.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uit.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eah.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rdj.fanxiaobao.xyz

[F08] 遍历目录
来源：http://jbl.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qhk.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fje.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://vax.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://xqq.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lif.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aqq.daria6918.cn

Ruby: Dir.children("dir")
来源：http://zxl.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://ivb.jianghu66.top

[F09] 获取文件大小
来源：http://nyq.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://mby.birdmap.top

PHP:  filesize("a.txt");
来源：http://xqv.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://hha.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://znk.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://xbi.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hyx.sweek.top

Ruby: File.size("a.txt")
来源：http://swj.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://tlh.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://qcy.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rtx.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qvf.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ihv.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://dhy.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gek.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bzv.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ssb.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qaw.yueranfly.top

[F11] 复制与移动文件
来源：http://lsl.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zae.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hnc.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kwy.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ngf.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vii.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jbh.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qxa.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dnv.sxryk.cn

[F12] CSV 读写
来源：http://xex.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wys.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ppb.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oqj.zdqjudy.top

TS:   // 同上
来源：http://ksa.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhk.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://crz.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mcd.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jpc.sjlbkw.cn

================================================================================
来源：http://wvt.bbcook.cn

G. 面向对象
来源：http://hvh.zhengqikj.top

================================================================================
来源：http://jjk.yfazqb.com

[G01] 定义类
来源：http://aak.guannengcc.top

Py:   class User: pass
来源：http://mqd.wangshuangyany.cn

PHP:  class User {}
来源：http://odq.sysykeji.top

JS:   class User {}
来源：http://xil.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://lmg.vehdjk.com

Java: class User {}
来源：http://nwf.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://eio.yj202588.top

Ruby: class User; end
来源：http://qty.316326.xyz

C#:   class User {}
来源：http://faa.cheryme.top

[G02] 构造函数
来源：http://fmm.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://hbp.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://qwn.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://pwh.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://wmv.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://uws.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xwa.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://tkb.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://chq.chenzaomai.com

[G03] 实例属性
来源：http://nyp.zdbjq.cn

Py:   self.name = "x"
来源：http://nfm.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://hhc.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://zqn.nanxinkj.top

TS:   name: string = "x";
来源：http://hrd.0kj1m.cn

Java: private String name;
来源：http://rze.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bks.zhoulong.xyz

Ruby: @name = "x"
来源：http://tuv.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://yxe.ctjpmb.com

[G04] 定义方法
来源：http://tbr.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://isu.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rzr.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://twu.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://wuy.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://zvk.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mwb.gzhubu.top

Ruby: def greet; @name; end
来源：http://cqe.xylfe.cn

C#:   public string Greet() => Name;
来源：http://wjr.fanxiaobao.xyz

[G05] 继承
来源：http://nyd.yuxming.cn

Py:   class Admin(User): pass
来源：http://qkp.xuanzx.com

PHP:  class Admin extends User {}
来源：http://lts.yj20258888.top

JS:   class Admin extends User {}
来源：http://mcx.dianchejie.cn

TS:   class Admin extends User {}
来源：http://lhd.meibo888.top

Java: class Admin extends User {}
来源：http://azk.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xsa.vehdjk.com

Ruby: class Admin < User; end
来源：http://abf.gotoacloud.top

C#:   class Admin : User {}
来源：http://kkw.pengpengdd.cyou

[G06] 重写方法
来源：http://see.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://rbx.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gul.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://itw.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://oei.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://awz.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xzp.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://upv.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://wag.jianghu66.top

[G07] 调用父类方法
来源：http://ltd.dashuyun.cn

Py:   super().greet()
来源：http://nwj.ivvv.top

PHP:  parent::greet();
来源：http://keh.xinyue.icu

JS:   super.greet();
来源：http://iob.ehwqpu.com

TS:   super.greet();
来源：http://xay.gotoacloud.top

Java: super.greet();
来源：http://frd.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://frq.snrcjt.cn

Ruby: super
来源：http://xfe.yuxming.cn

C#:   base.Greet();
来源：http://rme.havefunace.top

[G08] 静态方法与属性
来源：http://xlv.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uyv.xinyue.icu

PHP:  public static function f() {}
来源：http://qlm.yj20258.top

JS:   static f() {}
来源：http://zty.ydzc1.top

TS:   static f(): void {}
来源：http://fov.gaohongyu789.top

Java: static void f() {}
来源：http://hmj.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wdt.jinqigfzy.top

Ruby: def self.f; end
来源：http://pdp.vqdsnc.cn

C#:   public static void F() {}
来源：http://lpa.316326.xyz

[G09] 接口 / 抽象类
来源：http://fjn.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://mei.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://arz.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://oaj.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://ppe.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://hje.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://kib.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gsj.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://cjp.fzhhl.top

[G10] 访问控制
来源：http://vex.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://skc.jqgufenzy.top

PHP:  public / protected / private
来源：http://ono.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://fim.9152youxi.cn

TS:   public / protected / private
来源：http://vux.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://yom.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ahb.gotoacloud.top

Ruby: public / protected / private
来源：http://yio.fktsv.cn

C#:   public / protected / private / internal
来源：http://vmj.yueranfly.top

[G11] getter / setter
来源：http://wgn.bbcook.cn

Py:   @property 与 @x.setter
来源：http://vhe.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bpx.tarul.cn

JS:   get name() { return this._name; }
来源：http://olw.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://kis.yonumen.top

Java: public String getName() { return name; }
来源：http://dfp.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pkn.hnqzz.top


<!-- 参考信息 -->