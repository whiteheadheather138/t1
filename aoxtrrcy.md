代发 wailian999

Ruby: s.reverse
来源：http://mmt.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ncd.xinyue.icu

[E12] 统计某字符出现次数
来源：http://ahq.gogol.net.cn

Py:   s.count("a")
来源：http://yth.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://zay.aizwys.cn

JS:   s.split("a").length - 1
来源：http://vtr.shuidangran.top

TS:   s.split("a").length - 1
来源：http://kpf.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aeq.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://yan.xylfe.cn

Ruby: s.count("a")
来源：http://sch.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://mzq.xziqi.cn

[E13] 逐字符遍历
来源：http://soi.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://xqk.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rai.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hku.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fss.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uxl.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://igj.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oim.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jsx.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://gqa.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kpo.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lra.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wir.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://chc.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mhz.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qfp.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dxu.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nwd.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://lin.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ijy.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xoz.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hvv.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zkh.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fcg.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jui.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bgo.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lfc.andypj.xyz

[E16] 数字千分位
来源：http://muf.c1oappe.top

Py:   f"{1234567:,}"
来源：http://hop.mhx1999.top

PHP:  number_format(1234567);
来源：http://rgy.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fts.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wyx.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxk.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uhu.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pgm.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://kbf.jinghuilouyu.cn

[E17] 首字母大写
来源：http://xqj.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mym.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zmt.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zez.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gaz.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ijs.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zhx.pengpengdd.cyou

Ruby: s.capitalize
来源：http://bkm.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zhr.mhx1999.top

[E18] 模板占位符替换
来源：http://vrz.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tit.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bvx.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://onb.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://arh.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rff.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bjg.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ief.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sde.meibo888.top

[E19] 多行文本按行拆分
来源：http://pfl.hcnkem.com

Py:   s.splitlines()
来源：http://aet.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fec.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://llm.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://dul.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://uns.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://npm.fanxiaobao.xyz

Ruby: s.lines
来源：http://caz.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://fyq.hesvh.cn

[E20] 判断字符串是否为空
来源：http://web.zhijiandao.cn

Py:   if not s:
来源：http://byo.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rqn.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iwi.fzhhl.top

TS:   if (s === "") {}
来源：http://met.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://bbf.sxryk.cn

Go:   if s == "" {}
来源：http://xwg.daria6918.cn

Ruby: if s.empty?
来源：http://vou.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cgy.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://bog.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mff.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xuy.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cet.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xak.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rkq.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://lur.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pjg.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oaf.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://uke.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qtt.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ens.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ici.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ykv.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://etc.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oob.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://bic.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qhz.zhoulong.xyz

================================================================================
来源：http://ukq.ivvv.top

F. 文件与目录
来源：http://kkz.zhijiandao.cn

================================================================================
来源：http://brv.zhoulong.xyz

[F01] 读取整个文件
来源：http://djr.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pzd.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://zcq.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gya.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://svz.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jqq.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lmc.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://aao.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://qps.hysaishi.cn

[F02] 逐行读取文件
来源：http://jco.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rul.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://djd.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psk.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wqd.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbm.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://die.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tyt.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fpw.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://kmx.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yas.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vwc.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dlk.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qwk.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dlq.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vwr.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://rmw.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wce.ctjpmb.com

[F04] 追加写入文件
来源：http://juy.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xxp.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lma.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqr.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wui.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nvw.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lzl.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ocv.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vgc.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://bfw.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://loh.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://ppg.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://lor.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://dfi.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lal.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yon.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://dgu.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://evu.xuanzx.com

[F06] 删除文件
来源：http://xlj.pycfn.com

Py:   os.remove("a.txt")
来源：http://njw.bjfxy.top

PHP:  unlink("a.txt");
来源：http://krh.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eqx.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://nbm.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qes.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://hem.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://hbp.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://gzb.yfazqb.com

[F07] 创建目录（含多级）
来源：http://oeu.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cot.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rys.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gns.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xqd.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xiz.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vtf.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://keo.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xru.xylfe.cn

[F08] 遍历目录
来源：http://zst.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tld.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://opu.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://pkp.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://dwm.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ycq.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mqg.wangdashe.top

Ruby: Dir.children("dir")
来源：http://xrh.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://nya.ivvv.top

[F09] 获取文件大小
来源：http://yun.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://dya.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://ejp.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://dcu.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://swm.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ajn.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lbi.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://oez.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://fff.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://nqm.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mla.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mhm.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dfs.yj20258.top

