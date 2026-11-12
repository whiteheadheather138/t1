代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rwo.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://you.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://sht.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tfl.ydzc1.top

[E14] URL 编码与 Base64
来源：http://ltg.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://muf.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nqf.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rxa.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bbo.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://crd.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tan.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://haa.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rvp.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://pmi.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lcs.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlk.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yng.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mhg.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kdg.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ggm.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtr.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vbg.gzhubu.top

[E16] 数字千分位
来源：http://hzf.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://snl.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://iui.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xxx.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uzd.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vly.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebz.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fjm.cheryme.top

C#:   1234567.ToString("N0")
来源：http://gxi.jqgufenzy.top

[E17] 首字母大写
来源：http://ehm.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cae.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gjh.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ing.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjk.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mpc.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://krq.ybcxt.top

Ruby: s.capitalize
来源：http://pyf.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fzq.jiagoushi.top

[E18] 模板占位符替换
来源：http://cra.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://par.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zqq.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fin.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mzg.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rgn.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ppi.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vow.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cog.yuxming.cn

[E19] 多行文本按行拆分
来源：http://qad.jinqigfzy.top

Py:   s.splitlines()
来源：http://zgp.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vmo.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://zrs.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://utr.fehbvm.com

Java: s.lines().toList()
来源：http://arf.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://yzp.haohaochexian.top

Ruby: s.lines
来源：http://jyz.zhixingplan.top

C#:   s.Split('\n')
来源：http://cuu.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://yon.aizwys.cn

Py:   if not s:
来源：http://ldi.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyq.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nqq.yfazqb.com

TS:   if (s === "") {}
来源：http://hel.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://sal.fehbvm.com

Go:   if s == "" {}
来源：http://ufg.sysykeji.top

Ruby: if s.empty?
来源：http://lyj.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tnm.xuanzx.com

[E21] 超长截断加省略号
来源：http://ond.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vsl.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://svc.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ont.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjk.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pqh.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://zei.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lvv.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rzp.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://yms.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dtf.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xti.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hiw.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gft.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qav.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ojc.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://ekt.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zkp.wangshuangyany.cn

================================================================================
来源：http://ryq.yonumen.top

F. 文件与目录
来源：http://psi.zhijiandao.cn

================================================================================
来源：http://oxf.shangyingyoupin.top

[F01] 读取整个文件
来源：http://bjo.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oyg.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://tpx.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lta.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hkh.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://caf.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdg.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://isc.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://mlv.cqqwz.cn

[F02] 逐行读取文件
来源：http://xyp.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwp.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tqa.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zti.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehl.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://snn.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://awv.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://csn.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yoe.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://klx.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ysp.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bar.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okq.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfs.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ysd.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://deu.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://hgi.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uoi.haohaochexian.top

[F04] 追加写入文件
来源：http://tur.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ubx.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blo.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tha.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufz.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qfj.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dbw.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pxi.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pqc.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://kuz.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fkk.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://alk.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://mrs.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://xhw.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://owq.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dsq.sweek.top

Ruby: File.exist?("a.txt")
来源：http://nli.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://nch.0kj1m.cn

[F06] 删除文件
来源：http://fgt.cheryme.top

Py:   os.remove("a.txt")
来源：http://poe.uphjek.com

PHP:  unlink("a.txt");
来源：http://twl.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://duy.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://joe.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xxg.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://cdg.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://dhw.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://ovd.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://edh.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bwm.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mxp.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wsm.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bjh.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://azx.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mdx.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qmy.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pkf.guowangkeji.top

[F08] 遍历目录
来源：http://msd.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://llc.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xdk.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://cdi.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://jga.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mmp.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rak.xylfe.cn

Ruby: Dir.children("dir")
来源：http://huy.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://trm.snrcjt.cn

[F09] 获取文件大小
来源：http://anf.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://rmf.meibo888.top

PHP:  filesize("a.txt");
来源：http://hnk.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://bvx.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://wyw.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://ejz.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://heq.fktsv.cn

Ruby: File.size("a.txt")
来源：http://wsx.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://wgm.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://jwx.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nga.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rlc.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtr.epnwcf.com

TS:   path.extname("a.txt")
来源：http://pks.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fcp.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://imx.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lcg.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://klk.jyoumei.cn

[F11] 复制与移动文件
来源：http://umr.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yhs.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://drq.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wyc.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fmr.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cxi.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dox.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uwg.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ckd.tian-w.cn

[F12] CSV 读写
来源：http://xan.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvk.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://poe.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wjs.vqdsnc.cn

TS:   // 同上
来源：http://gom.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gwl.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hni.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vll.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ezd.shuidangran.top

