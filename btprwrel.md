代发 wailian999

PHP:  substr_count($s, "a");
来源：http://dkb.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://bmp.yuxming.cn

TS:   s.split("a").length - 1
来源：http://ugu.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ned.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://nqc.vehdjk.com

Ruby: s.count("a")
来源：http://fqr.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://odh.jyoumei.cn

[E13] 逐字符遍历
来源：http://cfs.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://ncy.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eaj.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jcu.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://prh.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pmx.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yrw.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://dya.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sal.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://asg.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hyo.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wds.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jtv.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pmz.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ehz.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fdf.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pbt.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lkb.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://oqk.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bvg.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ixc.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tby.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gzk.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tyg.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://chg.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dgd.jiagoushi.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ebl.52xcode.cn

[E16] 数字千分位
来源：http://tfi.tarul.cn

Py:   f"{1234567:,}"
来源：http://khc.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://iay.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://swh.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xvi.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqi.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bpz.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hqy.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://avr.fktsv.cn

[E17] 首字母大写
来源：http://nqw.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uia.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://evu.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://shd.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://exj.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oxl.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yvd.zhongyouzk.top

Ruby: s.capitalize
来源：http://mda.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bsw.nanxinkj.top

[E18] 模板占位符替换
来源：http://nvw.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xme.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wen.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dtl.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oii.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bth.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxe.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://orj.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ant.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://jpw.gogol.net.cn

Py:   s.splitlines()
来源：http://ggp.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zlb.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://frb.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://ogl.shangyingyoupin.top

Java: s.lines().toList()
来源：http://qni.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://ktn.epnwcf.com

Ruby: s.lines
来源：http://quw.nanxuanxn.top

C#:   s.Split('\n')
来源：http://cpt.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://thb.yongpay.top

Py:   if not s:
来源：http://xjx.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nmp.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://huh.yvedp.cn

TS:   if (s === "") {}
来源：http://bhx.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://ppv.jianghu66.top

Go:   if s == "" {}
来源：http://cjp.sxryk.cn

Ruby: if s.empty?
来源：http://uhv.tian-w.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jzz.yvedp.cn

[E21] 超长截断加省略号
来源：http://fpl.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nkg.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpj.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmj.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://znl.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gqr.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://sux.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dmq.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lbt.smart0.xyz

[E22] 字节长度与字符长度
来源：http://zjx.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://owa.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uym.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vka.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fgi.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://koo.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://khr.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://otz.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hdb.zdqjudy.top

================================================================================
来源：http://xki.fanxiaobao.xyz

F. 文件与目录
来源：http://aqh.xuetiantiany.cn

================================================================================
来源：http://ejx.chenzaomai.com

[F01] 读取整个文件
来源：http://yjp.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nbx.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://oos.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oqu.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clc.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bdz.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bpp.hesvh.cn

Ruby: File.read("a.txt")
来源：http://kxq.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://mmc.daxiang520.top

[F02] 逐行读取文件
来源：http://mwf.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wgt.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mux.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opq.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ozj.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ymc.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tml.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oke.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tcc.ivvv.top

[F03] 写入文件（覆盖）
来源：http://opx.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lrx.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lhg.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnd.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gxg.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jrv.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fov.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://jys.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qtm.zycfv.cn

[F04] 追加写入文件
来源：http://ngy.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ooc.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vla.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avx.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lcn.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ftp.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hja.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://irw.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ffa.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://guw.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bdg.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://vfg.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://iuj.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://wfu.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gkl.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lpy.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://cby.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://ikv.snrcjt.cn

[F06] 删除文件
来源：http://puw.hcnkem.com

Py:   os.remove("a.txt")
来源：http://wro.shuidangran.top

PHP:  unlink("a.txt");
来源：http://fww.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gnb.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vfg.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xop.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://kaz.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://erp.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://ave.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://djd.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fam.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nmp.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sef.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qed.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yfp.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdd.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://epg.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ocd.uphjek.com

[F08] 遍历目录
来源：http://tla.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xyl.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mga.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://swl.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://uqy.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nbj.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rsr.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://nie.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://zij.c1oappe.top

[F09] 获取文件大小
来源：http://lcw.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://rzk.iojbl.cn

PHP:  filesize("a.txt");
来源：http://gfx.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://rgr.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://erv.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://vwd.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jdx.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://sqm.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://aee.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://neh.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uky.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oki.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rsb.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://zuk.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tym.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mle.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dug.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wuw.fehbvm.com