TS:   path.extname("a.txt")
来源：http://zoj.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gwx.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uvs.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nxm.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nwp.jyoumei.cn

[F11] 复制与移动文件
来源：http://iyn.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bjh.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://urr.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdw.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yxn.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qwo.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yad.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vus.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xzb.snrcjt.cn

[F12] CSV 读写
来源：http://mad.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ikw.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nkk.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eho.guowangkeji.top

TS:   // 同上
来源：http://uug.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://twr.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wvt.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pes.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ddn.jiagoushi.top

================================================================================
来源：http://fws.shanyushiyangkeji.top

G. 面向对象
来源：http://tsv.chenzaomai.com

================================================================================
来源：http://pgl.smart0.xyz

[G01] 定义类
来源：http://rmd.yueranfly.top

Py:   class User: pass
来源：http://byu.tian-w.cn

PHP:  class User {}
来源：http://amn.havefunace.top

JS:   class User {}
来源：http://phu.yj202588.top

TS:   class User { name: string = ""; }
来源：http://kba.zdqjudy.top

Java: class User {}
来源：http://mjl.jianghu66.top

Go:   type User struct { Name string }
来源：http://ybi.hnxiangtu.top

Ruby: class User; end
来源：http://wca.ybcxt.top

C#:   class User {}
来源：http://htf.xylfe.cn

[G02] 构造函数
来源：http://vws.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://nhe.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://eub.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://kjb.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://mra.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://hay.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bum.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://amk.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://rlw.dianchejie.cn

[G03] 实例属性
来源：http://pva.iojbl.cn

Py:   self.name = "x"
来源：http://smt.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://clu.316326.xyz

JS:   this.name = "x";
来源：http://jhb.gzhubu.top

TS:   name: string = "x";
来源：http://ssq.ybcxt.top

Java: private String name;
来源：http://rvt.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zjy.hywenlv.cn

Ruby: @name = "x"
来源：http://wnj.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://yss.chenzaomai.com

[G04] 定义方法
来源：http://ami.cheryme.top

Py:   def greet(self): return self.name
来源：http://rjc.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dpk.iojbl.cn

JS:   greet() { return this.name; }
来源：http://xse.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://qxi.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://kfq.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dox.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://yym.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://elx.zycfv.cn

[G05] 继承
来源：http://qoh.hesvh.cn

Py:   class Admin(User): pass
来源：http://ygx.epnwcf.com

PHP:  class Admin extends User {}
来源：http://eix.ybcxt.top

JS:   class Admin extends User {}
来源：http://vna.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://umi.gogol.net.cn

Java: class Admin extends User {}
来源：http://fwv.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ksn.fktsv.cn

Ruby: class Admin < User; end
来源：http://mnx.svipenyu.cn

C#:   class Admin : User {}
来源：http://dhy.nanxuanxn.top

[G06] 重写方法
来源：http://yyf.cashguo.top

Py:   def greet(self): return "admin"
来源：http://dgv.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wyc.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://rns.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://xha.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://lhy.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikx.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://aug.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://nzg.ydjk.org.cn

[G07] 调用父类方法
来源：http://yub.feifeiyinyue.top

Py:   super().greet()
来源：http://rja.hcnkem.com

PHP:  parent::greet();
来源：http://hql.ywan-chungtsiang.top

JS:   super.greet();
来源：http://dnd.ppjwa.cn

TS:   super.greet();
来源：http://eea.svipenyu.cn

Java: super.greet();
来源：http://jcv.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hzm.gzhubu.top

Ruby: super
来源：http://hgq.gzhubu.top

C#:   base.Greet();
来源：http://ncm.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://lly.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bmd.hesvh.cn

PHP:  public static function f() {}
来源：http://nla.jinghuilouyu.cn

JS:   static f() {}
来源：http://bnl.gogol.net.cn

TS:   static f(): void {}
来源：http://lgn.jinqigfzy.top

Java: static void f() {}
来源：http://lfb.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kuv.chenzaomai.com

Ruby: def self.f; end
来源：http://mkm.iojbl.cn

C#:   public static void F() {}
来源：http://bbd.yonumen.top

[G09] 接口 / 抽象类
来源：http://lmz.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://vvd.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://cym.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nao.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://mfw.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://dsk.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://lfy.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zxx.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://ahn.zdbjq.cn

[G10] 访问控制
来源：http://ojo.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://qpw.ydjk.org.cn

PHP:  public / protected / private
来源：http://vxj.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://lxh.cheryme.top


<!-- 参考信息 -->