================================================================================
来源：http://hps.zhixingplan.top

G. 面向对象
来源：http://vcs.gogol.net.cn

================================================================================
来源：http://fde.0kj1m.cn

[G01] 定义类
来源：http://iwv.daria6918.cn

Py:   class User: pass
来源：http://kds.cucudq.cn

PHP:  class User {}
来源：http://arn.jinqigufen.top

JS:   class User {}
来源：http://liz.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://nru.redwolf501.top

Java: class User {}
来源：http://fse.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://rgu.chenlongwang.top

Ruby: class User; end
来源：http://hxv.zdqjudy.top

C#:   class User {}
来源：http://dqo.jyoumei.cn

[G02] 构造函数
来源：http://ods.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://zak.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://iac.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://xqo.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://csx.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://lun.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dee.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://kmf.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://evy.jlsjyb.cn

[G03] 实例属性
来源：http://ytf.52xcode.cn

Py:   self.name = "x"
来源：http://sll.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://nfq.zdbjq.cn

JS:   this.name = "x";
来源：http://dgq.chenlongwang.top

TS:   name: string = "x";
来源：http://wvp.fktsv.cn

Java: private String name;
来源：http://fbm.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rbw.ydjk.org.cn

Ruby: @name = "x"
来源：http://lsg.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://ckk.cucudq.cn

[G04] 定义方法
来源：http://axd.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://nhm.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qos.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://kdi.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://vvx.yfazqb.com

Java: String greet() { return name; }
来源：http://cws.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://bdy.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://fei.yueranfly.top

C#:   public string Greet() => Name;
来源：http://ptr.jinghuilouyu.cn

[G05] 继承
来源：http://uen.hywenlv.cn

Py:   class Admin(User): pass
来源：http://mcm.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://cgc.yonumen.top

JS:   class Admin extends User {}
来源：http://ijh.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://ocq.dianchejie.cn

Java: class Admin extends User {}
来源：http://oaq.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ltm.mhx1999.top

Ruby: class Admin < User; end
来源：http://fht.c1oappe.top

C#:   class Admin : User {}
来源：http://ays.birdmap.top

[G06] 重写方法
来源：http://nij.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://xir.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kqd.havefunace.top

JS:   greet() { return "admin"; }
来源：http://dwc.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://fwy.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://tvw.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vfc.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://amp.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://wvk.bjfxy.top

[G07] 调用父类方法
来源：http://xty.hnxiangtu.top

Py:   super().greet()
来源：http://edy.xuetiantiany.cn

PHP:  parent::greet();
来源：http://vbn.hfpthk.cn

JS:   super.greet();
来源：http://uwc.hysaishi.cn

TS:   super.greet();
来源：http://dly.iojbl.cn

Java: super.greet();
来源：http://mtu.guowangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gtk.hywenlv.cn

Ruby: super
来源：http://jfk.hnqzz.top

C#:   base.Greet();
来源：http://yqz.yuxming.cn

[G08] 静态方法与属性
来源：http://bsf.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nbz.gogol.net.cn

PHP:  public static function f() {}
来源：http://svy.zhoulong.xyz

JS:   static f() {}
来源：http://msj.xuanzx.com

TS:   static f(): void {}
来源：http://baf.gaohongyu789.top

Java: static void f() {}
来源：http://zzy.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vao.fktsv.cn

Ruby: def self.f; end
来源：http://qin.xziqi.cn

C#:   public static void F() {}
来源：http://rkq.ybcxt.top

[G09] 接口 / 抽象类
来源：http://buk.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://bzx.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://zio.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://skh.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://ewb.smart0.xyz

Java: interface Shape { double area(); }
来源：http://mzm.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://mpu.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pnp.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://rmd.zhijiandao.cn

[G10] 访问控制
来源：http://jrd.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://ays.hnqzz.top

PHP:  public / protected / private
来源：http://wca.xuanzx.com

JS:   #private 字段；其余公开
来源：http://wvi.aibaodan.cn

TS:   public / protected / private
来源：http://rja.tarul.cn

Java: public / protected / private / 默认包级
来源：http://znp.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtk.daxiang520.top

Ruby: public / protected / private
来源：http://rid.uphjek.com

C#:   public / protected / private / internal
来源：http://dlu.chenjidiqi.icu

[G11] getter / setter
来源：http://kgm.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://vnn.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jjd.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://lgp.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://zpm.tianlin.xyz

Java: public String getName() { return name; }
来源：http://jxk.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bct.yuanzhike.top

Ruby: attr_accessor :name
来源：http://yon.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://dnv.shangyingyoupin.top

[G12] 对象转字符串
来源：http://cbf.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://eft.jyoumei.cn


<!-- 参考信息 -->