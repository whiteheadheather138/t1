代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qya.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gve.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://awi.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xtg.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://sqq.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ylc.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://lng.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bqs.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ata.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ych.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nkd.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cxz.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vww.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://isl.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nkj.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfz.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sze.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ggm.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eba.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yxv.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aun.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://drs.zhixingplan.top

[E16] 数字千分位
来源：http://yzw.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://uip.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://iwl.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wsu.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://koi.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pno.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://euy.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mpm.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://vai.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://fxw.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://erw.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dvh.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iom.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jix.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cda.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bnx.haohaochexian.top

Ruby: s.capitalize
来源：http://iqv.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bdd.bbcook.cn

[E18] 模板占位符替换
来源：http://thl.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yvh.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nnv.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jdt.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zoe.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://buv.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://odr.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://inz.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sfn.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://ydt.wangdashe.top

Py:   s.splitlines()
来源：http://mqq.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qps.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://asm.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://pfe.sxryk.cn

Java: s.lines().toList()
来源：http://nvl.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://bpk.jianghu66.top

Ruby: s.lines
来源：http://mwp.jlsjyb.cn

C#:   s.Split('\n')
来源：http://rnp.birdmap.top

[E20] 判断字符串是否为空
来源：http://mjb.yueranfly.top

Py:   if not s:
来源：http://gtr.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ufu.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zab.hnxiangtu.top

TS:   if (s === "") {}
来源：http://tdq.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://jpl.chenjidiqi.icu

Go:   if s == "" {}
来源：http://yaq.shuidangran.top

Ruby: if s.empty?
来源：http://fqw.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://buc.hesvh.cn

[E21] 超长截断加省略号
来源：http://ydm.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oga.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ulf.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lhs.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oog.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xlx.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://tuq.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ist.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iic.xinyue.icu

[E22] 字节长度与字符长度
来源：http://kva.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://spz.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://trp.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vgp.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uus.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofz.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dda.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://jna.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oyk.yueranfly.top

================================================================================
来源：http://gox.ywan-chungtsiang.top

F. 文件与目录
来源：http://ukm.9152youxi.cn

================================================================================
来源：http://bro.ivvv.top

[F01] 读取整个文件
来源：http://cfl.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xbj.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://zjw.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rgr.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qac.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ztr.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xic.bjfxy.top

Ruby: File.read("a.txt")
来源：http://lkr.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://szg.iojbl.cn

[F02] 逐行读取文件
来源：http://ozb.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dxf.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ans.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ymm.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blu.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gfa.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gwh.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xln.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nvo.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://tgv.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vqr.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ysc.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sxl.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vhq.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://syx.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fek.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://vgj.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ywr.sweek.top

[F04] 追加写入文件
来源：http://dtj.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://etf.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://woz.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://evz.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cvd.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ton.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://upb.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://khl.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aoa.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://oas.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://usu.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://teo.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://veg.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://eiv.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yru.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jzm.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://fgp.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://lsx.hongshengwenyu.top

[F06] 删除文件
来源：http://wqe.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://hnm.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://pny.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://med.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://fmg.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://otm.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://wrj.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://ohp.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://wxn.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://dyc.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fkb.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ryi.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndc.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wbx.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jne.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jwt.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lwz.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tgr.chenlongwang.top

[F08] 遍历目录
来源：http://iae.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ats.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://his.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://cio.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://bgi.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mig.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fkk.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://nim.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://swf.ydjk.org.cn

[F09] 获取文件大小
来源：http://btj.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://ubr.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://ioz.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://xan.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://xcm.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nkg.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://osg.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://abu.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://cch.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://mtb.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eyb.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uhs.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qfu.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://jlp.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kvu.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yha.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hrf.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wuf.zhengqikj.top

[F11] 复制与移动文件
来源：http://sur.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xhe.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bqd.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eab.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://taw.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbp.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wlf.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nbj.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dst.hfpthk.cn

[F12] CSV 读写
来源：http://qmo.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://viq.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lpv.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yva.52xcode.cn

TS:   // 同上
来源：http://iur.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aow.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://amx.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qip.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gcb.zhaomingkeji.xyz

================================================================================
来源：http://yoi.quarkkingdee.top

G. 面向对象
来源：http://bhc.jqgufenzy.top

================================================================================
来源：http://bfa.dashuyun.cn

[G01] 定义类
来源：http://jdu.chenlongwang.top

Py:   class User: pass
来源：http://hhk.hysaishi.cn

