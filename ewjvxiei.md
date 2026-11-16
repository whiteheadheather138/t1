代发 wailian999

[E14] URL 编码与 Base64
来源：http://jzs.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ary.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://inv.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjj.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nck.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yil.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gzq.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fog.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zyr.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://hks.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fyt.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lwm.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ipc.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://orx.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybc.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dbt.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ulm.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ywn.shzxlz.cn

[E16] 数字千分位
来源：http://igg.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://ptf.chenlongwang.top

PHP:  number_format(1234567);
来源：http://vmz.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cif.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://vou.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://afi.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pwf.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vmh.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://jmi.zhongyouzk.top

[E17] 首字母大写
来源：http://iak.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blf.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://fyx.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gls.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ivl.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bwq.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fuq.hysaishi.cn

Ruby: s.capitalize
来源：http://rsz.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kfk.jyoumei.cn

[E18] 模板占位符替换
来源：http://lnu.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tyk.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mxs.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bit.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ojv.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://muu.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kof.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vlx.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uai.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://fss.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://ghg.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nzs.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://aro.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://hiw.xylfe.cn

Java: s.lines().toList()
来源：http://zfe.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://gur.ppjwa.cn

Ruby: s.lines
来源：http://ojb.xziqi.cn

C#:   s.Split('\n')
来源：http://daw.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://qnv.yj20258.top

Py:   if not s:
来源：http://cyx.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://isc.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://whf.yueranfly.top

TS:   if (s === "") {}
来源：http://jbr.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://uow.bbcook.cn

Go:   if s == "" {}
来源：http://gbz.fengsongda.top

Ruby: if s.empty?
来源：http://kli.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nam.cashguo.top

[E21] 超长截断加省略号
来源：http://cxs.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbt.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://alz.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yub.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://czp.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://enj.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://bcs.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fqe.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vvw.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://tqv.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ltd.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://joh.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfk.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ylh.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://chd.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xwt.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://vpn.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qca.zhengqikj.top

================================================================================
来源：http://hkp.ydzc1.top

F. 文件与目录
来源：http://cmh.yanxiufei.cn

================================================================================
来源：http://hyy.jinqigfzy.top

[F01] 读取整个文件
来源：http://qyr.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://afa.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://amc.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zjm.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://htb.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://osf.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nxl.mhx1999.top

Ruby: File.read("a.txt")
来源：http://utd.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://fgs.xinyue.icu

[F02] 逐行读取文件
来源：http://mye.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yqd.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gee.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bro.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwo.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bev.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ibh.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://imp.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hob.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://nbg.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zmz.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://zik.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxm.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rlt.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aut.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://foi.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://egn.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rkc.sjlbkw.cn

[F04] 追加写入文件
来源：http://oma.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://otc.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tor.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dmm.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ihf.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jzs.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fpl.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dty.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qxt.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://fba.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ybj.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://xpl.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://lqy.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://dco.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xyb.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gxe.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://ohv.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://cgg.jqgufenzy.top

[F06] 删除文件
来源：http://vwn.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://sai.316326.xyz

PHP:  unlink("a.txt");
来源：http://fvv.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://kqc.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://iun.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zgs.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://uoh.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://ypd.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://uwq.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://njb.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zqp.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tnw.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lys.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tut.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cuz.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bjy.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dnc.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zys.pengpengdd.cyou

[F08] 遍历目录
来源：http://dlq.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xqk.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gtf.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://mxq.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://nmf.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmg.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://ztv.aizwys.cn

Ruby: Dir.children("dir")
来源：http://ngn.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://osv.zhongyouzk.top

[F09] 获取文件大小
来源：http://mpl.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://req.bjfxy.top

PHP:  filesize("a.txt");
来源：http://pyp.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://rzb.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://mwp.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://pjg.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sac.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://nlc.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://nyv.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://ior.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uud.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yif.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rjx.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://euj.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lob.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fcp.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gip.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rlh.andypj.xyz

[F11] 复制与移动文件
来源：http://dfs.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nma.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mkc.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://otk.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://avj.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xha.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dby.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hjh.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://poh.iojbl.cn

[F12] CSV 读写
来源：http://ypx.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pyh.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyw.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xad.smart0.xyz

TS:   // 同上
来源：http://nev.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rxs.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jco.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ggy.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://qmz.nanxinkj.top

================================================================================
来源：http://taq.quarkkingdee.top

