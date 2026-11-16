代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yjj.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zym.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jvb.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mox.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://wud.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qrj.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://vvj.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cdm.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cxm.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jnm.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mlc.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xft.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pdg.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://tae.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qud.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ned.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nur.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ktj.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kbo.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hax.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://flx.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hfn.zhengqikj.top

[E16] 数字千分位
来源：http://hyg.xuanzx.com

Py:   f"{1234567:,}"
来源：http://zqf.hammf.cn

PHP:  number_format(1234567);
来源：http://kvq.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rtc.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://haq.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hya.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ljb.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kwo.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://bka.tarul.cn

[E17] 首字母大写
来源：http://zib.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rrc.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ici.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kjn.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dgi.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jvi.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lkg.jqgufenzy.top

Ruby: s.capitalize
来源：http://xox.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sck.ctjpmb.com

[E18] 模板占位符替换
来源：http://slg.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ewi.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mah.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ebz.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kmt.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wie.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bqh.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://beu.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://avq.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://qwi.jinqigufen.top

Py:   s.splitlines()
来源：http://ifk.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zot.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://eiv.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://zpz.bbcook.cn

Java: s.lines().toList()
来源：http://liq.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://ape.ydzc1.top

Ruby: s.lines
来源：http://hlc.hesvh.cn

C#:   s.Split('\n')
来源：http://pag.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://mxz.tarul.cn

Py:   if not s:
来源：http://nxq.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sat.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mfl.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://aeq.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://rsw.jianghu66.top

Go:   if s == "" {}
来源：http://ibd.chenjidiqi.icu

Ruby: if s.empty?
来源：http://yxd.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wng.vehdjk.com

[E21] 超长截断加省略号
来源：http://nnw.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xgw.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ngb.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://feb.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ffz.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rht.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://grb.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xbb.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://efs.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://fft.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pgj.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cvx.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkg.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrw.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tjm.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ohm.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://dif.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zmv.gotoacloud.top

================================================================================
来源：http://ybv.cheryme.top

F. 文件与目录
来源：http://lcw.ppjwa.cn

================================================================================
来源：http://usc.ydzc1.top

[F01] 读取整个文件
来源：http://ktd.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tne.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://joe.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wyu.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jhm.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pxn.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kst.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://oxt.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://rld.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://rjm.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nug.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kbq.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wag.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yyu.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xhb.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zlv.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kqz.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pvp.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://ruz.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://prw.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kgq.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sez.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzo.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xhc.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ake.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://twg.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pnt.smart0.xyz

[F04] 追加写入文件
来源：http://pru.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://esh.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://reg.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eno.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wda.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bin.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pnj.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ihz.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ywd.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://wht.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://efk.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://syw.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://wkl.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://csw.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://poc.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mtz.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://mgk.havefunace.top

C#:   File.Exists("a.txt")
来源：http://nci.xuetiantiany.cn

[F06] 删除文件
来源：http://eol.sysykeji.top

Py:   os.remove("a.txt")
来源：http://gfc.cashguo.top

PHP:  unlink("a.txt");
来源：http://rre.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://fsf.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://rsn.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uuq.cheryme.top

Go:   os.Remove("a.txt")
来源：http://jkw.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://ofu.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://ylp.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://ypu.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mdn.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yzw.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://slh.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esm.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfa.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oza.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oql.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blr.yangfankeji.com

[F08] 遍历目录
来源：http://avg.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yor.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qbl.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://gzl.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://boe.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ekd.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xqr.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://jac.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://uvj.sxryk.cn

[F09] 获取文件大小
来源：http://yfr.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://zjt.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://jhb.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://wzq.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://izn.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://oua.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fie.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://zfn.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://doq.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://chp.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yah.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oby.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://klb.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://lyh.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wdz.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vxf.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yas.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://idx.zycfv.cn

[F11] 复制与移动文件
来源：http://jkg.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lwe.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oht.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ign.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgc.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qzc.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rgv.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tyt.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tcz.birdmap.top

[F12] CSV 读写
来源：http://byu.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nbb.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ejv.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kuc.sysykeji.top

TS:   // 同上
来源：http://vod.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pjn.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://djf.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xzq.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dfe.nanxinkj.top

================================================================================
来源：http://ehq.guannengcc.top

G. 面向对象
来源：http://zrb.chenjidiqi.icu

================================================================================
来源：http://bmh.hongshengwenyu.top

[G01] 定义类
来源：http://dij.yuxming.cn

Py:   class User: pass
来源：http://ncw.redwolf501.top

