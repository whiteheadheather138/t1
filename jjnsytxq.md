代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fki.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ihw.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://adf.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uig.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blp.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://lsk.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://zmo.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ope.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zdh.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xxd.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sns.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jkg.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://itc.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ejb.gogol.net.cn

[E16] 数字千分位
来源：http://xhh.sweek.top

Py:   f"{1234567:,}"
来源：http://jey.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://vrn.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jaf.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yid.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rmm.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrg.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bnw.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://bsw.mhx1999.top

[E17] 首字母大写
来源：http://bfm.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vdo.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tdy.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xea.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gsd.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yiv.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qwz.ppjwa.cn

Ruby: s.capitalize
来源：http://msx.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sjb.guowangkeji.top

[E18] 模板占位符替换
来源：http://zfj.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://phi.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ear.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cke.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://khd.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uel.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yie.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://okj.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lhp.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://vki.yj202588.top

Py:   s.splitlines()
来源：http://thf.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://grp.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://wnc.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://ehm.chenlongwang.top

Java: s.lines().toList()
来源：http://hdg.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://qne.0kj1m.cn

Ruby: s.lines
来源：http://duu.sweek.top

C#:   s.Split('\n')
来源：http://ebz.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://yrq.dianchejie.cn

Py:   if not s:
来源：http://her.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://odp.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tng.meibo888.top

TS:   if (s === "") {}
来源：http://xyf.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://bdu.cashguo.top

Go:   if s == "" {}
来源：http://lke.shuidangran.top

Ruby: if s.empty?
来源：http://pzu.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://foa.iojbl.cn

[E21] 超长截断加省略号
来源：http://wdn.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxw.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fnq.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ovq.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ola.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://umf.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://nnf.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ptb.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://npa.c1oappe.top

[E22] 字节长度与字符长度
来源：http://mns.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ued.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyq.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://udo.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sku.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ent.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ncz.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://rwd.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqi.jinyuanbaomall.cn

================================================================================
来源：http://hjg.hywenlv.cn

F. 文件与目录
来源：http://dzk.hnqzz.top

================================================================================
来源：http://egn.xylfe.cn

[F01] 读取整个文件
来源：http://tou.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nfz.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://hha.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nhs.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irf.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://igp.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jht.redwolf501.top

Ruby: File.read("a.txt")
来源：http://jjm.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://puc.yvedp.cn

[F02] 逐行读取文件
来源：http://kds.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vis.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eij.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eds.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmy.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tvs.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rrp.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tlo.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hrl.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://srb.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xdl.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mcl.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ogp.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xmy.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yrv.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mkj.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://kcu.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vxx.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://gsm.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yby.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://riq.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kzw.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tax.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cet.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://utx.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ofy.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rrf.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://yrf.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jkg.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://iez.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://fzi.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://mxs.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yxh.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vgv.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://zmf.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://inf.vqdsnc.cn

[F06] 删除文件
来源：http://etk.wangdashe.top

Py:   os.remove("a.txt")
来源：http://fzm.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://yte.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://gpa.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://hji.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://est.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://qyf.cheryme.top

Ruby: File.delete("a.txt")
来源：http://wvl.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://knv.hnqzz.top

[F07] 创建目录（含多级）
来源：http://dau.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ccz.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yok.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spw.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uli.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wfa.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oxa.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lvw.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dxg.zycfv.cn

[F08] 遍历目录
来源：http://zdt.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://uyu.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://imb.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://jxp.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bnc.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ecl.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ynj.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://bag.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://qce.cheryme.top

[F09] 获取文件大小
来源：http://sdg.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://bxg.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://yfi.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://cur.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://hfk.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jox.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wbt.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://bti.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://dqb.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://uhj.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xmk.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pou.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bvw.cucudq.cn

TS:   path.extname("a.txt")
来源：http://qul.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jir.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://syr.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ydr.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ppd.fzhhl.top

[F11] 复制与移动文件
来源：http://jzd.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zgz.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://knr.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypi.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mlb.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qnq.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ddk.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ajr.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jyf.hfpthk.cn

[F12] CSV 读写
来源：http://xxr.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sec.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qxx.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hyr.ydzc1.top

TS:   // 同上
来源：http://rth.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cpr.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hws.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqv.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nww.yangfankeji.com

================================================================================
来源：http://xip.ivvv.top

G. 面向对象
来源：http://svn.kuanghao11.cn

================================================================================
来源：http://csm.hesvh.cn

[G01] 定义类
来源：http://dsv.jiagoushi.top

Py:   class User: pass
来源：http://gnw.yangfankeji.com

