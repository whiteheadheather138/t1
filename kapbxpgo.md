代发 wailian999

[E14] URL 编码与 Base64
来源：http://fhn.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pxk.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vfz.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rdk.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wqb.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iof.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ach.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jad.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zet.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://aim.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ajv.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vji.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lqu.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ncx.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lpp.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uwh.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vts.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jer.aibaodan.cn

[E16] 数字千分位
来源：http://wsc.sxryk.cn

Py:   f"{1234567:,}"
来源：http://tpo.jinqigufen.top

PHP:  number_format(1234567);
来源：http://vam.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://iul.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iox.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pun.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kgf.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xrx.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://mcc.dianchejie.cn

[E17] 首字母大写
来源：http://zkf.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://axb.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://svu.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qyf.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajq.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gyt.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ncn.aizwys.cn

Ruby: s.capitalize
来源：http://dlc.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bjh.dianchejie.cn

[E18] 模板占位符替换
来源：http://ycd.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yix.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hyj.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://twx.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cnj.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uvv.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oil.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wyv.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nsi.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://lfe.gaohongyu789.top

Py:   s.splitlines()
来源：http://uzv.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zjd.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://llq.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://bdv.haohaochexian.top

Java: s.lines().toList()
来源：http://xxm.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://pqt.zycfv.cn

Ruby: s.lines
来源：http://pkg.hcnkem.com

C#:   s.Split('\n')
来源：http://uzm.sysykeji.top

[E20] 判断字符串是否为空
来源：http://vlp.xinyue.icu

Py:   if not s:
来源：http://cnx.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fol.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://utz.meibo888.top

TS:   if (s === "") {}
来源：http://qsz.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://kwj.andypj.xyz

Go:   if s == "" {}
来源：http://iwc.zhongyouzk.top

Ruby: if s.empty?
来源：http://wrg.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gnc.bjfxy.top

[E21] 超长截断加省略号
来源：http://uep.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llv.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fwa.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfq.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cqo.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lfh.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://esz.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kof.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://her.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://ees.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ftg.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfg.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wps.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gtq.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jim.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jez.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://vls.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zov.vehdjk.com

================================================================================
来源：http://ddd.jyoumei.cn

F. 文件与目录
来源：http://mcz.yvedp.cn

================================================================================
来源：http://sie.meibo888.top

[F01] 读取整个文件
来源：http://xsq.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://msf.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://djz.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fvg.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qbs.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qts.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://plm.cashguo.top

Ruby: File.read("a.txt")
来源：http://odk.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://rxu.bbcook.cn

[F02] 逐行读取文件
来源：http://zub.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csf.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ury.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxs.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpu.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tmg.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rhh.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dqj.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pye.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://rhl.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzs.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tih.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nne.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vru.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sxh.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vix.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://qhx.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fwe.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://zpo.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kfc.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vsi.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xnq.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyq.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mqe.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://umn.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vym.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fuv.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://cri.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pow.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://tmc.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://zrl.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://zfd.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qdo.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://orc.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://lme.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://czp.ydzc1.top

[F06] 删除文件
来源：http://jap.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://ybo.sweek.top

PHP:  unlink("a.txt");
来源：http://pke.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://sin.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://esu.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hku.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://bzo.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://ijf.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://thw.sweek.top

[F07] 创建目录（含多级）
来源：http://acp.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://out.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wjb.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://euq.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spd.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gfp.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gkv.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ekm.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dyq.feifeiyinyue.top

[F08] 遍历目录
来源：http://kza.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xtm.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ryz.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://uwi.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://mst.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://poy.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wob.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://liz.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://ydc.yfazqb.com

[F09] 获取文件大小
来源：http://tzi.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://npq.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://jyb.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://rcn.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://pcd.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://kjf.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lfq.bjfxy.top

Ruby: File.size("a.txt")
来源：http://ggh.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://dpr.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://svm.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://irb.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pev.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gnl.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://vof.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mrl.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://egg.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mes.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hzd.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://bvd.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xyx.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qjj.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xzo.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rkl.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kma.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lyo.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jfc.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wfm.jiagoushi.top

[F12] CSV 读写
来源：http://ixf.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jvv.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://buq.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kgg.cheryme.top

TS:   // 同上
来源：http://fvw.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lhb.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vxp.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ifc.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rdx.aibaodan.cn

================================================================================
来源：http://fjb.yvedp.cn

G. 面向对象
来源：http://oax.andypj.xyz

================================================================================
来源：http://mym.yj20258.top

[G01] 定义类
来源：http://kcg.ywan-chungtsiang.top

