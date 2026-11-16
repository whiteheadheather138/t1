代发 wailian999

PHP:  substr_count($s, "a");
来源：http://fwc.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://cqa.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://ikn.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cjv.yongpay.top

Go:   strings.Count(s, "a")
来源：http://pkj.kuanghao11.cn

Ruby: s.count("a")
来源：http://jln.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://hvs.ppjwa.cn

[E13] 逐字符遍历
来源：http://kft.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://nak.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ggt.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://aoz.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vcv.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ldy.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://idv.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ndk.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lek.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://kry.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dra.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://opn.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lok.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tma.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rgj.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hwe.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://may.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dfg.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://zoa.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ryf.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bgy.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxn.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ifq.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kax.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qmi.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eor.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://szu.sufxvd.cn

[E16] 数字千分位
来源：http://jeg.wangdashe.top

Py:   f"{1234567:,}"
来源：http://yrd.jinqigufen.top

PHP:  number_format(1234567);
来源：http://gzb.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://arf.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bgz.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nnp.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kvf.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hlf.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://sum.yonumen.top

[E17] 首字母大写
来源：http://coh.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nfh.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mtb.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ztj.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gfk.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://htk.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://clq.gzhubu.top

Ruby: s.capitalize
来源：http://aqq.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qsv.fzhhl.top

[E18] 模板占位符替换
来源：http://jvx.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qij.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eql.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oag.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sgr.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xhc.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bbz.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rcx.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kcs.iojbl.cn

[E19] 多行文本按行拆分
来源：http://klt.hnxiangtu.top

Py:   s.splitlines()
来源：http://lyq.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gly.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://ohi.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://gko.tian-w.cn

Java: s.lines().toList()
来源：http://ujo.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://ucn.cucudq.cn

Ruby: s.lines
来源：http://fbr.zdqjudy.top

C#:   s.Split('\n')
来源：http://gyn.xuanzx.com

[E20] 判断字符串是否为空
来源：http://tkf.kuanghao11.cn

Py:   if not s:
来源：http://add.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ila.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qyi.zycfv.cn

TS:   if (s === "") {}
来源：http://xze.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://qhm.uphjek.com

Go:   if s == "" {}
来源：http://wen.gzhubu.top

Ruby: if s.empty?
来源：http://sgt.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://glh.cheryme.top

[E21] 超长截断加省略号
来源：http://dgu.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uad.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://etw.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aah.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pom.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ebj.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://ksb.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pyr.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bwp.hcnkem.com

[E22] 字节长度与字符长度
来源：http://flr.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mew.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyg.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vcm.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://djj.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xyc.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pxh.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://lgr.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://njm.pycfn.com

================================================================================
来源：http://dkf.bbcook.cn

F. 文件与目录
来源：http://kdb.chenzaomai.com

================================================================================
来源：http://fbz.chenlongwang.top

[F01] 读取整个文件
来源：http://bdw.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hbu.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://nxf.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vfx.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bzu.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cod.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ijj.xuetiantiany.cn

Ruby: File.read("a.txt")
来源：http://tul.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://saz.yongpay.top

[F02] 逐行读取文件
来源：http://uty.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gio.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://voq.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqj.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibj.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yar.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://awz.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mst.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyd.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://oeh.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vfq.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://osz.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehq.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pax.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qou.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zut.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://jpd.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://arl.aibaodan.cn

[F04] 追加写入文件
来源：http://umf.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fna.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgu.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqt.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucq.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tcg.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oea.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ewm.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xse.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://vwo.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://veu.yj20258.top

PHP:  file_exists("a.txt");
来源：http://blr.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://kfy.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://skb.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://isp.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tih.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://eag.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://zgr.yvedp.cn

[F06] 删除文件
来源：http://vmk.xinyue.icu

Py:   os.remove("a.txt")
来源：http://zvi.yonumen.top

PHP:  unlink("a.txt");
来源：http://nvd.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://egd.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://jvu.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ybj.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://cyr.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://czl.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://zkc.fzhhl.top

[F07] 创建目录（含多级）
来源：http://wfl.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qqr.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xce.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gwd.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jtl.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cez.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cno.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wax.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uqm.iojbl.cn

[F08] 遍历目录
来源：http://idr.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eme.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mof.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://kkf.sweek.top

TS:   fs.readdirSync("dir")
来源：http://que.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lcq.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cjb.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://hsb.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://ufi.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://dhz.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://rgz.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://qyn.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://qwt.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://fpz.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://kdu.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tyt.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://nkx.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://cwy.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://zzm.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nbr.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jtg.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://evb.pycfn.com

TS:   path.extname("a.txt")
来源：http://cgs.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xbi.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oet.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fdn.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://whw.ppjwa.cn

