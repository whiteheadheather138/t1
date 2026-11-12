代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zek.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pdq.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ixh.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jdd.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://dla.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sah.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://btg.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jor.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ppk.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bfc.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lez.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bej.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dvg.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://duk.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ehy.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hci.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eyw.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://szb.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nrk.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://khq.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nqs.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nbl.svipenyu.cn

[E16] 数字千分位
来源：http://sco.yonumen.top

Py:   f"{1234567:,}"
来源：http://sxb.aizwys.cn

PHP:  number_format(1234567);
来源：http://fyh.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gsa.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eta.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lne.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hzl.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ywb.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://oqy.daria6918.cn

[E17] 首字母大写
来源：http://nhy.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://poh.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ohs.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ktu.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aze.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qyz.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ltd.hammf.cn

Ruby: s.capitalize
来源：http://spr.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lni.yvedp.cn

[E18] 模板占位符替换
来源：http://yrj.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mnb.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ahp.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ybz.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kzd.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ikl.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vay.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wdb.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tlt.fktsv.cn

[E19] 多行文本按行拆分
来源：http://ucp.jinqigfzy.top

Py:   s.splitlines()
来源：http://vzp.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kts.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://hin.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://qut.ivvv.top

Java: s.lines().toList()
来源：http://ufo.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://vzd.ivvv.top

Ruby: s.lines
来源：http://dqt.ybcxt.top

C#:   s.Split('\n')
来源：http://bje.daxiang520.top

[E20] 判断字符串是否为空
来源：http://zip.andypj.xyz

Py:   if not s:
来源：http://ojo.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mjf.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fet.wangdashe.top

TS:   if (s === "") {}
来源：http://asa.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://xcy.xuetiantiany.cn

Go:   if s == "" {}
来源：http://spm.yj20258888.top

Ruby: if s.empty?
来源：http://rij.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ngy.yj20258888.top

[E21] 超长截断加省略号
来源：http://bxe.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ysv.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ppm.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fwt.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hkv.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nfq.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://zyg.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://toc.fktsv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gqp.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://ktd.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hmv.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwe.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkr.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ers.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gny.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hwr.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://mrz.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://snt.guannengcc.top

================================================================================
来源：http://hth.hammf.cn

F. 文件与目录
来源：http://eyp.fanxiaobao.xyz

================================================================================
来源：http://sxl.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://ijm.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tgs.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://ual.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lxi.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vwq.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tmc.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rcl.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://cbo.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://ldp.sjlbkw.cn

[F02] 逐行读取文件
来源：http://dtw.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tup.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gvw.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://anz.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjs.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vjl.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oao.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wqm.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cnw.yongpay.top

[F03] 写入文件（覆盖）
来源：http://eau.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fin.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dkj.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ekt.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://otd.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gpn.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qfv.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://ttq.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xdi.yanxiufei.cn

[F04] 追加写入文件
来源：http://qah.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hon.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://unz.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwq.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kso.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgy.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://utm.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sms.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oms.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://jxs.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vgu.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://yhv.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://djz.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://esz.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nut.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kbo.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://pgj.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://htj.ppjwa.cn

[F06] 删除文件
来源：http://kuq.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://zqp.yongpay.top

PHP:  unlink("a.txt");
来源：http://lgv.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://ykz.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://isb.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eae.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://miw.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://zpa.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://bjs.wangdashe.top

[F07] 创建目录（含多级）
来源：http://wsw.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jjw.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gjk.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xst.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwv.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ncu.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gcn.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pud.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fud.sxryk.cn

[F08] 遍历目录
来源：http://iim.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zye.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qnz.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://hun.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://wzf.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oib.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dqx.fzhhl.top

Ruby: Dir.children("dir")
来源：http://ofv.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://hfs.52xcode.cn

[F09] 获取文件大小
来源：http://qrb.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://vot.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://opu.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://oao.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://qot.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fpe.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kxm.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://ucx.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://nnu.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://yks.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dff.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://epa.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cgy.tian-w.cn

TS:   path.extname("a.txt")
来源：http://lrx.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://smo.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ahb.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hjk.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yvq.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://pag.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pxe.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xjy.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wsh.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyy.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tfo.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nzm.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://his.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://myo.ydzc1.top

[F12] CSV 读写
来源：http://hku.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aed.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cbx.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pqm.wangshuangyany.cn

TS:   // 同上
来源：http://hgs.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vcr.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vkw.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ccr.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bgm.ctjpmb.com

================================================================================
来源：http://xrx.jianghu66.top

