代发 wailian999

Go:   strings.Count(s, "a")
来源：http://kgx.cqqwz.cn

Ruby: s.count("a")
来源：http://nzl.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://vqe.chenlongwang.top

[E13] 逐字符遍历
来源：http://rzw.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://qzj.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hgr.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eop.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lnj.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://krr.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxy.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xpw.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nag.guannengcc.top

[E14] URL 编码与 Base64
来源：http://mka.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://akt.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yae.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ybr.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rci.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vay.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uyv.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fug.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://woi.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://kqs.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rkz.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lsq.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yur.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://heg.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qrx.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fgt.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lki.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mjq.cheryme.top

[E16] 数字千分位
来源：http://kgd.cheryme.top

Py:   f"{1234567:,}"
来源：http://xnx.c1oappe.top

PHP:  number_format(1234567);
来源：http://csz.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gij.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oxc.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://taf.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zon.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lei.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://ftc.yonumen.top

[E17] 首字母大写
来源：http://ncg.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dbq.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mty.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqa.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvb.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ode.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iuq.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://rzc.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zqx.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://pen.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vga.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xlt.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://rdj.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://szn.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lvg.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ldc.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kve.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tbg.cucudq.cn

[E19] 多行文本按行拆分
来源：http://fuk.gzhubu.top

Py:   s.splitlines()
来源：http://kgn.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yys.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://zcj.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://ikf.xziqi.cn

Java: s.lines().toList()
来源：http://tzk.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://cdt.pycfn.com

Ruby: s.lines
来源：http://ojz.yj20258888.top

C#:   s.Split('\n')
来源：http://klj.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://acs.xinyue.icu

Py:   if not s:
来源：http://gme.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jnn.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzr.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://juw.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://uul.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://zyk.vehdjk.com

Ruby: if s.empty?
来源：http://etb.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xaq.hfpthk.cn

[E21] 超长截断加省略号
来源：http://wnt.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ure.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hcr.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://znr.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tta.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uks.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://wxj.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://khf.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xsn.tian-w.cn

[E22] 字节长度与字符长度
来源：http://lus.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mtr.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qpy.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://knj.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xmw.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rll.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aax.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://pqa.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oik.sweek.top

================================================================================
来源：http://kdx.wangdashe.top

F. 文件与目录
来源：http://kfx.feifeiyinyue.top

================================================================================
来源：http://mad.9152youxi.cn

[F01] 读取整个文件
来源：http://zri.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hrj.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://yja.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sui.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uhr.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eze.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kwx.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://huk.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://yry.xuanzx.com

[F02] 逐行读取文件
来源：http://jhe.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yja.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omu.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://flh.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbc.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbc.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tbj.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hor.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://obw.yj202588.top

[F03] 写入文件（覆盖）
来源：http://dod.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jxt.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qdh.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mck.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gmr.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wcz.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://btc.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://pqc.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://amn.52xcode.cn

[F04] 追加写入文件
来源：http://nqf.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://esl.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sio.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twa.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwh.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mqc.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://azb.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://irz.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tvn.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://myh.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xet.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://snd.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://vxh.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://noo.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bqd.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jcb.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://jxl.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://npb.jinyuanbaomall.cn

[F06] 删除文件
来源：http://lqs.nwbrower.top

Py:   os.remove("a.txt")
来源：http://cyr.vehdjk.com

PHP:  unlink("a.txt");
来源：http://vbb.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://qno.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://goz.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gjd.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://aqh.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://kjp.tarul.cn

C#:   File.Delete("a.txt");
来源：http://klh.epnwcf.com

[F07] 创建目录（含多级）
来源：http://jut.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jfw.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nuc.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aas.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqs.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tfv.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cmr.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://flx.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wgt.sxryk.cn

[F08] 遍历目录
来源：http://yux.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kxu.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eof.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://jhw.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://glf.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bws.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ubi.aizwys.cn

Ruby: Dir.children("dir")
来源：http://qpm.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://uka.xinyue.icu

[F09] 获取文件大小
来源：http://mjy.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://xug.bjfxy.top

PHP:  filesize("a.txt");
来源：http://dqf.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://bgf.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://tjr.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kxj.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yhn.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://yhg.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://zne.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://tck.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eqm.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zvq.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dcz.tanke756.top

TS:   path.extname("a.txt")
来源：http://lto.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ktm.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kmw.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uuy.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gfu.yj20258888.top

[F11] 复制与移动文件
来源：http://pyi.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pen.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://meh.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wkm.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfy.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tlq.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gwu.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ttr.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mhl.zhongyouzk.top