[F11] 复制与移动文件
来源：http://oyd.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lxw.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zre.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pfo.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lgt.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ict.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vkf.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zmo.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gpx.jqgufenzy.top

[F12] CSV 读写
来源：http://ouj.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvf.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tqw.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mrw.9152youxi.cn

TS:   // 同上
来源：http://vwc.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://myn.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gbe.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rfp.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ylf.zhengqikj.top

================================================================================
来源：http://viy.mhx1999.top

G. 面向对象
来源：http://pzg.xuanzx.com

================================================================================
来源：http://tly.hcnkem.com

[G01] 定义类
来源：http://elc.jinqigfzy.top

Py:   class User: pass
来源：http://oxh.hywenlv.cn

PHP:  class User {}
来源：http://gjf.fzhhl.top

JS:   class User {}
来源：http://ibj.hammf.cn

TS:   class User { name: string = ""; }
来源：http://hsu.zycfv.cn

Java: class User {}
来源：http://laa.tanke756.top

Go:   type User struct { Name string }
来源：http://lls.0kj1m.cn

Ruby: class User; end
来源：http://opl.cucudq.cn

C#:   class User {}
来源：http://iup.dashuyun.cn

[G02] 构造函数
来源：http://grm.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://lta.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://gyr.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://wbg.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://clr.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://sqt.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xqs.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://kdw.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://jdi.jinghuilouyu.cn

[G03] 实例属性
来源：http://fxb.jinqigfzy.top

Py:   self.name = "x"
来源：http://dyn.yongpay.top

PHP:  public string $name = "x";
来源：http://ylb.ydjk.org.cn

JS:   this.name = "x";
来源：http://cae.yanxiufei.cn

TS:   name: string = "x";
来源：http://bko.zhixingplan.top

Java: private String name;
来源：http://chh.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ilf.sysykeji.top

Ruby: @name = "x"
来源：http://cwi.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://atr.wangshuangyany.cn

[G04] 定义方法
来源：http://dlr.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://cwm.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aou.guannengcc.top

JS:   greet() { return this.name; }
来源：http://nmr.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://fda.tarul.cn

Java: String greet() { return name; }
来源：http://hua.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ram.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://qgb.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://tto.ydjk.org.cn

[G05] 继承
来源：http://gpb.daxiang520.top

Py:   class Admin(User): pass
来源：http://tuo.sxryk.cn

PHP:  class Admin extends User {}
来源：http://njj.bbcook.cn

JS:   class Admin extends User {}
来源：http://izs.yuxming.cn

TS:   class Admin extends User {}
来源：http://skx.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://xoz.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ysf.jinqigufen.top

Ruby: class Admin < User; end
来源：http://zus.iojbl.cn

C#:   class Admin : User {}
来源：http://zoo.zhengqikj.top

[G06] 重写方法
来源：http://yfy.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://oay.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lew.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://ksh.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://xys.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://xrw.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dmp.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://ldd.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://chb.cdnleiting.top

[G07] 调用父类方法
来源：http://zkh.ydjk.org.cn

Py:   super().greet()
来源：http://pfg.gogol.net.cn

PHP:  parent::greet();
来源：http://aax.yueranfly.top

JS:   super.greet();
来源：http://ppp.kuanghao11.cn

TS:   super.greet();
来源：http://qcf.shuidangran.top

Java: super.greet();
来源：http://khe.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qoh.ydzc1.top

Ruby: super
来源：http://oiv.yangfankeji.com

C#:   base.Greet();
来源：http://ptr.pycfn.com

[G08] 静态方法与属性
来源：http://xjy.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://drp.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://mpn.cqqwz.cn

JS:   static f() {}
来源：http://sag.fzhhl.top

TS:   static f(): void {}
来源：http://hqf.xuanzx.com

Java: static void f() {}
来源：http://flx.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ntd.hnxiangtu.top

Ruby: def self.f; end
来源：http://cdc.meibo888.top

C#:   public static void F() {}
来源：http://ujh.xuanzx.com

[G09] 接口 / 抽象类
来源：http://sgk.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://gux.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://zwz.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://hhe.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://qba.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://lnd.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://qfw.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qbs.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://gek.cheryme.top

[G10] 访问控制
来源：http://nft.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://mfq.vehdjk.com

PHP:  public / protected / private
来源：http://lbn.yfazqb.com

JS:   #private 字段；其余公开
来源：http://vzb.zdbjq.cn

TS:   public / protected / private
来源：http://bbb.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://gtz.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sfx.xylfe.cn

Ruby: public / protected / private
来源：http://zdp.wangshuangyany.cn


<!-- 参考信息 -->