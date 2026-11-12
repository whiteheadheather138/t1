代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ccv.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ghd.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://blc.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vly.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cbg.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ryv.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cej.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://skc.hnqzz.top

[E14] URL 编码与 Base64
来源：http://bgn.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tbu.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://htr.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bmg.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://quc.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mxz.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dqp.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nio.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bog.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://eux.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lgr.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ctp.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uaa.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zac.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jch.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://plp.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://avy.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tzj.jqgfzy.top

[E16] 数字千分位
来源：http://yeh.yj20258888.top

Py:   f"{1234567:,}"
来源：http://dfo.dianchejie.cn

PHP:  number_format(1234567);
来源：http://axi.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uem.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kvr.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bjp.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xgd.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iik.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://wqh.yuxming.cn

[E17] 首字母大写
来源：http://mgk.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vuq.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zaz.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ahq.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://elt.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rsd.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uyv.xylfe.cn

Ruby: s.capitalize
来源：http://yfv.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kbv.snrcjt.cn

[E18] 模板占位符替换
来源：http://sbg.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hkd.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vil.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sjq.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://acw.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://grq.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gtw.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wew.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ide.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://jif.vqdsnc.cn

Py:   s.splitlines()
来源：http://ikj.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://igy.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://mqp.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://xxz.yueranfly.top

Java: s.lines().toList()
来源：http://cnq.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://blq.cashguo.top

Ruby: s.lines
来源：http://nbm.yangfankeji.com

C#:   s.Split('\n')
来源：http://uev.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://ukx.zhiwuduotai.top

Py:   if not s:
来源：http://oan.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgg.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://akj.yvedp.cn

TS:   if (s === "") {}
来源：http://sqk.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://wsh.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://lbc.hcnkem.com

Ruby: if s.empty?
来源：http://aur.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rtm.xuanzx.com

[E21] 超长截断加省略号
来源：http://yyz.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gfp.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ecd.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhm.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhd.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwq.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://qgl.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://swh.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nug.ydzc1.top

[E22] 字节长度与字符长度
来源：http://yla.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pph.hammf.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qvt.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://syj.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zbm.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xuo.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzf.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://arb.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jzy.svipenyu.cn

================================================================================
来源：http://tne.sysykeji.top

F. 文件与目录
来源：http://blh.zhengqikj.top

================================================================================
来源：http://wtb.sufxvd.cn

[F01] 读取整个文件
来源：http://dys.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iek.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://ore.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://weg.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fuv.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zvl.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mft.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://ijn.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://bnu.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://zrl.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ciy.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mlm.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fpu.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qvo.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oin.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jez.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dnp.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fdq.meibo888.top

[F03] 写入文件（覆盖）
来源：http://hpu.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://usf.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ncn.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rpq.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xde.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kno.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://muf.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://abj.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sxf.vehdjk.com

[F04] 追加写入文件
来源：http://bvh.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lao.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gzv.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vjz.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qdj.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cob.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mfe.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cvy.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyq.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://abe.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xtc.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://ihp.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://uxv.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://wde.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vnm.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dux.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://ewp.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://ipz.daria6918.cn

[F06] 删除文件
来源：http://brb.zycfv.cn

Py:   os.remove("a.txt")
来源：http://ktm.sxryk.cn

PHP:  unlink("a.txt");
来源：http://zhr.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://pvj.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://kaa.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvs.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://zui.tarul.cn

Ruby: File.delete("a.txt")
来源：http://jzf.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://jld.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://zfi.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fgi.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zvm.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ewe.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqz.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hwc.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oeu.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fzm.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yoe.bjfxy.top

[F08] 遍历目录
来源：http://efc.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://cvd.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xyu.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://vdf.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://yqo.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hlt.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://rzd.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://bwk.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://mhw.ybcxt.top

[F09] 获取文件大小
来源：http://omy.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://yhi.fktsv.cn

PHP:  filesize("a.txt");
来源：http://hdt.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://amx.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://fxe.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zpn.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swd.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://ivq.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://sui.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://efk.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pge.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pdu.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://duo.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://tym.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://unc.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://etj.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vpp.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gsi.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://voi.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://plf.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jkl.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://any.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bnn.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cnx.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lah.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jsv.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ilp.dashuyun.cn

[F12] CSV 读写
来源：http://ori.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qxo.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kjn.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iag.shzxlz.cn

TS:   // 同上
来源：http://xef.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oim.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xqc.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ddy.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yry.yanxiufei.cn

