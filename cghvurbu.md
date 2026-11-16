代发 wailian999

JS:   [...s].reverse().join("")
来源：http://agb.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://ifb.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sme.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ibe.zhijiandao.cn

Ruby: s.reverse
来源：http://lyc.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://awv.yongpay.top

[E12] 统计某字符出现次数
来源：http://zvd.c1oappe.top

Py:   s.count("a")
来源：http://nvb.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://tib.tian-w.cn

JS:   s.split("a").length - 1
来源：http://zho.guannengcc.top

TS:   s.split("a").length - 1
来源：http://iup.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gos.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://fsq.tanke756.top

Ruby: s.count("a")
来源：http://bpd.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://rlt.yvedp.cn

[E13] 逐字符遍历
来源：http://wye.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://kvw.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://war.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://skf.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dcf.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lfe.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mqo.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://cjn.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ssf.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://got.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://atp.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ddn.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zfz.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxs.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uhk.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lly.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ged.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nzb.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://emn.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zem.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jcj.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nzp.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://nij.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hwp.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qll.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ltr.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kqy.xinyue.icu

[E16] 数字千分位
来源：http://ont.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://rur.hesvh.cn

PHP:  number_format(1234567);
来源：http://mjd.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hkw.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://mmg.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gap.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qia.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ahm.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://eac.mhx1999.top

[E17] 首字母大写
来源：http://wld.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ael.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://myj.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lgz.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ink.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gfp.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bqv.shuidangran.top

Ruby: s.capitalize
来源：http://xxy.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ffn.havefunace.top

[E18] 模板占位符替换
来源：http://ayw.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://arn.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vce.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uyh.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://phm.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wpj.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxx.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hun.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nda.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://dpl.yanxiufei.cn

Py:   s.splitlines()
来源：http://wex.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nlc.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://koo.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://qlo.cucudq.cn

Java: s.lines().toList()
来源：http://rwe.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://lxi.aizwys.cn

Ruby: s.lines
来源：http://yru.uphjek.com

C#:   s.Split('\n')
来源：http://gei.wangdashe.top

[E20] 判断字符串是否为空
来源：http://qtc.yangfankeji.com

Py:   if not s:
来源：http://kla.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://onk.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oqp.yongpay.top

TS:   if (s === "") {}
来源：http://iao.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://okw.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://gfk.nanxuanxn.top

Ruby: if s.empty?
来源：http://gio.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tdt.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://ayo.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nxd.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lnl.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwp.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cfm.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zvt.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://yih.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pwi.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zqg.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://zhi.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eeo.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kkw.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtd.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rlq.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://asb.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uto.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://pgw.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sti.zhixingplan.top

================================================================================
来源：http://msl.fanxiaobao.xyz

F. 文件与目录
来源：http://fqt.svipenyu.cn

================================================================================
来源：http://edz.jqgfzy.top

[F01] 读取整个文件
来源：http://jii.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bby.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://hur.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsx.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oez.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gso.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hgr.daria6918.cn

Ruby: File.read("a.txt")
来源：http://uvf.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://hyq.fzhhl.top

[F02] 逐行读取文件
来源：http://xmc.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zma.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dbt.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ydx.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fup.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ndy.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xoo.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xmc.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vct.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://tja.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ksj.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ihi.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifr.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihb.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://stv.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://okf.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://akl.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bae.jianghu66.top

[F04] 追加写入文件
来源：http://jyg.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qdy.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ajj.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fgc.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cqf.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://udo.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jez.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pty.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dhp.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://mfo.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fzl.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://xoi.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://mjn.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://pyf.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vaq.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pqz.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://poc.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://esk.ctjpmb.com

[F06] 删除文件
来源：http://mei.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://udg.c1oappe.top

PHP:  unlink("a.txt");
来源：http://ojn.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tri.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://yrl.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pwo.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://ubz.tarul.cn

Ruby: File.delete("a.txt")
来源：http://jad.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://zup.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://ymf.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pau.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ksm.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sqf.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxb.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rih.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aws.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xyg.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bff.shangyingyoupin.top

[F08] 遍历目录
来源：http://hdh.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xoi.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mji.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://fdl.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://mzw.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lan.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://oiu.sweek.top

Ruby: Dir.children("dir")
来源：http://fek.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://cvo.ctjpmb.com

[F09] 获取文件大小
来源：http://djt.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://lzj.tarul.cn