Py:   class User: pass
来源：http://fba.yanxiufei.cn

PHP:  class User {}
来源：http://meg.jlsjyb.cn

JS:   class User {}
来源：http://xff.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://ebn.wangshuangyany.cn

Java: class User {}
来源：http://wpv.shuidangran.top

Go:   type User struct { Name string }
来源：http://kwh.fehbvm.com

Ruby: class User; end
来源：http://cnb.gotoacloud.top

C#:   class User {}
来源：http://qkr.fzhhl.top

[G02] 构造函数
来源：http://rhe.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://ycq.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://abv.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://aew.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://upi.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://tit.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aeo.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://mgj.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://kpz.yj20258.top

[G03] 实例属性
来源：http://gtw.xinyue.icu

Py:   self.name = "x"
来源：http://eme.gogol.net.cn

PHP:  public string $name = "x";
来源：http://uxo.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://jej.ppjwa.cn

TS:   name: string = "x";
来源：http://vwd.mhx1999.top

Java: private String name;
来源：http://wfj.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hbp.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://tlx.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://iuq.shangyingyoupin.top

[G04] 定义方法
来源：http://agn.bjfxy.top

Py:   def greet(self): return self.name
来源：http://hfq.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://byn.wangdashe.top

JS:   greet() { return this.name; }
来源：http://eab.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://sbt.gaohongyu789.top

Java: String greet() { return name; }
来源：http://xsy.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gxq.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://ztd.yvedp.cn

C#:   public string Greet() => Name;
来源：http://qdp.tanke756.top

[G05] 继承
来源：http://lre.svipenyu.cn

Py:   class Admin(User): pass
来源：http://vkm.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://esc.yuanzhike.top

JS:   class Admin extends User {}
来源：http://sfx.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://pvc.guowangkeji.top

Java: class Admin extends User {}
来源：http://hhv.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iii.yongpay.top

Ruby: class Admin < User; end
来源：http://omv.shzxlz.cn

C#:   class Admin : User {}
来源：http://dcj.aibaodan.cn

[G06] 重写方法
来源：http://kes.yongpay.top

Py:   def greet(self): return "admin"
来源：http://hmj.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://fms.birdmap.top

JS:   greet() { return "admin"; }
来源：http://gcc.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://njl.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://thr.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lqy.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://qki.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://rgz.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://spm.zycfv.cn

Py:   super().greet()
来源：http://sjp.chenzaomai.com

PHP:  parent::greet();
来源：http://hjs.yueranfly.top

JS:   super.greet();
来源：http://bjb.sufxvd.cn

TS:   super.greet();
来源：http://fdm.wangdashe.top

Java: super.greet();
来源：http://sqs.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://syi.fengsongda.top

Ruby: super
来源：http://ehr.nwbrower.top

C#:   base.Greet();
来源：http://sne.ydzc1.top

[G08] 静态方法与属性
来源：http://gpy.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iwz.yueranfly.top

PHP:  public static function f() {}
来源：http://fki.tarul.cn

JS:   static f() {}
来源：http://nln.snrcjt.cn

TS:   static f(): void {}
来源：http://geg.birdmap.top

Java: static void f() {}
来源：http://mhj.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibn.yuxming.cn

Ruby: def self.f; end
来源：http://dil.yvedp.cn

C#:   public static void F() {}
来源：http://gch.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://cpv.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://nxt.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://gxu.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ltd.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://qst.hammf.cn

Java: interface Shape { double area(); }
来源：http://zvg.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://wmr.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jgd.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://vpw.fzhhl.top

[G10] 访问控制
来源：http://acy.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://wpp.aizwys.cn

PHP:  public / protected / private
来源：http://dvq.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://iac.gogol.net.cn

TS:   public / protected / private
来源：http://ogh.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://uwe.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ulk.zhiwuduotai.top

Ruby: public / protected / private
来源：http://qfe.tanke756.top

C#:   public / protected / private / internal
来源：http://joz.gzhubu.top

[G11] getter / setter
来源：http://zqp.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://dwu.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://iqv.yvedp.cn

JS:   get name() { return this._name; }
来源：http://zhs.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://qcc.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://nzt.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zho.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://uuw.daria6918.cn

C#:   public string Name { get; set; }
来源：http://ive.sjlbkw.cn

[G12] 对象转字符串
来源：http://zwj.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://pnd.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rso.sxryk.cn

JS:   toString() { return this.name; }
来源：http://dix.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://lgt.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://gzg.ybcxt.top


<!-- 参考信息 -->