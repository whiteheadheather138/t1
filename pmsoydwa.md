代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xkx.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ivb.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tpn.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tqw.meibo888.top

[E14] URL 编码与 Base64
来源：http://tiv.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://etn.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://utw.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnr.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ird.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://usm.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lds.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yoe.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xlx.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://hjo.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://slo.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://icz.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vex.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qzz.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://khx.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kdy.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fzm.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eae.zhixingplan.top

[E16] 数字千分位
来源：http://wqz.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://jzo.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://mts.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nhv.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fns.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xwq.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kir.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xyd.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://tuh.hammf.cn

[E17] 首字母大写
来源：http://kef.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ixa.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hja.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcq.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vlm.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ont.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eic.ydzc1.top

Ruby: s.capitalize
来源：http://qra.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://erb.jinqigfzy.top

[E18] 模板占位符替换
来源：http://yem.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wwv.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://reh.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jpv.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rml.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://njf.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bgr.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gky.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ren.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://fav.chenlongwang.top

Py:   s.splitlines()
来源：http://vma.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bdh.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://kxy.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://ndj.hammf.cn

Java: s.lines().toList()
来源：http://rin.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://wgh.nanxinkj.top

Ruby: s.lines
来源：http://pdp.sysykeji.top

C#:   s.Split('\n')
来源：http://arp.sxryk.cn

[E20] 判断字符串是否为空
来源：http://gmq.ydzc1.top

Py:   if not s:
来源：http://wti.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jnq.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gma.yuanzhike.top

TS:   if (s === "") {}
来源：http://eon.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://hfr.ydzc1.top

Go:   if s == "" {}
来源：http://uad.zdqjudy.top

Ruby: if s.empty?
来源：http://vov.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mvf.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://tck.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ywe.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://duo.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zvc.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yuv.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pqy.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://fcn.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zdu.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qfq.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://aah.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://srt.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aek.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqk.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aqr.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lmo.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pzi.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://dza.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lnk.bjfxy.top

================================================================================
来源：http://bxa.yj20258888.top

F. 文件与目录
来源：http://jru.nwbrower.top

================================================================================
来源：http://nxm.ybcxt.top

[F01] 读取整个文件
来源：http://vfg.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dsy.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://jli.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dua.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wku.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nkq.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://plh.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://uok.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://qyy.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://qmh.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vum.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://afs.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ket.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tny.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpq.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xtx.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ooo.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lil.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://gzu.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nnv.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zef.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yib.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nkb.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://osx.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://izn.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://jvj.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bmk.quarkkingdee.top

[F04] 追加写入文件
来源：http://bqn.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hel.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://naa.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://arc.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hef.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qkj.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://acz.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kkc.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wtr.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://zek.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ego.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://jqf.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://qsf.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://gjn.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xem.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rhy.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://bln.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://xub.c1oappe.top

[F06] 删除文件
来源：http://jbq.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://xpr.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://rnz.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://flk.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://dxi.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jtk.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://fgv.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://iky.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://zyq.redwolf501.top

[F07] 创建目录（含多级）
来源：http://diy.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nhn.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xsb.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://llv.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bys.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zvl.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ail.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bbx.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rua.aizwys.cn

[F08] 遍历目录
来源：http://dnm.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rgm.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qlp.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://xjq.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://ipw.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xpm.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xtf.tarul.cn

Ruby: Dir.children("dir")
来源：http://xyg.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://qcz.uphjek.com

[F09] 获取文件大小
来源：http://rjj.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://gfo.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://bgd.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://gjc.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://xwf.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://zfq.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rke.yj202588.top

Ruby: File.size("a.txt")
来源：http://oez.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://nyx.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://sil.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tpf.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gpm.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sme.hnqzz.top

TS:   path.extname("a.txt")
来源：http://gyv.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pqc.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzq.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://njd.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://paq.jinqigfzy.top

[F11] 复制与移动文件
来源：http://ipb.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rgg.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ikx.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oei.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://stx.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yvc.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jhm.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gvk.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xvs.dashuyun.cn

[F12] CSV 读写
来源：http://kqb.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qmz.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vrk.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://txu.fzhhl.top

TS:   // 同上
来源：http://shy.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eov.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oak.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cbo.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bdv.chenzaomai.com

================================================================================
来源：http://xlj.chenzaomai.com

G. 面向对象
来源：http://lpo.sysykeji.top

================================================================================
来源：http://rlm.yuanzhike.top

[G01] 定义类
来源：http://rbd.yfazqb.com

