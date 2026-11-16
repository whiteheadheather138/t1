代发 wailian999

Py:   for ch in s: print(ch)
来源：http://pso.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hng.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://brg.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://vuq.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lhv.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fph.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://xyt.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vkc.yueranfly.top

[E14] URL 编码与 Base64
来源：http://miz.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rin.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://yfp.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lhp.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbv.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzb.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ssf.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gte.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ntw.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://cdf.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://icn.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hek.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cli.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vys.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kml.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ibu.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jzi.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lkg.smart0.xyz

[E16] 数字千分位
来源：http://ccx.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://lwt.meibo888.top

PHP:  number_format(1234567);
来源：http://swu.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tdr.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xqs.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://obs.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebt.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oyp.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://xvx.yongpay.top

[E17] 首字母大写
来源：http://nsu.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tea.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fcn.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzg.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oaf.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jpt.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nom.shzxlz.cn

Ruby: s.capitalize
来源：http://ysx.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rsx.vehdjk.com

[E18] 模板占位符替换
来源：http://xme.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yrg.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://scs.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ojw.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://flb.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuw.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://opk.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://esa.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fqd.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://mmx.9152youxi.cn

Py:   s.splitlines()
来源：http://nen.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qpb.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://yet.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://avx.snrcjt.cn

Java: s.lines().toList()
来源：http://pwf.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://zey.daxiang520.top

Ruby: s.lines
来源：http://vqh.cheryme.top

C#:   s.Split('\n')
来源：http://cks.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://ypf.ctjpmb.com

Py:   if not s:
来源：http://ylk.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wnj.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vtv.guannengcc.top

TS:   if (s === "") {}
来源：http://jeq.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://gev.vqdsnc.cn

Go:   if s == "" {}
来源：http://zdg.sjlbkw.cn

Ruby: if s.empty?
来源：http://ovx.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://osx.tian-w.cn

[E21] 超长截断加省略号
来源：http://xpr.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zel.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cjr.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rtd.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qos.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dyv.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://dur.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://shr.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lrb.daxiang520.top

[E22] 字节长度与字符长度
来源：http://xlc.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqq.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lzr.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfb.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://skk.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bjw.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yia.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://gda.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ftt.gzhubu.top

================================================================================
来源：http://mvy.jinqigufen.top

F. 文件与目录
来源：http://pvk.zhengqikj.top

================================================================================
来源：http://hhm.vqdsnc.cn

[F01] 读取整个文件
来源：http://qwr.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ifs.pengpengdd.cyou

PHP:  file_get_contents("a.txt");
来源：http://lyd.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lwn.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ean.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ojw.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hsw.xuetiantiany.cn

Ruby: File.read("a.txt")
来源：http://boq.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://fwq.zycfv.cn

[F02] 逐行读取文件
来源：http://wzt.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rax.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rvl.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lko.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fiz.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xno.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://csq.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lxe.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqb.birdmap.top

[F03] 写入文件（覆盖）
来源：http://cyc.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgz.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vkj.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbo.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ope.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://avx.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://icm.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://tiz.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nyj.tanke756.top

[F04] 追加写入文件
来源：http://qpo.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbw.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obj.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sow.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlv.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uiw.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wft.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gyn.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://djk.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://qdm.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://erh.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://hlf.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://zjc.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://zca.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pbb.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bau.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://pkh.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://awm.gotoacloud.top

[F06] 删除文件
来源：http://kva.sweek.top

Py:   os.remove("a.txt")
来源：http://jam.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://hma.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://lpr.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://qdq.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rbp.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://lup.yj202588.top

Ruby: File.delete("a.txt")
来源：http://yee.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://yea.fzhhl.top

[F07] 创建目录（含多级）
来源：http://ynq.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nnd.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ytp.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yji.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lat.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bzn.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zac.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nhu.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://phb.jyoumei.cn

[F08] 遍历目录
来源：http://rzx.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fra.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://app.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://hpm.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://nkv.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wgq.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://kat.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://dts.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://otg.epnwcf.com

[F09] 获取文件大小
来源：http://mcz.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://uaw.meibo888.top

PHP:  filesize("a.txt");
来源：http://dsy.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://yuv.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://xpd.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://tpt.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zir.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://mxt.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://yzq.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://epb.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://amu.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oes.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sru.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://fwy.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbh.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kor.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdb.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fbj.yj20258888.top

[F11] 复制与移动文件
来源：http://oee.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://syh.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjk.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hys.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wzd.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vjl.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://roe.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ixf.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://imh.feifeiyinyue.top

[F12] CSV 读写
来源：http://aab.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ojn.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hrf.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rux.dashuyun.cn