PHP:  class User {}
来源：http://cbi.gzhubu.top

JS:   class User {}
来源：http://puq.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://tvc.redwolf501.top

Java: class User {}
来源：http://yzj.zdqjudy.top

Go:   type User struct { Name string }
来源：http://arc.xinyue.icu

Ruby: class User; end
来源：http://ysj.cheryme.top

C#:   class User {}
来源：http://apz.zhijiandao.cn

[G02] 构造函数
来源：http://thf.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://soa.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://xls.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://dum.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://frf.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://dce.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wgj.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://efj.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://idw.bbcook.cn

[G03] 实例属性
来源：http://zhz.hammf.cn

Py:   self.name = "x"
来源：http://lio.nwbrower.top

PHP:  public string $name = "x";
来源：http://ixa.gaohongyu789.top

JS:   this.name = "x";
来源：http://gbc.epnwcf.com

TS:   name: string = "x";
来源：http://kds.fktsv.cn

Java: private String name;
来源：http://nsl.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://elm.fengsongda.top

Ruby: @name = "x"
来源：http://ppl.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://xwv.wangdashe.top

[G04] 定义方法
来源：http://yxz.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://qdp.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nvy.havefunace.top

JS:   greet() { return this.name; }
来源：http://eom.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://gnj.chenlongwang.top

Java: String greet() { return name; }
来源：http://ufq.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wtw.chenzaomai.com

Ruby: def greet; @name; end
来源：http://qih.jianghu66.top

C#:   public string Greet() => Name;
来源：http://ucp.tarul.cn

[G05] 继承
来源：http://trf.52xcode.cn

Py:   class Admin(User): pass
来源：http://xku.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://nux.ehwqpu.com

JS:   class Admin extends User {}
来源：http://sct.zhixingplan.top

TS:   class Admin extends User {}
来源：http://fub.sufxvd.cn

Java: class Admin extends User {}
来源：http://apf.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xai.hnqzz.top

Ruby: class Admin < User; end
来源：http://xqu.cashguo.top

C#:   class Admin : User {}
来源：http://xgt.hammf.cn

[G06] 重写方法
来源：http://dqp.cashguo.top

Py:   def greet(self): return "admin"
来源：http://xfq.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gfo.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://vso.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://obn.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://njl.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://etl.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://hyh.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://cxz.yueranfly.top

[G07] 调用父类方法
来源：http://cjq.hammf.cn

Py:   super().greet()
来源：http://yky.yj202588.top

PHP:  parent::greet();
来源：http://luh.bjfxy.top

JS:   super.greet();
来源：http://wbo.hysaishi.cn

TS:   super.greet();
来源：http://drq.aizwys.cn

Java: super.greet();
来源：http://ddt.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://whm.fktsv.cn

Ruby: super
来源：http://sav.sjlbkw.cn

C#:   base.Greet();
来源：http://lqy.jqgfzy.top

[G08] 静态方法与属性
来源：http://osn.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iic.yuxming.cn

PHP:  public static function f() {}
来源：http://bbp.fanxiaobao.xyz

JS:   static f() {}
来源：http://uvm.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://ggd.kuanghao11.cn

Java: static void f() {}
来源：http://ony.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bip.tianlin.xyz

Ruby: def self.f; end
来源：http://flg.xuanzx.com

C#:   public static void F() {}
来源：http://qlu.yj20258888.top

[G09] 接口 / 抽象类
来源：http://rpx.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://bjs.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://wkl.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ngh.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://pgo.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://urx.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://kdf.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zyt.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://vvi.cucudq.cn

[G10] 访问控制
来源：http://gsb.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://wbf.zhijiandao.cn

PHP:  public / protected / private
来源：http://xhr.epnwcf.com

JS:   #private 字段；其余公开
来源：http://myv.shzxlz.cn

TS:   public / protected / private
来源：http://yla.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://eix.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://jbm.shzxlz.cn

Ruby: public / protected / private
来源：http://jcr.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://kxw.chenzaomai.com

[G11] getter / setter
来源：http://gtu.zycfv.cn

Py:   @property 与 @x.setter
来源：http://kia.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://cuv.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://nhn.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://fur.shuidangran.top

Java: public String getName() { return name; }
来源：http://mff.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ldn.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://ttp.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://mfy.ydzc1.top

[G12] 对象转字符串
来源：http://slt.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://gzw.cucudq.cn


<!-- 参考信息 -->