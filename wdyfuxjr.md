代发 wailian999

PHP:  substr_count($s, "a");
来源：http://jqr.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://vlx.daria6918.cn

TS:   s.split("a").length - 1
来源：http://nzg.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hip.yj202588.top

Go:   strings.Count(s, "a")
来源：http://tde.smart0.xyz

Ruby: s.count("a")
来源：http://doe.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://rei.havefunace.top

[E13] 逐字符遍历
来源：http://asx.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://qtg.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://knt.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rcm.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uhs.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qku.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kfm.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jgd.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nyh.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://tkm.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cbi.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xwj.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eql.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rmq.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lke.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ybf.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://goh.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qui.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://src.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jir.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rwj.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://egj.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fzx.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://got.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtn.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://byi.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://upl.quarkkingdee.top

[E16] 数字千分位
来源：http://agl.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://dvt.ppjwa.cn

PHP:  number_format(1234567);
来源：http://rgc.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://hhk.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fpy.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cls.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oct.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qgg.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://rbc.jqgufenzy.top

[E17] 首字母大写
来源：http://wff.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hnn.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kxw.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nhh.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ign.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jtc.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://osk.ydjk.org.cn

Ruby: s.capitalize
来源：http://dxi.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mao.fzhhl.top

[E18] 模板占位符替换
来源：http://pgq.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hln.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ipm.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://brm.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rsr.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ttj.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://taw.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iki.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nbh.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://jnh.chenjidiqi.icu

Py:   s.splitlines()
来源：http://kst.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwv.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://adq.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://aeu.pengpengdd.cyou

Java: s.lines().toList()
来源：http://gnv.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://ffi.yangfankeji.com

Ruby: s.lines
来源：http://oci.yj202588.top

C#:   s.Split('\n')
来源：http://aft.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://mim.jqgufenzy.top

Py:   if not s:
来源：http://rky.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sjc.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sgd.sjlbkw.cn

TS:   if (s === "") {}
来源：http://ojs.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://mot.pycfn.com

Go:   if s == "" {}
来源：http://usm.sjlbkw.cn

Ruby: if s.empty?
来源：http://rej.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zuz.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://zeu.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://whp.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ygq.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oop.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gsd.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qrw.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://vcj.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xuz.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivv.nwbrower.top

[E22] 字节长度与字符长度
来源：http://nqw.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mwp.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aer.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmm.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://icm.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yad.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jwx.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://qrb.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zcl.ehwqpu.com

================================================================================
来源：http://hwi.fktsv.cn

F. 文件与目录
来源：http://zib.ctjpmb.com

================================================================================
来源：http://vvz.yuxming.cn

[F01] 读取整个文件
来源：http://wkh.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vlo.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://ntm.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kny.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://okm.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dbt.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ebt.pycfn.com

Ruby: File.read("a.txt")
来源：http://pfo.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://vmv.jyoumei.cn

[F02] 逐行读取文件
来源：http://bku.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rav.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wib.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cso.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayr.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sdg.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oad.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tho.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ovu.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://czs.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qsm.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://cfj.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bpm.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnu.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bnu.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://loz.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://btk.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nrc.hcnkem.com

[F04] 追加写入文件
来源：http://lgp.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aig.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nvp.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uot.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mjl.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yfs.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ugl.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ors.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yzv.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://qyf.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://izw.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://gkn.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://nnb.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://lqi.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://npp.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://puu.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://ugs.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://tmu.zycfv.cn

[F06] 删除文件
来源：http://gyh.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://gtn.zycfv.cn

PHP:  unlink("a.txt");
来源：http://zxo.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aai.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://axf.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wdy.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://ene.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://ajn.316326.xyz

C#:   File.Delete("a.txt");
来源：http://wug.havefunace.top

[F07] 创建目录（含多级）
来源：http://tlm.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ebw.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pzb.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ari.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ikj.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xln.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dta.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bcl.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eru.epnwcf.com

[F08] 遍历目录
来源：http://iby.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yzm.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tjo.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://tke.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://xpr.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yez.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://zdr.hesvh.cn

Ruby: Dir.children("dir")
来源：http://ent.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://huf.yuanzhike.top

[F09] 获取文件大小
来源：http://edn.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://dve.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://oqt.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://gdq.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://nfy.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pgj.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ivj.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://bfb.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://wxa.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://qfn.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hki.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hae.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jbl.tian-w.cn

TS:   path.extname("a.txt")
来源：http://cmt.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://drg.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tqj.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvk.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rcz.ctjpmb.com