TS:   // 同上
来源：http://ukd.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xgf.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://srn.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ook.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wdw.cdnleiting.top

================================================================================
来源：http://pru.feifeiyinyue.top

G. 面向对象
来源：http://gxg.sufxvd.cn

================================================================================
来源：http://ztc.52xcode.cn

[G01] 定义类
来源：http://uzx.hongshengwenyu.top

Py:   class User: pass
来源：http://gva.snrcjt.cn

PHP:  class User {}
来源：http://ljz.snrcjt.cn

JS:   class User {}
来源：http://bfr.yj20258.top

TS:   class User { name: string = ""; }
来源：http://wlc.cucudq.cn

Java: class User {}
来源：http://hnp.havefunace.top

Go:   type User struct { Name string }
来源：http://eve.chenlongwang.top

Ruby: class User; end
来源：http://gae.gzhubu.top

C#:   class User {}
来源：http://ttg.meibo888.top

[G02] 构造函数
来源：http://qld.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://bbe.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://zpy.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://lup.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://hjt.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://ckf.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wzh.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://iti.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://vjy.cashguo.top

[G03] 实例属性
来源：http://xnd.nanxinkj.top

Py:   self.name = "x"
来源：http://ngt.xylfe.cn

PHP:  public string $name = "x";
来源：http://dua.ydjk.org.cn

JS:   this.name = "x";
来源：http://kzp.ydjk.org.cn

TS:   name: string = "x";
来源：http://qvg.mhx1999.top

Java: private String name;
来源：http://scx.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lti.havefunace.top

Ruby: @name = "x"
来源：http://dyd.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://zdo.zhaomingkeji.xyz

[G04] 定义方法
来源：http://uog.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://blt.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://der.jianghu66.top

JS:   greet() { return this.name; }
来源：http://vld.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://obh.nanxuanxn.top

Java: String greet() { return name; }
来源：http://wmo.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vrd.ydzc1.top

Ruby: def greet; @name; end
来源：http://sru.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://dth.nanxinkj.top

[G05] 继承
来源：http://chn.0kj1m.cn

Py:   class Admin(User): pass
来源：http://fbt.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://hgu.yj202588.top

JS:   class Admin extends User {}
来源：http://fuz.yj20258.top

TS:   class Admin extends User {}
来源：http://vra.ivvv.top

Java: class Admin extends User {}
来源：http://xgl.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kmd.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://jpo.zycfv.cn

C#:   class Admin : User {}
来源：http://pul.iojbl.cn

[G06] 重写方法
来源：http://qou.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://lbw.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://sar.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://acy.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://ujn.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://ehc.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bno.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://fjs.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://pgv.xuetiantiany.cn

[G07] 调用父类方法
来源：http://vqj.nanxinkj.top

Py:   super().greet()
来源：http://fwa.wangdashe.top

PHP:  parent::greet();
来源：http://pjj.gogol.net.cn

JS:   super.greet();
来源：http://uwl.bbcook.cn

TS:   super.greet();
来源：http://fsq.hongshengwenyu.top

Java: super.greet();
来源：http://gid.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bbp.daria6918.cn

Ruby: super
来源：http://mrv.9152youxi.cn

C#:   base.Greet();
来源：http://wpb.tanke756.top

[G08] 静态方法与属性
来源：http://yab.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eht.cucudq.cn

PHP:  public static function f() {}
来源：http://oby.cqqwz.cn

JS:   static f() {}
来源：http://dmi.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://kfs.shzxlz.cn

Java: static void f() {}
来源：http://nnj.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://drk.daxiang520.top

Ruby: def self.f; end
来源：http://qgc.vehdjk.com

C#:   public static void F() {}
来源：http://nik.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://dkh.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://paz.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://eri.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fzl.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://hda.sysykeji.top

Java: interface Shape { double area(); }
来源：http://mfz.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://pus.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vhg.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://muu.hnqzz.top

[G10] 访问控制
来源：http://plz.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://tqi.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://jdl.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://bhq.sweek.top

TS:   public / protected / private
来源：http://wgo.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://drl.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bxr.zdbjq.cn

Ruby: public / protected / private
来源：http://diw.cheryme.top

C#:   public / protected / private / internal
来源：http://nwh.daria6918.cn

[G11] getter / setter
来源：http://zfw.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://bzr.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eso.yvedp.cn

JS:   get name() { return this._name; }
来源：http://gdc.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://arg.hysaishi.cn

Java: public String getName() { return name; }
来源：http://ptj.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jaq.yongpay.top


<!-- 参考信息 -->