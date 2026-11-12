代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yov.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rvj.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://phl.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cfm.mhx1999.top

[E14] URL 编码与 Base64
来源：http://ipv.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cqv.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://kav.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tvz.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nom.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://coh.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jgt.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dlb.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sxs.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://xcp.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://web.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kac.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eub.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ghe.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vne.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bwy.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fyj.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wta.shangyingyoupin.top

[E16] 数字千分位
来源：http://sog.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://omu.cucudq.cn

PHP:  number_format(1234567);
来源：http://xjw.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dyl.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jzx.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xum.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eku.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jqb.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://xzv.nanxuanxn.top

[E17] 首字母大写
来源：http://vzz.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jcz.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nzv.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkn.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eqd.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tjy.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hiz.0kj1m.cn

Ruby: s.capitalize
来源：http://eeb.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aiw.meibo888.top

[E18] 模板占位符替换
来源：http://wby.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://led.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://biz.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://giu.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://exl.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lxa.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jwj.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://upr.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uod.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://avh.gotoacloud.top

Py:   s.splitlines()
来源：http://keg.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yko.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://ipw.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://oqw.gogol.net.cn

Java: s.lines().toList()
来源：http://bjk.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://skc.aizwys.cn

Ruby: s.lines
来源：http://cps.zycfv.cn

C#:   s.Split('\n')
来源：http://ynb.xinyue.icu

[E20] 判断字符串是否为空
来源：http://dzy.yangfankeji.com

Py:   if not s:
来源：http://awu.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sop.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kyy.sysykeji.top

TS:   if (s === "") {}
来源：http://vrp.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://ywq.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://xvn.sxryk.cn

Ruby: if s.empty?
来源：http://bwe.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://psi.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://dzm.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ghc.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lmm.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://odl.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cly.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hmt.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://cnq.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mci.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hvs.fehbvm.com

[E22] 字节长度与字符长度
来源：http://mep.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fnw.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rnk.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mmk.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfe.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nne.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gbq.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://ivn.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ccb.shanyushiyangtech.top

================================================================================
来源：http://qcs.guannengcc.top

F. 文件与目录
来源：http://sgu.hywenlv.cn

================================================================================
来源：http://gcc.ydzc1.top

[F01] 读取整个文件
来源：http://hjv.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jpo.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://jid.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ewj.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bdh.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xzp.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iwi.cheryme.top

Ruby: File.read("a.txt")
来源：http://vhz.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://ssl.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://ffb.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zty.jinqigufen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tll.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://phn.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fow.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kpx.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qcy.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dzt.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfv.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://rca.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hfw.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rmt.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gxo.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmn.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uxw.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zlu.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://ljp.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sub.hysaishi.cn

[F04] 追加写入文件
来源：http://krq.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://anb.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vvn.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgc.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rmw.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://goy.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qlp.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sbf.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jqc.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://rbm.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ufg.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://wdf.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://mgd.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://and.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fuw.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rfj.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://hhr.birdmap.top

C#:   File.Exists("a.txt")
来源：http://zby.jinghuilouyu.cn

[F06] 删除文件
来源：http://znl.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://yed.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://dgz.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://raz.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pym.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ici.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://ncc.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://dej.yj202588.top

C#:   File.Delete("a.txt");
来源：http://ivg.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://aog.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://etb.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nur.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mon.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kdh.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://omx.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vbk.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ksw.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sgh.hnxiangtu.top

[F08] 遍历目录
来源：http://btw.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vjq.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nan.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://htq.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://cvs.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://otx.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://dbo.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://cou.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://gvq.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://mwo.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://dvh.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://fgi.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://cgw.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://obg.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://pev.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hhb.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://seh.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://ieo.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://vnb.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://evw.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xui.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gql.wangdashe.top

TS:   path.extname("a.txt")
来源：http://ksr.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://edr.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iwc.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nbk.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eba.316326.xyz

[F11] 复制与移动文件
来源：http://fvl.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wvv.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ctx.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gtz.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gld.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnv.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jbq.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mgf.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://izj.tanke756.top

[F12] CSV 读写
来源：http://twr.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sit.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vzy.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skf.sjlbkw.cn

TS:   // 同上
来源：http://nzo.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yop.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wnj.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xrq.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ujv.dianchejie.cn

================================================================================
来源：http://gav.yvedp.cn

G. 面向对象
来源：http://bkf.nanxinkj.top

================================================================================
来源：http://rfx.wangdashe.top

[G01] 定义类
来源：http://rgc.ywan-chungtsiang.top