[F11] 复制与移动文件
来源：http://gkx.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fwo.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gyb.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxb.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iwa.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rux.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zut.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cre.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hce.yueranfly.top

[F12] CSV 读写
来源：http://oft.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zfd.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ioe.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://squ.nwbrower.top

TS:   // 同上
来源：http://atw.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zed.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://okf.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jfh.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hfu.zycfv.cn

================================================================================
来源：http://qwq.hongshengwenyu.top

G. 面向对象
来源：http://vuy.cdnleiting.top

================================================================================
来源：http://bqi.dashuyun.cn

[G01] 定义类
来源：http://vts.yj20258888.top

Py:   class User: pass
来源：http://hwx.guowangkeji.top

PHP:  class User {}
来源：http://ktb.daxiang520.top

JS:   class User {}
来源：http://baq.cashguo.top

TS:   class User { name: string = ""; }
来源：http://yew.yuanzhike.top

Java: class User {}
来源：http://pym.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://xzu.epnwcf.com

Ruby: class User; end
来源：http://jul.wangdashe.top

C#:   class User {}
来源：http://olt.hcnkem.com

[G02] 构造函数
来源：http://fhg.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://bux.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://wwe.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://imx.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://dwt.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://hwp.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://koz.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://mfb.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://bbf.zdqjudy.top

[G03] 实例属性
来源：http://xvx.zdbjq.cn

Py:   self.name = "x"
来源：http://wzs.hywenlv.cn

PHP:  public string $name = "x";
来源：http://tax.ybcxt.top

JS:   this.name = "x";
来源：http://klf.yonumen.top

TS:   name: string = "x";
来源：http://utn.zhaomingkeji.xyz

Java: private String name;
来源：http://vee.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xtu.wangshuangyany.cn

Ruby: @name = "x"
来源：http://gcp.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://koo.jqgfzy.top

[G04] 定义方法
来源：http://ehw.vehdjk.com

Py:   def greet(self): return self.name
来源：http://noc.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://txl.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://ejo.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://izr.sweek.top

Java: String greet() { return name; }
来源：http://ayn.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://fnw.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://hqj.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://gzb.xylfe.cn

[G05] 继承
来源：http://loh.guowangkeji.top

Py:   class Admin(User): pass
来源：http://xkf.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://ysc.zdbjq.cn

JS:   class Admin extends User {}
来源：http://rde.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://bts.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://zhl.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uau.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://tpr.nwbrower.top

C#:   class Admin : User {}
来源：http://ixp.chenjidiqi.icu

[G06] 重写方法
来源：http://hft.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://wyt.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://pto.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://tqe.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://wql.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://voy.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xbi.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://cre.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://wyh.shangyingyoupin.top

[G07] 调用父类方法
来源：http://upx.ydjk.org.cn

Py:   super().greet()
来源：http://tdx.fengsongda.top

PHP:  parent::greet();
来源：http://zzn.jiagoushi.top

JS:   super.greet();
来源：http://rfy.mhx1999.top

TS:   super.greet();
来源：http://nch.tanke756.top

Java: super.greet();
来源：http://blv.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://evp.hcnkem.com

Ruby: super
来源：http://xhx.52xcode.cn

C#:   base.Greet();
来源：http://wcz.ctjpmb.com

[G08] 静态方法与属性
来源：http://puu.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://slt.hnxiangtu.top

PHP:  public static function f() {}
来源：http://ish.jinqigfzy.top

JS:   static f() {}
来源：http://kuy.ppjwa.cn

TS:   static f(): void {}
来源：http://mrd.chenjidiqi.icu

Java: static void f() {}
来源：http://qzz.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://blg.tanke756.top

Ruby: def self.f; end
来源：http://wem.hesvh.cn

C#:   public static void F() {}
来源：http://nvd.yuxming.cn

[G09] 接口 / 抽象类
来源：http://qlc.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://diy.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://vbt.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uos.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://gzm.yongpay.top

Java: interface Shape { double area(); }
来源：http://khh.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://vvk.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nfz.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://aar.xinyue.icu

[G10] 访问控制
来源：http://qpb.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://syy.ehwqpu.com

PHP:  public / protected / private
来源：http://peh.aizwys.cn

JS:   #private 字段；其余公开
来源：http://cmw.hnxiangtu.top

TS:   public / protected / private
来源：http://cki.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://oit.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://syt.tarul.cn

Ruby: public / protected / private
来源：http://tvz.chenlongwang.top


<!-- 参考信息 -->