PHP:  class User {}
来源：http://oqm.xingfuxueyuan.xyz

JS:   class User {}
来源：http://nql.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://wqm.yongpay.top

Java: class User {}
来源：http://wre.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://rwo.pycfn.com

Ruby: class User; end
来源：http://ixd.havefunace.top

C#:   class User {}
来源：http://fji.ydjk.org.cn

[G02] 构造函数
来源：http://ubu.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://npf.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kxm.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://npq.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://ngy.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://fqo.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://egv.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://rqk.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://ajw.zdbjq.cn

[G03] 实例属性
来源：http://jsq.hongshengwenyu.top

Py:   self.name = "x"
来源：http://aea.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://myf.fehbvm.com

JS:   this.name = "x";
来源：http://nix.svipenyu.cn

TS:   name: string = "x";
来源：http://rzw.andypj.xyz

Java: private String name;
来源：http://dqj.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ndg.fehbvm.com

Ruby: @name = "x"
来源：http://ina.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://wra.zhiwuduotai.top

[G04] 定义方法
来源：http://vwc.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://zvl.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mwx.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://xhv.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://cbg.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://gms.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnb.aizwys.cn

Ruby: def greet; @name; end
来源：http://xkg.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://lqp.redwolf501.top

[G05] 继承
来源：http://qyg.hesvh.cn

Py:   class Admin(User): pass
来源：http://kda.smart0.xyz

PHP:  class Admin extends User {}
来源：http://trr.bbcook.cn

JS:   class Admin extends User {}
来源：http://mow.yj202588.top

TS:   class Admin extends User {}
来源：http://shb.fengsongda.top

Java: class Admin extends User {}
来源：http://yqd.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sqq.xziqi.cn

Ruby: class Admin < User; end
来源：http://ykg.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://nuc.zhaomingkeji.xyz

[G06] 重写方法
来源：http://ypt.sweek.top

Py:   def greet(self): return "admin"
来源：http://fkh.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gqc.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://ctj.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://nyb.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://kqa.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://shg.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://cpp.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://kae.andypj.xyz

[G07] 调用父类方法
来源：http://nye.daria6918.cn

Py:   super().greet()
来源：http://thx.andypj.xyz

PHP:  parent::greet();
来源：http://bfk.sweek.top

JS:   super.greet();
来源：http://glv.svipenyu.cn

TS:   super.greet();
来源：http://yaf.jqgufenzy.top

Java: super.greet();
来源：http://sji.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yaf.hongshengwenyu.top

Ruby: super
来源：http://nma.gaohongyu789.top

C#:   base.Greet();
来源：http://arh.cdnleiting.top

[G08] 静态方法与属性
来源：http://ukg.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eox.zhijiandao.cn

PHP:  public static function f() {}
来源：http://tgv.vehdjk.com

JS:   static f() {}
来源：http://rzy.nanxinkj.top

TS:   static f(): void {}
来源：http://uou.fktsv.cn

Java: static void f() {}
来源：http://ywz.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qky.gotoacloud.top

Ruby: def self.f; end
来源：http://frt.yanxiufei.cn

C#:   public static void F() {}
来源：http://idh.bjfxy.top

[G09] 接口 / 抽象类
来源：http://fmc.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://msf.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wrf.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzq.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://rix.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://zns.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://sgi.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://khk.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://bbb.jlsjyb.cn

[G10] 访问控制
来源：http://vpc.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://yxe.hammf.cn

PHP:  public / protected / private
来源：http://zxf.sysykeji.top

JS:   #private 字段；其余公开
来源：http://kuv.guannengcc.top

TS:   public / protected / private
来源：http://xwz.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://avh.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://otv.yueranfly.top

Ruby: public / protected / private
来源：http://yvb.zycfv.cn

C#:   public / protected / private / internal
来源：http://zhn.ivvv.top

[G11] getter / setter
来源：http://nvd.zycfv.cn

Py:   @property 与 @x.setter
来源：http://ben.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://chc.pycfn.com

JS:   get name() { return this._name; }
来源：http://wwj.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://dsv.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://iwk.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://cpd.havefunace.top

Ruby: attr_accessor :name
来源：http://yzq.yfazqb.com

C#:   public string Name { get; set; }
来源：http://jcy.cheryme.top

[G12] 对象转字符串
来源：http://mrv.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://rpn.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ybe.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://bhf.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://rqq.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://req.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://piv.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://udt.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://ypf.xuetiantiany.cn

[G13] 判断对象类型
来源：http://yub.gaohongyu789.top


<!-- 参考信息 -->