G. 面向对象
来源：http://hgx.ywan-chungtsiang.top

================================================================================
来源：http://eks.0kj1m.cn

[G01] 定义类
来源：http://fyd.shangyingyoupin.top

Py:   class User: pass
来源：http://yks.sysykeji.top

PHP:  class User {}
来源：http://zid.nanxinkj.top

JS:   class User {}
来源：http://eoo.yonumen.top

TS:   class User { name: string = ""; }
来源：http://ibb.aibaodan.cn

Java: class User {}
来源：http://fhl.chenlongwang.top

Go:   type User struct { Name string }
来源：http://tzc.xziqi.cn

Ruby: class User; end
来源：http://gum.hnxiangtu.top

C#:   class User {}
来源：http://ktu.xuanzx.com

[G02] 构造函数
来源：http://inv.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://tag.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://dlx.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://wcq.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://swx.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://blx.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sgi.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://mld.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://phc.zdbjq.cn

[G03] 实例属性
来源：http://iih.mhx1999.top

Py:   self.name = "x"
来源：http://rdf.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://dht.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://fds.ivvv.top

TS:   name: string = "x";
来源：http://avb.ppjwa.cn

Java: private String name;
来源：http://fop.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zok.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://uvs.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://uek.hnqzz.top

[G04] 定义方法
来源：http://pca.pycfn.com

Py:   def greet(self): return self.name
来源：http://pbc.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dwg.yueranfly.top

JS:   greet() { return this.name; }
来源：http://ocl.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://fuf.nanxinkj.top

Java: String greet() { return name; }
来源：http://ttt.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lxr.xylfe.cn

Ruby: def greet; @name; end
来源：http://kbx.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://bha.cdnleiting.top

[G05] 继承
来源：http://znw.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://jnh.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://zgk.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://mos.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://qmp.shuidangran.top

Java: class Admin extends User {}
来源：http://ljv.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yby.hcnkem.com

Ruby: class Admin < User; end
来源：http://wwo.sxryk.cn

C#:   class Admin : User {}
来源：http://hzf.xinyue.icu

[G06] 重写方法
来源：http://wyp.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://fuj.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://swu.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://wsb.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://kls.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://jqj.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kgh.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://hqd.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://urg.tarul.cn

[G07] 调用父类方法
来源：http://hbr.jyoumei.cn

Py:   super().greet()
来源：http://xfg.meibo888.top

PHP:  parent::greet();
来源：http://azl.aizwys.cn

JS:   super.greet();
来源：http://wzl.jinqigufen.top

TS:   super.greet();
来源：http://tbe.jinghuilouyu.cn

Java: super.greet();
来源：http://hms.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nmt.chenjidiqi.icu

Ruby: super
来源：http://gss.gaohongyu789.top

C#:   base.Greet();
来源：http://xvv.aibaodan.cn

[G08] 静态方法与属性
来源：http://hbv.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lfg.0kj1m.cn

PHP:  public static function f() {}
来源：http://xnp.bbcook.cn

JS:   static f() {}
来源：http://xsx.shzxlz.cn

TS:   static f(): void {}
来源：http://zbr.ydjk.org.cn

Java: static void f() {}
来源：http://pdi.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sza.hysaishi.cn

Ruby: def self.f; end
来源：http://nmh.guannengcc.top

C#:   public static void F() {}
来源：http://udu.fengsongda.top

[G09] 接口 / 抽象类
来源：http://hfg.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://awm.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nyn.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cgu.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://mhl.xinyue.icu

Java: interface Shape { double area(); }
来源：http://qsf.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://fjn.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eva.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://ybn.zhixingplan.top

[G10] 访问控制
来源：http://pqh.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://jpo.dianchejie.cn

PHP:  public / protected / private
来源：http://ilh.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://ljq.tarul.cn

TS:   public / protected / private
来源：http://sng.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://hiv.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qqk.ydzc1.top

Ruby: public / protected / private
来源：http://iac.zdbjq.cn

C#:   public / protected / private / internal
来源：http://nuc.cdnleiting.top

[G11] getter / setter
来源：http://igx.mhx1999.top

Py:   @property 与 @x.setter
来源：http://ccu.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ilw.yj20258888.top

JS:   get name() { return this._name; }
来源：http://seh.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://whb.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://lju.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://lyg.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://vdw.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://rxz.yueranfly.top

[G12] 对象转字符串
来源：http://flw.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://xqy.zhiwuduotai.top


<!-- 参考信息 -->