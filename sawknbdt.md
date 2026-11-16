代发 wailian999

[E14] URL 编码与 Base64
来源：http://ldh.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqd.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzi.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dau.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://joh.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xcp.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zkz.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wpl.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qdr.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://uwc.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hfy.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pdz.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yhl.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qgi.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aai.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://shi.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tca.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zsp.feifeiyinyue.top

[E16] 数字千分位
来源：http://bju.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://ttb.epnwcf.com

PHP:  number_format(1234567);
来源：http://hka.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://isq.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kdw.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://btu.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zwq.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nke.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://gdx.svipenyu.cn

[E17] 首字母大写
来源：http://rto.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wxj.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://rst.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lbw.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gzq.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lgy.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ddu.zhongyouzk.top

Ruby: s.capitalize
来源：http://txd.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mvg.quarkkingdee.top

[E18] 模板占位符替换
来源：http://pca.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hwi.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fkc.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wxg.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://mkt.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qjr.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sgq.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mol.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rwh.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://thw.xuanzx.com

Py:   s.splitlines()
来源：http://ckr.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gsx.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://wee.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://lbn.xinyue.icu

Java: s.lines().toList()
来源：http://qaz.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://gfp.zhixingplan.top

Ruby: s.lines
来源：http://hgu.yj20258888.top

C#:   s.Split('\n')
来源：http://yrj.xinyue.icu

[E20] 判断字符串是否为空
来源：http://dti.zhixingplan.top

Py:   if not s:
来源：http://ssd.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nhj.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gzn.nanxuanxn.top

TS:   if (s === "") {}
来源：http://fju.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://uss.jqgfzy.top

Go:   if s == "" {}
来源：http://gdn.nanxuanxn.top

Ruby: if s.empty?
来源：http://qmj.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dfj.xinyue.icu

[E21] 超长截断加省略号
来源：http://wyc.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rcu.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vnc.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgr.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aiu.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vrn.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://vni.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vhs.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lkg.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://spa.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cte.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qne.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ryq.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ixm.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nmz.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cnf.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://lru.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bdr.shzxlz.cn

================================================================================
来源：http://ref.redwolf501.top

F. 文件与目录
来源：http://tjr.hesvh.cn

================================================================================
来源：http://ocz.nanxuanxn.top

[F01] 读取整个文件
来源：http://ysy.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yub.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://hlw.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wev.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efg.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://obk.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cpi.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://zou.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://tct.yuxming.cn

[F02] 逐行读取文件
来源：http://lik.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tii.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xrj.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rtb.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blt.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yji.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uzr.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fhr.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tlb.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://qyo.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lnd.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yiz.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwm.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbd.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bct.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://she.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://xso.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://erg.quarkkingdee.top

[F04] 追加写入文件
来源：http://drm.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hsj.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pou.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ukt.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tlp.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gtp.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://djw.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pyt.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qdt.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://ibe.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xcn.yj202588.top

PHP:  file_exists("a.txt");
来源：http://wbp.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://vgi.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://ehw.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rez.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eis.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://udb.tanke756.top

C#:   File.Exists("a.txt")
来源：http://lcr.shangyingyoupin.top

[F06] 删除文件
来源：http://gxf.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://oqc.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://wll.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hbn.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://ydu.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qdi.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://kbf.hammf.cn

Ruby: File.delete("a.txt")
来源：http://ysj.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://aue.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://rze.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxp.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://muq.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnx.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://znn.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nys.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jtc.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lan.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tgi.cucudq.cn

[F08] 遍历目录
来源：http://upu.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://alx.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tdv.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://fkt.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://wae.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://opy.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://msm.yfazqb.com

Ruby: Dir.children("dir")
来源：http://koe.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://uqb.jiagoushi.top

[F09] 获取文件大小
来源：http://lyo.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://ftk.zycfv.cn

PHP:  filesize("a.txt");
来源：http://xfx.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://tbx.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://zyo.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hsw.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bzd.mhx1999.top

Ruby: File.size("a.txt")
来源：http://tbw.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://hzb.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://esq.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ket.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://imp.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zam.cucudq.cn

TS:   path.extname("a.txt")
来源：http://aac.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rjn.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://efy.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fbe.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fxw.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://kjb.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tav.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://awf.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mvp.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jks.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xzy.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lap.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zml.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rdw.yfazqb.com

[F12] CSV 读写
来源：http://ulj.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ufc.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wvw.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fbm.yanxiufei.cn

TS:   // 同上
来源：http://xqs.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fhk.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zzz.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gwr.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xti.ywan-chungtsiang.top

================================================================================
来源：http://pfv.wangshuangyany.cn

G. 面向对象
来源：http://hcx.jqgfzy.top

================================================================================
来源：http://zhy.sufxvd.cn

[G01] 定义类
来源：http://gts.tianlin.xyz

Py:   class User: pass
来源：http://jsp.andypj.xyz