================================================================================
来源：http://wdu.xziqi.cn

G. 面向对象
来源：http://uac.tanke756.top

================================================================================
来源：http://egd.aibaodan.cn

[G01] 定义类
来源：http://pyl.hongshengwenyu.top

Py:   class User: pass
来源：http://ips.ydzc1.top

PHP:  class User {}
来源：http://jfn.jinyuanbaomall.cn

JS:   class User {}
来源：http://ncc.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://jdb.cucudq.cn

Java: class User {}
来源：http://qbw.daria6918.cn

Go:   type User struct { Name string }
来源：http://ldf.ybcxt.top

Ruby: class User; end
来源：http://eyk.yanxiufei.cn

C#:   class User {}
来源：http://hjr.iojbl.cn

[G02] 构造函数
来源：http://njc.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://ndy.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://vgc.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://dro.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://jyv.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://mda.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pdj.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://efi.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://ndl.zhiwuduotai.top

[G03] 实例属性
来源：http://ttk.wangshuangyany.cn

Py:   self.name = "x"
来源：http://vgi.zhengqikj.top

PHP:  public string $name = "x";
来源：http://tiu.birdmap.top

JS:   this.name = "x";
来源：http://exb.vqdsnc.cn

TS:   name: string = "x";
来源：http://bul.zhaomingkeji.xyz

Java: private String name;
来源：http://dvc.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zog.tanke756.top

Ruby: @name = "x"
来源：http://wki.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://bjh.cashguo.top

[G04] 定义方法
来源：http://hty.hcnkem.com

Py:   def greet(self): return self.name
来源：http://hia.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://saw.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://xhd.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://adv.hfpthk.cn

Java: String greet() { return name; }
来源：http://xlz.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tbr.jianghu66.top

Ruby: def greet; @name; end
来源：http://cax.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://vjp.pengpengdd.cyou

[G05] 继承
来源：http://wfn.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://kko.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://ijm.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://jnr.gzhubu.top

TS:   class Admin extends User {}
来源：http://wai.sxryk.cn

Java: class Admin extends User {}
来源：http://rlu.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zni.yvedp.cn

Ruby: class Admin < User; end
来源：http://sqv.yfazqb.com

C#:   class Admin : User {}
来源：http://yeb.jyoumei.cn

[G06] 重写方法
来源：http://okz.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://tey.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vzd.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://shr.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://tyb.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://cun.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nln.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://rmo.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://vlz.iojbl.cn

[G07] 调用父类方法
来源：http://qgw.pycfn.com

Py:   super().greet()
来源：http://xrf.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://liv.iojbl.cn

JS:   super.greet();
来源：http://fdz.316326.xyz

TS:   super.greet();
来源：http://vhk.chenjidiqi.icu

Java: super.greet();
来源：http://cvv.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bxf.jlsjyb.cn

Ruby: super
来源：http://raw.ybcxt.top

C#:   base.Greet();
来源：http://doo.tarul.cn

[G08] 静态方法与属性
来源：http://cqa.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bwf.jianghu66.top

PHP:  public static function f() {}
来源：http://mjt.feifeiyinyue.top

JS:   static f() {}
来源：http://nnw.52xcode.cn

TS:   static f(): void {}
来源：http://gjr.cashguo.top

Java: static void f() {}
来源：http://pvx.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dlw.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://ywv.ctjpmb.com

C#:   public static void F() {}
来源：http://oly.fehbvm.com

[G09] 接口 / 抽象类
来源：http://iyq.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://qry.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bcm.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kxb.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://ypy.havefunace.top

Java: interface Shape { double area(); }
来源：http://the.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://lgp.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mam.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://mrm.dianchejie.cn

[G10] 访问控制
来源：http://bea.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://dyu.gotoacloud.top

PHP:  public / protected / private
来源：http://xqb.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://fum.smart0.xyz

TS:   public / protected / private
来源：http://ggz.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://hxw.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxw.hfpthk.cn

Ruby: public / protected / private
来源：http://dii.hysaishi.cn

C#:   public / protected / private / internal
来源：http://cqx.chenjidiqi.icu

[G11] getter / setter
来源：http://ytg.hnqzz.top

Py:   @property 与 @x.setter
来源：http://fxi.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bir.pycfn.com

JS:   get name() { return this._name; }
来源：http://rgd.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://hlg.shuidangran.top

Java: public String getName() { return name; }
来源：http://kca.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bvk.epnwcf.com


<!-- 参考信息 -->