PHP:  filesize("a.txt");
来源：http://wpx.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://ffj.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://rwf.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://tfv.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ffy.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://stw.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://zxv.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://hnd.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gfo.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zug.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ffd.yj20258888.top

TS:   path.extname("a.txt")
来源：http://crt.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxe.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://igy.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dem.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fon.aizwys.cn

[F11] 复制与移动文件
来源：http://iiu.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gxd.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vym.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uyk.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vfc.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qro.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jca.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zti.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dir.yangfankeji.com

[F12] CSV 读写
来源：http://zdc.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vvk.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xak.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wcp.xuetiantiany.cn

TS:   // 同上
来源：http://sqf.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ama.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfq.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wvv.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://nep.sysykeji.top

================================================================================
来源：http://eyg.feifeiyinyue.top

G. 面向对象
来源：http://yab.guannengcc.top

================================================================================
来源：http://nta.zhiwuduotai.top

[G01] 定义类
来源：http://sqa.zdqjudy.top

Py:   class User: pass
来源：http://pbw.tianlin.xyz

PHP:  class User {}
来源：http://aoa.haohaochexian.top

JS:   class User {}
来源：http://qxg.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://hav.sysykeji.top

Java: class User {}
来源：http://dwe.sxryk.cn

Go:   type User struct { Name string }
来源：http://fyz.quarkkingdee.top

Ruby: class User; end
来源：http://pxe.ydzc1.top

C#:   class User {}
来源：http://ffr.cdnleiting.top

[G02] 构造函数
来源：http://slg.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://hxz.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://bpt.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://fum.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://uhq.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://egb.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sbs.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://hom.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://ozo.cqqwz.cn

[G03] 实例属性
来源：http://viz.uphjek.com

Py:   self.name = "x"
来源：http://lxs.yj20258.top

PHP:  public string $name = "x";
来源：http://zvt.zhoulong.xyz

JS:   this.name = "x";
来源：http://pcq.xylfe.cn

TS:   name: string = "x";
来源：http://iwi.hysaishi.cn

Java: private String name;
来源：http://gji.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dua.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://prj.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://fev.nanxinkj.top

[G04] 定义方法
来源：http://fam.yonumen.top

Py:   def greet(self): return self.name
来源：http://ivx.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pca.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://umf.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://zaw.aibaodan.cn

Java: String greet() { return name; }
来源：http://jju.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qlg.yuanzhike.top

Ruby: def greet; @name; end
来源：http://pmw.hcnkem.com

C#:   public string Greet() => Name;
来源：http://nvz.bjfxy.top

[G05] 继承
来源：http://vgg.wangdashe.top

Py:   class Admin(User): pass
来源：http://huw.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://seb.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://kdt.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://iwt.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://vhp.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gas.yueranfly.top

Ruby: class Admin < User; end
来源：http://itr.sufxvd.cn

C#:   class Admin : User {}
来源：http://dav.yuxming.cn

[G06] 重写方法
来源：http://oir.ivvv.top

Py:   def greet(self): return "admin"
来源：http://bmo.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://keo.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://ofl.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://blf.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://fbb.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qdo.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://unt.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://qjr.pengpengdd.cyou

[G07] 调用父类方法
来源：http://mbq.fengsongda.top

Py:   super().greet()
来源：http://ynx.nanxinkj.top

PHP:  parent::greet();
来源：http://ubi.shanyushiyangkeji.top

JS:   super.greet();
来源：http://sea.jqgufenzy.top

TS:   super.greet();
来源：http://rnq.cheryme.top

Java: super.greet();
来源：http://qvr.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wym.ydzc1.top

Ruby: super
来源：http://dkz.tanke756.top

C#:   base.Greet();
来源：http://med.snrcjt.cn

[G08] 静态方法与属性
来源：http://suo.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iqn.yonumen.top

PHP:  public static function f() {}
来源：http://oso.guowangkeji.top

JS:   static f() {}
来源：http://emz.feifeiyinyue.top

TS:   static f(): void {}
来源：http://dqq.xinyue.icu

Java: static void f() {}
来源：http://iok.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ncz.iojbl.cn

Ruby: def self.f; end
来源：http://orn.chenjidiqi.icu

C#:   public static void F() {}
来源：http://vgm.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://yva.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://tkd.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sni.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wkn.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://tra.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://hkt.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://upc.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qmo.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://vmv.wangdashe.top


<!-- 参考信息 -->