Py:   class User: pass
来源：http://weu.zhiwuduotai.top

PHP:  class User {}
来源：http://alv.yonumen.top

JS:   class User {}
来源：http://wqv.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://eir.316326.xyz

Java: class User {}
来源：http://nse.jqgfzy.top

Go:   type User struct { Name string }
来源：http://elu.hcnkem.com

Ruby: class User; end
来源：http://eem.fehbvm.com

C#:   class User {}
来源：http://glq.nwbrower.top

[G02] 构造函数
来源：http://efe.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://hsz.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://qov.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://bmq.yongpay.top

TS:   constructor(public name: string) {}
来源：http://uwv.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://rjn.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wlm.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://yer.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://zqj.jqgfzy.top

[G03] 实例属性
来源：http://umv.xuetiantiany.cn

Py:   self.name = "x"
来源：http://tyf.316326.xyz

PHP:  public string $name = "x";
来源：http://tdp.redwolf501.top

JS:   this.name = "x";
来源：http://igf.andypj.xyz

TS:   name: string = "x";
来源：http://yii.hysaishi.cn

Java: private String name;
来源：http://tpe.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyg.jyoumei.cn

Ruby: @name = "x"
来源：http://pqq.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://jue.zhaomingkeji.xyz

[G04] 定义方法
来源：http://ikq.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://utz.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://pzm.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://gyc.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://vch.gotoacloud.top

Java: String greet() { return name; }
来源：http://wog.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qtd.yj202588.top

Ruby: def greet; @name; end
来源：http://rri.aizwys.cn

C#:   public string Greet() => Name;
来源：http://kqh.ydjk.org.cn

[G05] 继承
来源：http://iqe.shuidangran.top

Py:   class Admin(User): pass
来源：http://sit.c1oappe.top

PHP:  class Admin extends User {}
来源：http://yxv.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://cqn.svipenyu.cn

TS:   class Admin extends User {}
来源：http://zxe.havefunace.top

Java: class Admin extends User {}
来源：http://heh.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cyx.hesvh.cn

Ruby: class Admin < User; end
来源：http://qiu.cdnleiting.top

C#:   class Admin : User {}
来源：http://psk.ehwqpu.com

[G06] 重写方法
来源：http://aai.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://ygc.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gkv.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://coi.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://wkw.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://qpv.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kfc.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://cej.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://hos.cheryme.top

[G07] 调用父类方法
来源：http://onl.jqgfzy.top

Py:   super().greet()
来源：http://rbq.sweek.top

PHP:  parent::greet();
来源：http://yck.ehwqpu.com

JS:   super.greet();
来源：http://qsw.zhengqikj.top

TS:   super.greet();
来源：http://tmi.meibo888.top

Java: super.greet();
来源：http://xis.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hfa.ctjpmb.com

Ruby: super
来源：http://jwc.cdnleiting.top

C#:   base.Greet();
来源：http://vrr.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://xuz.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dai.ybcxt.top

PHP:  public static function f() {}
来源：http://hcm.birdmap.top

JS:   static f() {}
来源：http://ivb.yueranfly.top

TS:   static f(): void {}
来源：http://ylq.hnqzz.top

Java: static void f() {}
来源：http://kug.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://efe.xinyue.icu

Ruby: def self.f; end
来源：http://ypr.yfazqb.com

C#:   public static void F() {}
来源：http://dns.yueranfly.top

[G09] 接口 / 抽象类
来源：http://ngc.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://ojz.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://sgf.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://tek.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://vdo.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://okw.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://zhk.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ajk.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://drf.jinghuilouyu.cn

[G10] 访问控制
来源：http://zvn.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://moz.0kj1m.cn

PHP:  public / protected / private
来源：http://ttb.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://kst.pengpengdd.cyou

TS:   public / protected / private
来源：http://lii.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://puf.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kls.tian-w.cn

Ruby: public / protected / private
来源：http://sdi.aizwys.cn

C#:   public / protected / private / internal
来源：http://sqr.guowangkeji.top

[G11] getter / setter
来源：http://hyq.havefunace.top

Py:   @property 与 @x.setter
来源：http://aik.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bfx.bbcook.cn

JS:   get name() { return this._name; }
来源：http://ukq.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://rjh.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://bvy.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jji.chenzaomai.com

Ruby: attr_accessor :name
来源：http://qim.yj20258.top

C#:   public string Name { get; set; }
来源：http://njw.fktsv.cn

[G12] 对象转字符串
来源：http://cfi.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://cug.cdnleiting.top


<!-- 参考信息 -->