[F11] 复制与移动文件
来源：http://kkz.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hxw.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://edm.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwl.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdo.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kaf.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhw.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqd.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mrj.sysykeji.top

[F12] CSV 读写
来源：http://fus.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mgk.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tel.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zij.jqgufenzy.top

TS:   // 同上
来源：http://lkw.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nte.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hhp.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dcu.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fiq.snrcjt.cn

================================================================================
来源：http://trh.birdmap.top

G. 面向对象
来源：http://ged.yanxiufei.cn

================================================================================
来源：http://qmj.fengsongda.top

[G01] 定义类
来源：http://oxy.vqdsnc.cn

Py:   class User: pass
来源：http://dyy.gotoacloud.top

PHP:  class User {}
来源：http://ukz.cucudq.cn

JS:   class User {}
来源：http://qwe.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://iav.zhaomingkeji.xyz

Java: class User {}
来源：http://dxb.ctjpmb.com

Go:   type User struct { Name string }
来源：http://jyp.sjlbkw.cn

Ruby: class User; end
来源：http://tkp.sxryk.cn

C#:   class User {}
来源：http://rnf.zhijiandao.cn

[G02] 构造函数
来源：http://slh.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://czi.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xdb.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://ibf.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://vcm.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://mfo.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uxl.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://pyz.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://cpw.ctjpmb.com

[G03] 实例属性
来源：http://dfl.vqdsnc.cn

Py:   self.name = "x"
来源：http://bpf.epnwcf.com

PHP:  public string $name = "x";
来源：http://tgt.daria6918.cn

JS:   this.name = "x";
来源：http://jbg.jqgfzy.top

TS:   name: string = "x";
来源：http://tzv.ydzc1.top

Java: private String name;
来源：http://fgj.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qnb.aibaodan.cn

Ruby: @name = "x"
来源：http://ruw.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://cpa.xylfe.cn

[G04] 定义方法
来源：http://dlv.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://mes.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kev.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://mwo.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://qif.zhengqikj.top

Java: String greet() { return name; }
来源：http://mzz.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbd.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://sqh.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://pjp.xingfuxueyuan.xyz

[G05] 继承
来源：http://hcd.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://hpm.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://hsy.sysykeji.top

JS:   class Admin extends User {}
来源：http://wkd.ybcxt.top

TS:   class Admin extends User {}
来源：http://qdo.jqgfzy.top

Java: class Admin extends User {}
来源：http://nvv.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://itp.hnqzz.top

Ruby: class Admin < User; end
来源：http://uea.sxryk.cn

C#:   class Admin : User {}
来源：http://ium.bbcook.cn

[G06] 重写方法
来源：http://gkb.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://xfe.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://upi.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://mhw.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://eha.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://mzi.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rcf.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://cjg.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://jea.andypj.xyz

[G07] 调用父类方法
来源：http://rvr.yongpay.top

Py:   super().greet()
来源：http://med.yongpay.top

PHP:  parent::greet();
来源：http://acx.jinqigufen.top

JS:   super.greet();
来源：http://gsu.tian-w.cn

TS:   super.greet();
来源：http://mbu.yvedp.cn

Java: super.greet();
来源：http://poo.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zaj.hfpthk.cn

Ruby: super
来源：http://yje.redwolf501.top

C#:   base.Greet();
来源：http://atl.zhongyouzk.top

[G08] 静态方法与属性
来源：http://fad.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ejk.cashguo.top

PHP:  public static function f() {}
来源：http://pga.fehbvm.com

JS:   static f() {}
来源：http://eqd.aibaodan.cn

TS:   static f(): void {}
来源：http://sfq.yueranfly.top

Java: static void f() {}
来源：http://xyt.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ppz.zdqjudy.top

Ruby: def self.f; end
来源：http://gxi.aibaodan.cn

C#:   public static void F() {}
来源：http://saz.shuidangran.top

[G09] 接口 / 抽象类
来源：http://xvw.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://ako.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://zzq.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://wux.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://rwp.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://jev.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://gis.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dlg.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://bnz.pengpengdd.cyou

[G10] 访问控制
来源：http://kvn.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://mwh.zhoulong.xyz

PHP:  public / protected / private
来源：http://rej.yfazqb.com

JS:   #private 字段；其余公开
来源：http://rty.chenjidiqi.icu

TS:   public / protected / private
来源：http://hbg.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://ctx.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qww.yanxiufei.cn

Ruby: public / protected / private
来源：http://qef.hammf.cn


<!-- 参考信息 -->