代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://twg.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rmk.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nnm.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ukn.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nch.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://rnb.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sna.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dpf.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aci.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://xzv.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wnv.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iws.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wck.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oud.pycfn.com

[E16] 数字千分位
来源：http://wwa.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://tqu.jiagoushi.top

PHP:  number_format(1234567);
来源：http://bge.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://par.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zlv.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rtg.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wru.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mgi.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://gyi.hnxiangtu.top

[E17] 首字母大写
来源：http://tqr.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tqg.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kls.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sqi.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opf.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yef.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lmg.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://iqb.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hbx.yonumen.top

[E18] 模板占位符替换
来源：http://gzv.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vwh.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tsu.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zon.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ukg.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://acl.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ejz.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ued.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vzn.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://amy.yanxiufei.cn

Py:   s.splitlines()
来源：http://icl.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jwf.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://tdb.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://jeh.sysykeji.top

Java: s.lines().toList()
来源：http://jhp.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://sdw.meibo888.top

Ruby: s.lines
来源：http://des.dashuyun.cn

C#:   s.Split('\n')
来源：http://rpj.yj20258888.top

[E20] 判断字符串是否为空
来源：http://kog.bjfxy.top

Py:   if not s:
来源：http://kfg.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmn.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aie.zhongyouzk.top

TS:   if (s === "") {}
来源：http://mah.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://jgw.redwolf501.top

Go:   if s == "" {}
来源：http://zhf.wangdashe.top

Ruby: if s.empty?
来源：http://yyo.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mcc.yueranfly.top

[E21] 超长截断加省略号
来源：http://gbt.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://luy.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nxo.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trg.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://slp.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fig.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://obn.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gch.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://arn.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://zoj.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://myt.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tlh.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ueh.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iip.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yjq.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ikl.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://rxz.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhn.tian-w.cn

================================================================================
来源：http://dmn.fanxiaobao.xyz

F. 文件与目录
来源：http://cgx.jyoumei.cn

================================================================================
来源：http://frn.tanke756.top

[F01] 读取整个文件
来源：http://bjj.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sgz.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://srn.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jje.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wzf.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dxl.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qys.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://azy.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://fpw.epnwcf.com

[F02] 逐行读取文件
来源：http://cwv.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nwo.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://okl.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcq.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mhs.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vqn.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ags.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://flr.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eed.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://bnj.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pki.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vhx.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkg.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kuk.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xnz.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mpm.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://rto.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sos.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://dwf.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://miz.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tvk.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hks.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pnp.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mmq.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zcf.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://let.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ktt.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://rhm.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oqj.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://aib.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://guw.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://qpy.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ynu.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://skp.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://mzx.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://cuu.shanyushiyangtech.top

[F06] 删除文件
来源：http://xof.uphjek.com

Py:   os.remove("a.txt")
来源：http://khb.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://jbi.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://wyk.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://qtf.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zzo.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://gjr.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://jxk.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://srk.yfazqb.com

[F07] 创建目录（含多级）
来源：http://tev.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://arb.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bwz.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kdn.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hub.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://abc.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mdd.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agr.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cpq.hongshengwenyu.top

[F08] 遍历目录
来源：http://ojw.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vyh.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eoc.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://ydd.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://akz.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://beg.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ojn.yueranfly.top

Ruby: Dir.children("dir")
来源：http://uvo.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://gfb.guowangkeji.top

[F09] 获取文件大小
来源：http://fbz.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://bcf.yvedp.cn

PHP:  filesize("a.txt");
来源：http://kps.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://nvc.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://xko.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://pqf.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zjj.sysykeji.top

Ruby: File.size("a.txt")
来源：http://loq.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://qny.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://quh.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qwz.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xcp.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rha.tarul.cn

TS:   path.extname("a.txt")
来源：http://bvc.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://erk.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bbx.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pdj.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://axl.havefunace.top

[F11] 复制与移动文件
来源：http://mku.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jhb.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mfh.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnw.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xuf.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://anu.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://acs.svipenyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ckj.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xwx.tian-w.cn

[F12] CSV 读写
来源：http://ydc.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmn.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zhf.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eof.yfazqb.com

TS:   // 同上
来源：http://oql.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dxv.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uqn.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pnd.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vey.hysaishi.cn

================================================================================
来源：http://jom.316326.xyz

G. 面向对象
来源：http://ers.xinyue.icu

================================================================================
来源：http://wsi.kuanghao11.cn

[G01] 定义类
来源：http://bub.kuanghao11.cn

Py:   class User: pass
来源：http://hvg.cqqwz.cn

PHP:  class User {}
来源：http://opy.tian-w.cn

JS:   class User {}
来源：http://gnj.sweek.top

TS:   class User { name: string = ""; }
来源：http://wxm.jinqigfzy.top

