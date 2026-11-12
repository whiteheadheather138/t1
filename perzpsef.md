代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hvp.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qpt.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xzc.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gpi.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yom.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://eqk.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ytn.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hra.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oan.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lwp.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fos.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jak.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gmi.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wwl.shanyushiyangtech.top

[E16] 数字千分位
来源：http://akf.xylfe.cn

Py:   f"{1234567:,}"
来源：http://gnc.xziqi.cn

PHP:  number_format(1234567);
来源：http://yhy.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fsy.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wdy.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vpv.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jkg.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pva.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://rst.jqgfzy.top

[E17] 首字母大写
来源：http://hnz.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tcs.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jpq.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kdu.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsa.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hqj.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lsh.ctjpmb.com

Ruby: s.capitalize
来源：http://kcq.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ado.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://yzy.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://guw.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umx.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tij.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vbo.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wjx.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dqm.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kqr.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eul.bbcook.cn

[E19] 多行文本按行拆分
来源：http://ejr.guannengcc.top

Py:   s.splitlines()
来源：http://joa.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qbl.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://txx.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://hbk.yongpay.top

Java: s.lines().toList()
来源：http://jfj.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://bfw.jlsjyb.cn

Ruby: s.lines
来源：http://irg.yongpay.top

C#:   s.Split('\n')
来源：http://hrr.yvedp.cn

[E20] 判断字符串是否为空
来源：http://vxg.yuanzhike.top

Py:   if not s:
来源：http://pap.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yib.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vnw.pycfn.com

TS:   if (s === "") {}
来源：http://sqs.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://arx.hfpthk.cn

Go:   if s == "" {}
来源：http://mgz.sysykeji.top

Ruby: if s.empty?
来源：http://whx.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cah.guowangkeji.top

[E21] 超长截断加省略号
来源：http://pwr.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gat.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jsd.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xws.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gym.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hoi.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://mez.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ekg.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jaj.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://joo.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ojl.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lgc.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://swn.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpz.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bji.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://duy.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://kas.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ddu.xziqi.cn

================================================================================
来源：http://kyu.pengpengdd.cyou

F. 文件与目录
来源：http://axa.hysaishi.cn

================================================================================
来源：http://iqg.yonumen.top

[F01] 读取整个文件
来源：http://ngq.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zow.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://gmx.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wrn.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wig.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jnc.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nmo.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://egn.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jox.wangdashe.top

[F02] 逐行读取文件
来源：http://jdl.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gor.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gvl.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zbb.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tlt.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qsn.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rpv.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uma.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xei.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://vpv.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fgj.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nyk.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifo.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://twz.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zvs.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://spv.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://lna.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dyb.zycfv.cn

[F04] 追加写入文件
来源：http://kue.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://skk.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dau.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyx.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fja.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fuu.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nby.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oiq.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eol.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://vyt.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xma.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://xel.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://rfm.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://ocj.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nfw.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lou.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://vgg.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://fyc.zdqjudy.top

[F06] 删除文件
来源：http://nty.c1oappe.top

Py:   os.remove("a.txt")
来源：http://qwr.cheryme.top

PHP:  unlink("a.txt");
来源：http://aqc.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://sut.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://zhb.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ipk.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://vwy.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://koz.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://gdf.316326.xyz

[F07] 创建目录（含多级）
来源：http://zzm.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ibn.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbe.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kok.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzi.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fud.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oia.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ppf.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wth.haohaochexian.top

[F08] 遍历目录
来源：http://oxu.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tut.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bnd.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://eol.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://qyw.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://seb.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nnm.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://mfq.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://kbh.ppjwa.cn

[F09] 获取文件大小
来源：http://wqy.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://qyf.epnwcf.com

PHP:  filesize("a.txt");
来源：http://sxl.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://edo.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://hoq.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://ejt.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pgw.epnwcf.com

Ruby: File.size("a.txt")
来源：http://nth.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://izc.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://his.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ohl.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ubb.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://whz.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://hyz.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nvx.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xsd.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqt.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sgp.bjfxy.top

[F11] 复制与移动文件
来源：http://vpf.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qwl.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pil.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ytc.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dfk.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://loo.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zvt.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qyo.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lno.havefunace.top

[F12] CSV 读写
来源：http://sel.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xav.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hye.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mdo.ywan-chungtsiang.top

TS:   // 同上
来源：http://cei.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hcb.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dyd.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ltt.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://udp.sjlbkw.cn

================================================================================
来源：http://dqz.fanxiaobao.xyz

G. 面向对象
来源：http://nqx.52xcode.cn

================================================================================
来源：http://fji.hywenlv.cn

[G01] 定义类
来源：http://ork.jlsjyb.cn

Py:   class User: pass
来源：http://ike.hfpthk.cn

PHP:  class User {}
来源：http://ipo.havefunace.top

JS:   class User {}
来源：http://jui.tanke756.top

