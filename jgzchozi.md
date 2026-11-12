代发 wailian999

[E14] URL 编码与 Base64
来源：http://rja.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rut.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rls.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fhe.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhw.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vpk.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wmx.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://npr.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ryf.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://ldz.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yff.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cus.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://quw.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pcw.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tyz.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lrj.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gxm.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqh.bbcook.cn

[E16] 数字千分位
来源：http://ocd.nwbrower.top

Py:   f"{1234567:,}"
来源：http://wtf.ctjpmb.com

PHP:  number_format(1234567);
来源：http://ljq.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qks.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://vdo.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ktz.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ifz.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aoq.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://ivl.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://yry.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ifv.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fon.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zby.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qar.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ktp.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rhh.fehbvm.com

Ruby: s.capitalize
来源：http://abt.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdj.cdnleiting.top

[E18] 模板占位符替换
来源：http://xqz.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vki.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tqq.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jdg.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nyx.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lvk.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jde.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tpd.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hlq.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://ofm.zhiwuduotai.top

Py:   s.splitlines()
来源：http://wst.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jtn.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://hjt.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://olf.wangdashe.top

Java: s.lines().toList()
来源：http://ymy.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://egf.dashuyun.cn

Ruby: s.lines
来源：http://nue.mhx1999.top

C#:   s.Split('\n')
来源：http://hpn.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://wvz.c1oappe.top

Py:   if not s:
来源：http://gjh.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zbv.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yfi.c1oappe.top

TS:   if (s === "") {}
来源：http://mgb.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://jeg.birdmap.top

Go:   if s == "" {}
来源：http://twq.hesvh.cn

Ruby: if s.empty?
来源：http://kev.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aii.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://rdm.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wzg.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ppm.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvl.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bku.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dnv.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://dzo.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://twm.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kwa.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://agd.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lww.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://msd.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvc.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://paz.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mxo.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tvo.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://wel.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qkf.meibo888.top

================================================================================
来源：http://mlx.xylfe.cn

F. 文件与目录
来源：http://smp.hnqzz.top

================================================================================
来源：http://tej.cqqwz.cn

[F01] 读取整个文件
来源：http://mxp.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aln.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://icu.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sok.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eni.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://btq.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfm.havefunace.top

Ruby: File.read("a.txt")
来源：http://zom.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://all.yj202588.top

[F02] 逐行读取文件
来源：http://yjz.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zqk.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lrs.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://njt.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uld.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dlc.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jlh.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://keq.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pqo.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://upz.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kfr.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pvb.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zjl.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tya.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://plo.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mht.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://kqa.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://whu.chenjidiqi.icu

[F04] 追加写入文件
来源：http://pey.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mue.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yiw.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctq.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xor.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fge.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fae.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xfa.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gya.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://rnh.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://duh.yongpay.top

PHP:  file_exists("a.txt");
来源：http://vfj.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://adn.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://dge.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ltf.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rly.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://teh.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://vof.c1oappe.top

[F06] 删除文件
来源：http://mxa.yongpay.top

Py:   os.remove("a.txt")
来源：http://wro.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://izr.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://npg.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cav.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xfb.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://ouw.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://cep.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://fpt.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://nvj.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://feh.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tdl.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnq.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lpg.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jhm.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ntz.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kkj.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xpx.tianlin.xyz

[F08] 遍历目录
来源：http://gkj.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ujb.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qlm.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://cto.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://lhg.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qda.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mzp.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://cby.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://usz.wangdashe.top

[F09] 获取文件大小
来源：http://pln.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ogp.meibo888.top

PHP:  filesize("a.txt");
来源：http://ngb.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://yyc.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://nry.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zki.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://whm.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://vij.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://rpj.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://yfa.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gpq.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zuc.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://byz.cucudq.cn

TS:   path.extname("a.txt")
来源：http://bud.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dys.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fwp.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nfo.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://brt.yangfankeji.com

[F11] 复制与移动文件
来源：http://vpc.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hiq.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://htt.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egw.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://muy.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oqz.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://byu.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aic.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lvd.cucudq.cn

[F12] CSV 读写
来源：http://lce.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://osz.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bcm.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oum.smart0.xyz

TS:   // 同上
来源：http://xyx.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://onr.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://phd.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wip.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ght.ehwqpu.com

================================================================================
来源：http://ahg.shangyingyoupin.top

G. 面向对象
来源：http://lvv.mhx1999.top

================================================================================
来源：http://ezb.shzxlz.cn

[G01] 定义类
来源：http://rin.ppjwa.cn