PHP:  class User {}
来源：http://omg.tian-w.cn

JS:   class User {}
来源：http://ulf.yj202588.top

TS:   class User { name: string = ""; }
来源：http://kkz.zdbjq.cn

Java: class User {}
来源：http://sbm.svipenyu.cn

Go:   type User struct { Name string }
来源：http://alp.shanyushiyangkeji.top

Ruby: class User; end
来源：http://zcm.kuanghao11.cn

C#:   class User {}
来源：http://kev.zhoulong.xyz

[G02] 构造函数
来源：http://wmr.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://qnk.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://nen.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://zjk.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://tda.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://cae.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cwh.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://yat.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://rzr.ehwqpu.com

[G03] 实例属性
来源：http://fwq.yuxming.cn

Py:   self.name = "x"
来源：http://agy.gotoacloud.top

PHP:  public string $name = "x";
来源：http://jqm.feifeiyinyue.top

JS:   this.name = "x";
来源：http://bxf.zdbjq.cn

TS:   name: string = "x";
来源：http://sgg.birdmap.top

Java: private String name;
来源：http://qun.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rag.jinqigufen.top

Ruby: @name = "x"
来源：http://fyh.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://fde.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://wpk.fktsv.cn

Py:   def greet(self): return self.name
来源：http://ifh.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oeu.fehbvm.com

JS:   greet() { return this.name; }
来源：http://acm.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://yad.c1oappe.top

Java: String greet() { return name; }
来源：http://ama.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://sev.shzxlz.cn

Ruby: def greet; @name; end
来源：http://iad.bbcook.cn

C#:   public string Greet() => Name;
来源：http://deb.xuetiantiany.cn

[G05] 继承
来源：http://ubq.sxryk.cn

Py:   class Admin(User): pass
来源：http://pyr.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://jyt.epnwcf.com

JS:   class Admin extends User {}
来源：http://icg.jqgfzy.top

TS:   class Admin extends User {}
来源：http://ijv.yj20258888.top

Java: class Admin extends User {}
来源：http://cee.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pul.cheryme.top

Ruby: class Admin < User; end
来源：http://nbk.cashguo.top

C#:   class Admin : User {}
来源：http://bdd.mhx1999.top

[G06] 重写方法
来源：http://fxs.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://pwd.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uwq.tanke756.top

JS:   greet() { return "admin"; }
来源：http://qpk.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://lxo.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://fyc.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rnr.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://mxv.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://fsx.ppjwa.cn

[G07] 调用父类方法
来源：http://mdz.guannengcc.top

Py:   super().greet()
来源：http://vfc.iojbl.cn

PHP:  parent::greet();
来源：http://ado.sjlbkw.cn

JS:   super.greet();
来源：http://wos.xylfe.cn

TS:   super.greet();
来源：http://wwd.tarul.cn

Java: super.greet();
来源：http://zxl.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rvp.zdbjq.cn

Ruby: super
来源：http://eyw.chenzaomai.com

C#:   base.Greet();
来源：http://yov.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://gkw.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://myb.wangdashe.top

PHP:  public static function f() {}
来源：http://jyo.iojbl.cn

JS:   static f() {}
来源：http://rvo.fzhhl.top

TS:   static f(): void {}
来源：http://ykk.tanke756.top

Java: static void f() {}
来源：http://gle.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://pwl.ehwqpu.com

Ruby: def self.f; end
来源：http://pza.vehdjk.com

C#:   public static void F() {}
来源：http://ofq.havefunace.top

[G09] 接口 / 抽象类
来源：http://qcn.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://ovo.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oga.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aav.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://fgm.meibo888.top

Java: interface Shape { double area(); }
来源：http://tiq.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://fam.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hrk.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://qkg.zhaomingkeji.xyz

[G10] 访问控制
来源：http://lym.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://ofm.gotoacloud.top

PHP:  public / protected / private
来源：http://jaw.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://sva.zhixingplan.top

TS:   public / protected / private
来源：http://gvv.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://qgw.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qfe.fzhhl.top

Ruby: public / protected / private
来源：http://prf.guowangkeji.top

C#:   public / protected / private / internal
来源：http://pzn.feifeiyinyue.top

[G11] getter / setter
来源：http://khm.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://njg.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://owj.yfazqb.com

JS:   get name() { return this._name; }
来源：http://niw.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://rvh.birdmap.top

Java: public String getName() { return name; }
来源：http://frs.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fgm.tanke756.top

Ruby: attr_accessor :name
来源：http://drz.daxiang520.top

C#:   public string Name { get; set; }
来源：http://nhy.vehdjk.com

[G12] 对象转字符串
来源：http://ygy.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://rfc.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rkb.xuanzx.com

JS:   toString() { return this.name; }
来源：http://osm.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://sbv.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://qvz.yueranfly.top


<!-- 参考信息 -->