PHP:  class User {}
来源：http://gfo.gaohongyu789.top

JS:   class User {}
来源：http://pby.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://mju.snrcjt.cn

Java: class User {}
来源：http://fnt.dianchejie.cn

Go:   type User struct { Name string }
来源：http://slj.ivvv.top

Ruby: class User; end
来源：http://syn.ydzc1.top

C#:   class User {}
来源：http://ryr.0kj1m.cn

[G02] 构造函数
来源：http://ctu.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://wlm.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://pci.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://zff.yongpay.top

TS:   constructor(public name: string) {}
来源：http://aev.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://cuu.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gls.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://tfg.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://qco.aizwys.cn

[G03] 实例属性
来源：http://owb.yj20258.top

Py:   self.name = "x"
来源：http://zpe.chenzaomai.com

PHP:  public string $name = "x";
来源：http://klb.0kj1m.cn

JS:   this.name = "x";
来源：http://ifi.bbcook.cn

TS:   name: string = "x";
来源：http://vov.yueranfly.top

Java: private String name;
来源：http://juz.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dpy.dashuyun.cn

Ruby: @name = "x"
来源：http://oat.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://ycz.zhijiandao.cn

[G04] 定义方法
来源：http://fuh.sysykeji.top

Py:   def greet(self): return self.name
来源：http://lrq.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sor.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://wjx.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://bsu.bjfxy.top

Java: String greet() { return name; }
来源：http://vla.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://efg.ydzc1.top

Ruby: def greet; @name; end
来源：http://nxk.aizwys.cn

C#:   public string Greet() => Name;
来源：http://fsf.daxiang520.top

[G05] 继承
来源：http://yqz.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://csp.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://eud.haohaochexian.top

JS:   class Admin extends User {}
来源：http://han.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://wjn.dianchejie.cn

Java: class Admin extends User {}
来源：http://wki.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qbz.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://gvh.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://kuo.bbcook.cn

[G06] 重写方法
来源：http://pea.tanke756.top

Py:   def greet(self): return "admin"
来源：http://yzz.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uju.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://bsk.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://ivn.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://nzs.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgj.pycfn.com

Ruby: def greet; "admin"; end
来源：http://lux.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://qjx.yuxming.cn

[G07] 调用父类方法
来源：http://aum.dianchejie.cn

Py:   super().greet()
来源：http://xbn.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://kkr.xuetiantiany.cn

JS:   super.greet();
来源：http://jhs.zhongyouzk.top

TS:   super.greet();
来源：http://btp.tian-w.cn

Java: super.greet();
来源：http://udz.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yvu.xuetiantiany.cn

Ruby: super
来源：http://wvt.mhx1999.top

C#:   base.Greet();
来源：http://nqh.gogol.net.cn

[G08] 静态方法与属性
来源：http://bbd.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bad.ivvv.top

PHP:  public static function f() {}
来源：http://mmk.ppjwa.cn

JS:   static f() {}
来源：http://snm.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://dui.yuxming.cn

Java: static void f() {}
来源：http://cld.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://raa.hongshengwenyu.top

Ruby: def self.f; end
来源：http://joo.iojbl.cn

C#:   public static void F() {}
来源：http://uth.andypj.xyz

[G09] 接口 / 抽象类
来源：http://nxs.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://upi.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://mfq.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pkc.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://fpy.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://ldy.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://yro.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ddo.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://zgf.fzhhl.top

[G10] 访问控制
来源：http://sot.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://smi.cashguo.top

PHP:  public / protected / private
来源：http://wqh.birdmap.top

JS:   #private 字段；其余公开
来源：http://qpq.vqdsnc.cn

TS:   public / protected / private
来源：http://vqt.cashguo.top

Java: public / protected / private / 默认包级
来源：http://bcc.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xpq.shzxlz.cn

Ruby: public / protected / private
来源：http://ril.pycfn.com

C#:   public / protected / private / internal
来源：http://eiy.gaohongyu789.top

[G11] getter / setter
来源：http://zrp.hammf.cn

Py:   @property 与 @x.setter
来源：http://bni.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kcm.epnwcf.com

JS:   get name() { return this._name; }
来源：http://ksw.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://hrd.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://spy.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://noy.fengsongda.top

Ruby: attr_accessor :name
来源：http://svv.fengsongda.top

C#:   public string Name { get; set; }
来源：http://nmb.fzhhl.top

[G12] 对象转字符串
来源：http://xmr.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://dzo.cucudq.cn


<!-- 参考信息 -->