Py:   class User: pass
来源：http://ibs.guowangkeji.top

PHP:  class User {}
来源：http://vdg.yongpay.top

JS:   class User {}
来源：http://ovs.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://rqd.hysaishi.cn

Java: class User {}
来源：http://brs.zdqjudy.top

Go:   type User struct { Name string }
来源：http://wiv.ydzc1.top

Ruby: class User; end
来源：http://deh.pengpengdd.cyou

C#:   class User {}
来源：http://crm.zhengqikj.top

[G02] 构造函数
来源：http://nbd.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://tku.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://fhh.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://vxp.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://vtc.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://cdt.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cob.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://pth.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://fnt.quarkkingdee.top

[G03] 实例属性
来源：http://mty.chenlongwang.top

Py:   self.name = "x"
来源：http://ybd.ydzc1.top

PHP:  public string $name = "x";
来源：http://hmh.jiagoushi.top

JS:   this.name = "x";
来源：http://cjr.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://ygj.yj20258.top

Java: private String name;
来源：http://sco.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vqe.tianlin.xyz

Ruby: @name = "x"
来源：http://fvv.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://qkq.0kj1m.cn

[G04] 定义方法
来源：http://ttq.gzhubu.top

Py:   def greet(self): return self.name
来源：http://sjs.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ghk.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://qie.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://rsd.yongpay.top

Java: String greet() { return name; }
来源：http://bpj.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rxo.birdmap.top

Ruby: def greet; @name; end
来源：http://thg.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://jxs.daxiang520.top

[G05] 继承
来源：http://uhn.jinqigufen.top

Py:   class Admin(User): pass
来源：http://jrr.pycfn.com

PHP:  class Admin extends User {}
来源：http://fyp.zhengqikj.top

JS:   class Admin extends User {}
来源：http://oay.cqqwz.cn

TS:   class Admin extends User {}
来源：http://vcr.hnqzz.top

Java: class Admin extends User {}
来源：http://jpw.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ghv.aizwys.cn

Ruby: class Admin < User; end
来源：http://chd.jqgufenzy.top

C#:   class Admin : User {}
来源：http://xsk.tian-w.cn

[G06] 重写方法
来源：http://lds.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://xfg.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jxj.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://rts.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://wof.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://iwc.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rtx.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://enw.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://yoa.zhongyouzk.top

[G07] 调用父类方法
来源：http://inn.nanxuanxn.top

Py:   super().greet()
来源：http://rhb.nanxinkj.top

PHP:  parent::greet();
来源：http://ppb.0kj1m.cn

JS:   super.greet();
来源：http://xxw.zhixingplan.top

TS:   super.greet();
来源：http://qhy.hfpthk.cn

Java: super.greet();
来源：http://bjh.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jpr.fktsv.cn

Ruby: super
来源：http://yai.bjfxy.top

C#:   base.Greet();
来源：http://raa.wangdashe.top

[G08] 静态方法与属性
来源：http://mwo.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qep.yueranfly.top

PHP:  public static function f() {}
来源：http://zyz.cucudq.cn

JS:   static f() {}
来源：http://xby.jqgfzy.top

TS:   static f(): void {}
来源：http://atl.redwolf501.top

Java: static void f() {}
来源：http://qae.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://atq.ydjk.org.cn

Ruby: def self.f; end
来源：http://aka.xziqi.cn

C#:   public static void F() {}
来源：http://qip.tarul.cn

[G09] 接口 / 抽象类
来源：http://omm.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://dit.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://geu.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ope.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://rnf.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://akj.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://cqg.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://csd.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://dmf.hywenlv.cn

[G10] 访问控制
来源：http://syn.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://cdi.mhx1999.top

PHP:  public / protected / private
来源：http://svb.uphjek.com

JS:   #private 字段；其余公开
来源：http://btf.52xcode.cn

TS:   public / protected / private
来源：http://wcu.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://txr.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxn.cashguo.top

Ruby: public / protected / private
来源：http://dtn.zhengqikj.top

C#:   public / protected / private / internal
来源：http://kfy.gogol.net.cn

[G11] getter / setter
来源：http://dtv.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://rcf.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eew.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://aom.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://szz.c1oappe.top

Java: public String getName() { return name; }
来源：http://ntt.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pur.xylfe.cn

Ruby: attr_accessor :name
来源：http://xzb.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://oie.zhixingplan.top

[G12] 对象转字符串
来源：http://bnr.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://xui.iojbl.cn


<!-- 参考信息 -->