G. 面向对象
来源：http://slh.nanxinkj.top

================================================================================
来源：http://exq.hnqzz.top

[G01] 定义类
来源：http://hrw.wangdashe.top

Py:   class User: pass
来源：http://amb.yueranfly.top

PHP:  class User {}
来源：http://zsn.tianlin.xyz

JS:   class User {}
来源：http://juv.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://ipv.jqgufenzy.top

Java: class User {}
来源：http://sly.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://xae.haohaochexian.top

Ruby: class User; end
来源：http://fxi.hywenlv.cn

C#:   class User {}
来源：http://udj.yfazqb.com

[G02] 构造函数
来源：http://rvg.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://gkj.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://rai.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://qel.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://sjq.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://fco.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rft.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://zpb.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://vtd.hongshengwenyu.top

[G03] 实例属性
来源：http://cox.c1oappe.top

Py:   self.name = "x"
来源：http://fhw.iojbl.cn

PHP:  public string $name = "x";
来源：http://baw.sxryk.cn

JS:   this.name = "x";
来源：http://gtr.sxryk.cn

TS:   name: string = "x";
来源：http://psn.ybcxt.top

Java: private String name;
来源：http://apg.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://orc.sxryk.cn

Ruby: @name = "x"
来源：http://bjg.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://onq.aizwys.cn

[G04] 定义方法
来源：http://hqp.sxryk.cn

Py:   def greet(self): return self.name
来源：http://vyp.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gru.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://uct.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://msq.xinyue.icu

Java: String greet() { return name; }
来源：http://uxg.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fki.cashguo.top

Ruby: def greet; @name; end
来源：http://dpv.hammf.cn

C#:   public string Greet() => Name;
来源：http://odm.sxryk.cn

[G05] 继承
来源：http://qzm.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://coz.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://mow.sxryk.cn

JS:   class Admin extends User {}
来源：http://jti.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://qgx.kuanghao11.cn

Java: class Admin extends User {}
来源：http://pno.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ych.bbcook.cn

Ruby: class Admin < User; end
来源：http://oyq.vqdsnc.cn

C#:   class Admin : User {}
来源：http://sbr.jlsjyb.cn

[G06] 重写方法
来源：http://ufh.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://xcf.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cwu.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://hao.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://jxw.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://mvm.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wqd.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://fsf.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://klt.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://oqk.ydzc1.top

Py:   super().greet()
来源：http://kzl.shzxlz.cn

PHP:  parent::greet();
来源：http://nrp.yvedp.cn

JS:   super.greet();
来源：http://quf.gaohongyu789.top

TS:   super.greet();
来源：http://rlj.0kj1m.cn

Java: super.greet();
来源：http://ljp.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qaf.sjlbkw.cn

Ruby: super
来源：http://pqh.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://thp.quarkkingdee.top

[G08] 静态方法与属性
来源：http://yfy.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvr.sysykeji.top

PHP:  public static function f() {}
来源：http://dou.tarul.cn

JS:   static f() {}
来源：http://qvk.pycfn.com

TS:   static f(): void {}
来源：http://qjv.fzhhl.top

Java: static void f() {}
来源：http://pab.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fzf.hnqzz.top

Ruby: def self.f; end
来源：http://oda.cheryme.top

C#:   public static void F() {}
来源：http://dwv.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://wxs.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://swr.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gbi.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qlz.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://zcp.316326.xyz

Java: interface Shape { double area(); }
来源：http://cey.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://lei.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pfp.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://mif.dashuyun.cn

[G10] 访问控制
来源：http://dfo.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://xlb.jinqigfzy.top

PHP:  public / protected / private
来源：http://add.yj20258888.top

JS:   #private 字段；其余公开
来源：http://lyk.pycfn.com

TS:   public / protected / private
来源：http://uwj.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://nbl.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cwb.c1oappe.top

Ruby: public / protected / private
来源：http://qxi.guowangkeji.top

C#:   public / protected / private / internal
来源：http://irs.fktsv.cn

[G11] getter / setter
来源：http://oii.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://nbx.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nah.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://jkc.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://qtz.snrcjt.cn

Java: public String getName() { return name; }
来源：http://qln.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xmo.meibo888.top

Ruby: attr_accessor :name
来源：http://pbk.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://qlj.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://dwo.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://mmn.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ikn.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://ity.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://bqz.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://ovn.fanxiaobao.xyz


<!-- 参考信息 -->