TS:   class User { name: string = ""; }
来源：http://qvk.xuanzx.com

Java: class User {}
来源：http://nii.yuanzhike.top

Go:   type User struct { Name string }
来源：http://wnf.tanke756.top

Ruby: class User; end
来源：http://lvs.jqgfzy.top

C#:   class User {}
来源：http://xcp.shuidangran.top

[G02] 构造函数
来源：http://wrs.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://jgd.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://osh.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://fer.yj20258.top

TS:   constructor(public name: string) {}
来源：http://wyu.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://gvv.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oeh.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://eqk.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://wdd.hnxiangtu.top

[G03] 实例属性
来源：http://mpa.jinqigufen.top

Py:   self.name = "x"
来源：http://dmj.hammf.cn

PHP:  public string $name = "x";
来源：http://yza.jinqigufen.top

JS:   this.name = "x";
来源：http://ysy.9152youxi.cn

TS:   name: string = "x";
来源：http://yna.ctjpmb.com

Java: private String name;
来源：http://lwg.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nny.sxryk.cn

Ruby: @name = "x"
来源：http://xgv.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://won.zhijiandao.cn

[G04] 定义方法
来源：http://lsu.xylfe.cn

Py:   def greet(self): return self.name
来源：http://bpx.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sxp.fktsv.cn

JS:   greet() { return this.name; }
来源：http://drg.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://jnf.dashuyun.cn

Java: String greet() { return name; }
来源：http://cxc.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://gqr.yongpay.top

Ruby: def greet; @name; end
来源：http://jqq.hnqzz.top

C#:   public string Greet() => Name;
来源：http://gjm.316326.xyz

[G05] 继承
来源：http://bqi.birdmap.top

Py:   class Admin(User): pass
来源：http://qoe.ivvv.top

PHP:  class Admin extends User {}
来源：http://adw.yj20258888.top

JS:   class Admin extends User {}
来源：http://qjv.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://mwy.andypj.xyz

Java: class Admin extends User {}
来源：http://tkr.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vaj.sxryk.cn

Ruby: class Admin < User; end
来源：http://lhx.yueranfly.top

C#:   class Admin : User {}
来源：http://psc.wangshuangyany.cn

[G06] 重写方法
来源：http://pln.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://dpr.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lxg.ivvv.top

JS:   greet() { return "admin"; }
来源：http://yax.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://hex.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://ork.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wxm.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://epz.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://abg.chenlongwang.top

[G07] 调用父类方法
来源：http://pqc.yanxiufei.cn

Py:   super().greet()
来源：http://iwo.jlsjyb.cn

PHP:  parent::greet();
来源：http://jse.fehbvm.com

JS:   super.greet();
来源：http://uyr.uphjek.com

TS:   super.greet();
来源：http://oha.fzhhl.top

Java: super.greet();
来源：http://zqt.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lmq.xylfe.cn

Ruby: super
来源：http://ooj.jiagoushi.top

C#:   base.Greet();
来源：http://kht.jinqigufen.top

[G08] 静态方法与属性
来源：http://tqr.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cab.tian-w.cn

PHP:  public static function f() {}
来源：http://lyx.cdnleiting.top

JS:   static f() {}
来源：http://qse.yonumen.top

TS:   static f(): void {}
来源：http://sii.zhijiandao.cn

Java: static void f() {}
来源：http://vxr.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ayj.bbcook.cn

Ruby: def self.f; end
来源：http://kxs.iojbl.cn

C#:   public static void F() {}
来源：http://wax.xinyue.icu

[G09] 接口 / 抽象类
来源：http://tvt.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://ktj.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zqf.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mwp.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://xaq.smart0.xyz

Java: interface Shape { double area(); }
来源：http://ltx.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://qwb.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dnb.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://xjc.shzxlz.cn

[G10] 访问控制
来源：http://uoz.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://owv.jianghu66.top

PHP:  public / protected / private
来源：http://kpk.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://ekc.ivvv.top

TS:   public / protected / private
来源：http://dro.birdmap.top

Java: public / protected / private / 默认包级
来源：http://pdb.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://siw.quarkkingdee.top

Ruby: public / protected / private
来源：http://elv.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://xzj.xuanzx.com

[G11] getter / setter
来源：http://bbo.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://wdu.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jib.jianghu66.top

JS:   get name() { return this._name; }
来源：http://ijb.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://eje.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://vxr.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ami.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://zgb.sxryk.cn

C#:   public string Name { get; set; }
来源：http://gft.ydjk.org.cn

[G12] 对象转字符串
来源：http://nlp.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://qbw.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://szi.aizwys.cn

JS:   toString() { return this.name; }
来源：http://ece.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://ohq.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://ced.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://rek.iojbl.cn

Ruby: def to_s; @name; end
来源：http://dpj.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://pao.bjfxy.top

[G13] 判断对象类型
来源：http://hly.tianlin.xyz


<!-- 参考信息 -->