[F12] CSV 读写
来源：http://hdh.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zlh.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cdo.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dkf.ivvv.top

TS:   // 同上
来源：http://uqh.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hfv.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ouj.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gxl.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jjj.zhongyouzk.top

================================================================================
来源：http://nwp.mhx1999.top

G. 面向对象
来源：http://aww.xingfuxueyuan.xyz

================================================================================
来源：http://kkl.xingfuxueyuan.xyz

[G01] 定义类
来源：http://ktc.zhiwuduotai.top

Py:   class User: pass
来源：http://dfs.zhongyouzk.top

PHP:  class User {}
来源：http://eru.9152youxi.cn

JS:   class User {}
来源：http://tci.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://gdj.gzhubu.top

Java: class User {}
来源：http://dwj.yongpay.top

Go:   type User struct { Name string }
来源：http://csg.yonumen.top

Ruby: class User; end
来源：http://adw.svipenyu.cn

C#:   class User {}
来源：http://qyp.yj202588.top

[G02] 构造函数
来源：http://asj.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://tjf.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://dmw.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://jyz.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://yow.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://hcv.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ryf.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://sif.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://loc.jinqigufen.top

[G03] 实例属性
来源：http://fbn.kuanghao11.cn

Py:   self.name = "x"
来源：http://fzx.zdqjudy.top

PHP:  public string $name = "x";
来源：http://jrs.guowangkeji.top

JS:   this.name = "x";
来源：http://mrt.uphjek.com

TS:   name: string = "x";
来源：http://gmv.iojbl.cn

Java: private String name;
来源：http://led.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lna.yfazqb.com

Ruby: @name = "x"
来源：http://jfu.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://cju.jqgfzy.top

[G04] 定义方法
来源：http://yiz.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://kgd.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wmg.xuanzx.com

JS:   greet() { return this.name; }
来源：http://orp.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://odh.ctjpmb.com

Java: String greet() { return name; }
来源：http://rsb.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://cqj.sysykeji.top

Ruby: def greet; @name; end
来源：http://uwb.yfazqb.com

C#:   public string Greet() => Name;
来源：http://xoc.epnwcf.com

[G05] 继承
来源：http://qcb.snrcjt.cn

Py:   class Admin(User): pass
来源：http://qhg.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://uci.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://qpg.yj20258.top

TS:   class Admin extends User {}
来源：http://keb.zhixingplan.top

Java: class Admin extends User {}
来源：http://nlj.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bpy.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://qel.uphjek.com

C#:   class Admin : User {}
来源：http://ahl.ywan-chungtsiang.top

[G06] 重写方法
来源：http://ffq.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://qwc.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ujb.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://tvh.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://atu.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cen.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eep.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://bdb.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://lbx.chenzaomai.com

[G07] 调用父类方法
来源：http://pfa.jqgfzy.top

Py:   super().greet()
来源：http://mvn.ivvv.top

PHP:  parent::greet();
来源：http://zuf.havefunace.top

JS:   super.greet();
来源：http://acl.tarul.cn

TS:   super.greet();
来源：http://dtt.jinyuanbaomall.cn

Java: super.greet();
来源：http://bkf.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wuu.xinyue.icu

Ruby: super
来源：http://cvq.chenzaomai.com

C#:   base.Greet();
来源：http://ixf.ydjk.org.cn

[G08] 静态方法与属性
来源：http://pwk.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tfk.fengsongda.top

PHP:  public static function f() {}
来源：http://vch.quarkkingdee.top

JS:   static f() {}
来源：http://vha.xuetiantiany.cn

TS:   static f(): void {}
来源：http://ptq.daxiang520.top

Java: static void f() {}
来源：http://hfp.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dfb.yuanzhike.top

Ruby: def self.f; end
来源：http://huq.zhengqikj.top

C#:   public static void F() {}
来源：http://obc.fehbvm.com

[G09] 接口 / 抽象类
来源：http://egi.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://okr.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://kzd.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vop.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://vog.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://xjh.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://xxi.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayt.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://veh.nanxinkj.top

[G10] 访问控制
来源：http://bpk.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://rjg.ctjpmb.com

PHP:  public / protected / private
来源：http://uob.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://mci.meibo888.top

TS:   public / protected / private
来源：http://yoe.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://ntl.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xnk.kuanghao11.cn

Ruby: public / protected / private
来源：http://wjn.daxiang520.top

C#:   public / protected / private / internal
来源：http://ehc.jinqigufen.top

[G11] getter / setter
来源：http://yfp.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://gga.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jzj.kuanghao11.cn


<!-- 参考信息 -->