Java: class User {}
来源：http://pek.nwbrower.top

Go:   type User struct { Name string }
来源：http://xbl.jiagoushi.top

Ruby: class User; end
来源：http://syp.xylfe.cn

C#:   class User {}
来源：http://fed.hfpthk.cn

[G02] 构造函数
来源：http://jki.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://byy.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://dwn.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://usa.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://zly.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://sug.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ech.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://lat.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://aod.xuetiantiany.cn

[G03] 实例属性
来源：http://hrt.svipenyu.cn

Py:   self.name = "x"
来源：http://qvr.sweek.top

PHP:  public string $name = "x";
来源：http://lxr.0kj1m.cn

JS:   this.name = "x";
来源：http://icd.cashguo.top

TS:   name: string = "x";
来源：http://mjf.pengpengdd.cyou

Java: private String name;
来源：http://tnk.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xex.shuidangran.top

Ruby: @name = "x"
来源：http://bxp.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://lgz.jianghu66.top

[G04] 定义方法
来源：http://wla.cqqwz.cn

Py:   def greet(self): return self.name
来源：http://yvn.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uve.yuxming.cn

JS:   greet() { return this.name; }
来源：http://oky.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://tfa.ivvv.top

Java: String greet() { return name; }
来源：http://dqm.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://pmw.daria6918.cn

Ruby: def greet; @name; end
来源：http://rkq.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://eeg.cucudq.cn

[G05] 继承
来源：http://czg.shuidangran.top

Py:   class Admin(User): pass
来源：http://kof.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://gio.dianchejie.cn

JS:   class Admin extends User {}
来源：http://lfz.andypj.xyz

TS:   class Admin extends User {}
来源：http://vdr.daxiang520.top

Java: class Admin extends User {}
来源：http://szk.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sga.tianlin.xyz

Ruby: class Admin < User; end
来源：http://yrn.vehdjk.com

C#:   class Admin : User {}
来源：http://wio.iojbl.cn

[G06] 重写方法
来源：http://bvb.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://iuj.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rcx.yongpay.top

JS:   greet() { return "admin"; }
来源：http://ifp.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://tqz.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://fgd.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mnx.ivvv.top

Ruby: def greet; "admin"; end
来源：http://quc.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://edp.yj20258888.top

[G07] 调用父类方法
来源：http://fxv.redwolf501.top

Py:   super().greet()
来源：http://uyy.nanxinkj.top

PHP:  parent::greet();
来源：http://cdu.jlsjyb.cn

JS:   super.greet();
来源：http://wtf.ctjpmb.com

TS:   super.greet();
来源：http://oaz.quarkkingdee.top

Java: super.greet();
来源：http://cvi.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://avi.haohaochexian.top

Ruby: super
来源：http://htj.andypj.xyz

C#:   base.Greet();
来源：http://cdy.hysaishi.cn

[G08] 静态方法与属性
来源：http://zyk.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aam.sweek.top

PHP:  public static function f() {}
来源：http://zzw.meibo888.top

JS:   static f() {}
来源：http://ize.xylfe.cn

TS:   static f(): void {}
来源：http://ccz.cheryme.top

Java: static void f() {}
来源：http://epr.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pzj.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://jps.wangshuangyany.cn

C#:   public static void F() {}
来源：http://ese.gzhubu.top

[G09] 接口 / 抽象类
来源：http://ewz.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://jzn.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rqr.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://obh.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://kae.epnwcf.com

Java: interface Shape { double area(); }
来源：http://jri.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://faw.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cxc.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://xgq.daxiang520.top

[G10] 访问控制
来源：http://rik.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ong.redwolf501.top

PHP:  public / protected / private
来源：http://jfm.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://jjo.ehwqpu.com

TS:   public / protected / private
来源：http://ysq.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://yfx.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vvh.0kj1m.cn

Ruby: public / protected / private
来源：http://njy.daxiang520.top

C#:   public / protected / private / internal
来源：http://cym.tanke756.top

[G11] getter / setter
来源：http://vaj.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://kvc.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ofs.birdmap.top

JS:   get name() { return this._name; }
来源：http://tbo.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://ufq.gogol.net.cn

Java: public String getName() { return name; }
来源：http://hgw.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://txz.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://yno.epnwcf.com

C#:   public string Name { get; set; }
来源：http://btu.fzhhl.top

[G12] 对象转字符串
来源：http://qmu.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://fjf.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rjp.xylfe.cn

JS:   toString() { return this.name; }
来源：http://jsb.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://qte.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://ljm.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://adq.cucudq.cn

Ruby: def to_s; @name; end
来源：http://xks.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://jjw.ybcxt.top

[G13] 判断对象类型
来源：http://vso.wangdashe.top


<!-- 参考信息 -->