Py:   class User: pass
来源：http://vkm.zhijiandao.cn

PHP:  class User {}
来源：http://mlj.svipenyu.cn

JS:   class User {}
来源：http://jit.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://tdd.zdbjq.cn

Java: class User {}
来源：http://prd.ppjwa.cn

Go:   type User struct { Name string }
来源：http://tkt.yonumen.top

Ruby: class User; end
来源：http://ews.gotoacloud.top

C#:   class User {}
来源：http://vzg.yj202588.top

[G02] 构造函数
来源：http://xvn.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://srw.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://wam.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://okb.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://wrd.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://esy.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://not.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://uxj.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://omt.feifeiyinyue.top

[G03] 实例属性
来源：http://ftv.hcnkem.com

Py:   self.name = "x"
来源：http://zpi.fzhhl.top

PHP:  public string $name = "x";
来源：http://pqm.hnqzz.top

JS:   this.name = "x";
来源：http://cmx.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://xhu.gogol.net.cn

Java: private String name;
来源：http://mhf.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dpy.shangyingyoupin.top

Ruby: @name = "x"
来源：http://vey.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://qgl.hfpthk.cn

[G04] 定义方法
来源：http://kgt.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://axj.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vsr.bbcook.cn

JS:   greet() { return this.name; }
来源：http://ayq.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://hfj.aizwys.cn

Java: String greet() { return name; }
来源：http://nva.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://agf.daria6918.cn

Ruby: def greet; @name; end
来源：http://nyq.bbcook.cn

C#:   public string Greet() => Name;
来源：http://nfb.jinghuilouyu.cn

[G05] 继承
来源：http://uwe.hfpthk.cn

Py:   class Admin(User): pass
来源：http://hty.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://uxo.fengsongda.top

JS:   class Admin extends User {}
来源：http://mjs.fengsongda.top

TS:   class Admin extends User {}
来源：http://yws.yuxming.cn

Java: class Admin extends User {}
来源：http://wyb.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lvc.sweek.top

Ruby: class Admin < User; end
来源：http://eth.zdqjudy.top

C#:   class Admin : User {}
来源：http://edm.nanxinkj.top

[G06] 重写方法
来源：http://hgk.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://ryy.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xzx.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://npd.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://hin.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://fby.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fll.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://pre.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://yhn.hfpthk.cn

[G07] 调用父类方法
来源：http://uuj.jiagoushi.top

Py:   super().greet()
来源：http://jby.fzhhl.top

PHP:  parent::greet();
来源：http://bpn.gotoacloud.top

JS:   super.greet();
来源：http://oaa.xinyue.icu

TS:   super.greet();
来源：http://ren.jyoumei.cn

Java: super.greet();
来源：http://nww.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uxn.ivvv.top

Ruby: super
来源：http://pjs.yonumen.top

C#:   base.Greet();
来源：http://unt.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://uis.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oab.jqgfzy.top

PHP:  public static function f() {}
来源：http://fmx.xziqi.cn

JS:   static f() {}
来源：http://eqi.snrcjt.cn

TS:   static f(): void {}
来源：http://gna.cdnleiting.top

Java: static void f() {}
来源：http://yqi.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://azo.yangfankeji.com

Ruby: def self.f; end
来源：http://ipi.yfazqb.com

C#:   public static void F() {}
来源：http://qjh.cashguo.top

[G09] 接口 / 抽象类
来源：http://ttb.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://bgf.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://azr.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jyl.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://uod.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://yam.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://mlz.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lew.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://wqk.yj202588.top

[G10] 访问控制
来源：http://mru.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://uhl.yanxiufei.cn

PHP:  public / protected / private
来源：http://jgh.smart0.xyz

JS:   #private 字段；其余公开
来源：http://wcj.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://fiy.cashguo.top

Java: public / protected / private / 默认包级
来源：http://hip.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kcx.52xcode.cn

Ruby: public / protected / private
来源：http://xhd.tianlin.xyz

C#:   public / protected / private / internal
来源：http://zbb.havefunace.top

[G11] getter / setter
来源：http://qkz.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://vwj.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ojz.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://dyx.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://hca.bjfxy.top

Java: public String getName() { return name; }
来源：http://wqp.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mle.cdnleiting.top

Ruby: attr_accessor :name
来源：http://yfq.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://dzp.gaohongyu789.top

[G12] 对象转字符串
来源：http://vai.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://lnj.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tlf.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://sfv.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://npn.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://zuc.shanyushiyangkeji.top


<!-- 参考信息 -->