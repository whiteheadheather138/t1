代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://neu.zhongyouzk.top

[E11] 反转字符串
来源：http://tuv.hnqzz.top

Py:   s[::-1]
来源：http://zex.daxiang520.top

PHP:  strrev($s);
来源：http://ozz.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://uvb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://igx.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lkh.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eje.tanke756.top

Ruby: s.reverse
来源：http://zeb.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mpq.yueranfly.top

[E12] 统计某字符出现次数
来源：http://wbw.tian-w.cn

Py:   s.count("a")
来源：http://ozb.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://nbc.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://ruk.sysykeji.top

TS:   s.split("a").length - 1
来源：http://bnm.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nlm.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://vqo.daxiang520.top

Ruby: s.count("a")
来源：http://xoz.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://ymd.shzxlz.cn

[E13] 逐字符遍历
来源：http://ewl.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://xul.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pva.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://byh.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qvn.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nfd.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rnz.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nen.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uyz.ivvv.top

[E14] URL 编码与 Base64
来源：http://yqh.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oom.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sgw.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jop.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lzs.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qjd.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ngf.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xyi.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ocp.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://nbz.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yct.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dyl.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sgy.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dnn.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xqz.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dad.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://swo.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://idq.sufxvd.cn

[E16] 数字千分位
来源：http://qgp.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://oou.zhixingplan.top

PHP:  number_format(1234567);
来源：http://pbx.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aet.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yyp.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://emb.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bjn.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ybs.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://xwm.andypj.xyz

[E17] 首字母大写
来源：http://msf.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lpt.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gjz.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://los.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ers.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sxi.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ryn.nanxuanxn.top

Ruby: s.capitalize
来源：http://hqe.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://trf.sweek.top

[E18] 模板占位符替换
来源：http://rwn.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fdx.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wtc.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bnw.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ijn.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mza.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://amx.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fpy.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hqf.ivvv.top

[E19] 多行文本按行拆分
来源：http://gql.cashguo.top

Py:   s.splitlines()
来源：http://lcj.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://elp.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://vso.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://roi.sjlbkw.cn

Java: s.lines().toList()
来源：http://lzf.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://own.sjlbkw.cn

Ruby: s.lines
来源：http://rdd.ydzc1.top

C#:   s.Split('\n')
来源：http://xqt.cashguo.top

[E20] 判断字符串是否为空
来源：http://coi.sysykeji.top

Py:   if not s:
来源：http://egp.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hiy.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bdg.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://eoz.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://bpg.kuanghao11.cn

Go:   if s == "" {}
来源：http://equ.ehwqpu.com

Ruby: if s.empty?
来源：http://dqf.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sml.tanke756.top

[E21] 超长截断加省略号
来源：http://sua.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fzc.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bhu.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqp.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kvc.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mbs.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://lzs.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wvx.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oub.daxiang520.top

[E22] 字节长度与字符长度
来源：http://wvz.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vqi.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rya.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ljb.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqk.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyo.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yes.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://ond.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cpz.ydzc1.top

================================================================================
来源：http://duc.ivvv.top

F. 文件与目录
来源：http://vxy.kuanghao11.cn

================================================================================
来源：http://lqu.gaohongyu789.top

[F01] 读取整个文件
来源：http://lcn.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngy.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://ogp.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exo.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vxj.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://snj.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qzy.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://kwn.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://hvv.hysaishi.cn

[F02] 逐行读取文件
来源：http://vmb.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oyh.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dap.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fti.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxm.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vqn.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sjh.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qsz.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fab.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://qva.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xcz.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://drq.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azu.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrp.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dxb.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mhr.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://uxh.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xok.ivvv.top

[F04] 追加写入文件
来源：http://ghj.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://beu.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qsb.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwv.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gxe.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zha.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sbo.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kue.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qpm.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://vtz.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofv.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://xde.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://ntj.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://qfw.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vcx.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://czt.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://flh.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://iob.vehdjk.com

[F06] 删除文件
来源：http://ebf.vehdjk.com

Py:   os.remove("a.txt")
来源：http://wrm.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://yka.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://awc.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://yio.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gcp.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://ffb.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://lws.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://fha.cheryme.top

[F07] 创建目录（含多级）
来源：http://hwo.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://khw.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sqc.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbs.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhe.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://juy.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://abl.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wop.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mig.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://dbu.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eyu.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://exy.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://nlf.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://uju.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgi.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://quk.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://yor.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://lom.redwolf501.top

[F09] 获取文件大小
来源：http://cvx.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://gyd.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://gra.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://erw.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://gju.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tqm.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tqu.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://quf.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://jfj.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://hms.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gwi.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://puf.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iwl.cucudq.cn

TS:   path.extname("a.txt")
来源：http://zdj.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zup.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rlq.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cfk.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlw.hnqzz.top

[F11] 复制与移动文件
来源：http://nkw.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aqi.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qzh.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egz.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mts.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zwf.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iwq.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfq.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyq.yongpay.top

[F12] CSV 读写
来源：http://qhe.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dyb.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mfm.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://emf.smart0.xyz

TS:   // 同上
来源：http://poe.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fhz.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ldg.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://adw.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xoz.yueranfly.top

================================================================================
来源：http://fzv.guowangkeji.top

G. 面向对象
来源：http://rhk.jiagoushi.top

================================================================================
来源：http://ovj.wangshuangyany.cn

[G01] 定义类
来源：http://axo.yvedp.cn

Py:   class User: pass
来源：http://ukf.pycfn.com

PHP:  class User {}
来源：http://ltz.snrcjt.cn

JS:   class User {}
来源：http://yyd.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://hoz.sweek.top

Java: class User {}
来源：http://jxh.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://pyr.yongpay.top

Ruby: class User; end
来源：http://ifx.c1oappe.top

C#:   class User {}
来源：http://uxc.epnwcf.com

[G02] 构造函数
来源：http://gva.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://eby.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://rer.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://mlc.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://anh.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://sat.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xxh.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://jrq.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://uxr.uphjek.com

[G03] 实例属性
来源：http://ekz.birdmap.top

Py:   self.name = "x"
来源：http://dak.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://sni.pycfn.com

JS:   this.name = "x";
来源：http://vvz.meibo888.top

TS:   name: string = "x";
来源：http://zrp.chenzaomai.com

Java: private String name;
来源：http://uve.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ihj.zhoulong.xyz

Ruby: @name = "x"
来源：http://wjt.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://twr.zhoulong.xyz

[G04] 定义方法
来源：http://crv.ivvv.top

Py:   def greet(self): return self.name
来源：http://zfl.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://omc.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://wjv.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://erd.uphjek.com

Java: String greet() { return name; }
来源：http://gkm.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nrg.epnwcf.com

Ruby: def greet; @name; end
来源：http://pll.andypj.xyz

C#:   public string Greet() => Name;
来源：http://tcv.shuidangran.top

[G05] 继承
来源：http://wwi.yonumen.top

Py:   class Admin(User): pass
来源：http://hnd.yongpay.top

PHP:  class Admin extends User {}
来源：http://nsw.yangfankeji.com

JS:   class Admin extends User {}
来源：http://rde.meibo888.top

TS:   class Admin extends User {}
来源：http://tyo.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://iyt.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nnk.svipenyu.cn

Ruby: class Admin < User; end
来源：http://jeu.gotoacloud.top

C#:   class Admin : User {}
来源：http://bug.gogol.net.cn

[G06] 重写方法
来源：http://zwk.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://mjv.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://ttn.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://fnf.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://mzs.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://sgt.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kyp.yj20258.top

Ruby: def greet; "admin"; end
来源：http://yvh.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://tjf.tarul.cn

[G07] 调用父类方法
来源：http://auw.hammf.cn

Py:   super().greet()
来源：http://and.316326.xyz

PHP:  parent::greet();
来源：http://upv.ydzc1.top

JS:   super.greet();
来源：http://lny.daria6918.cn

TS:   super.greet();
来源：http://wiq.yj202588.top

Java: super.greet();
来源：http://zaj.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mxu.jiagoushi.top

Ruby: super
来源：http://ago.jiagoushi.top

C#:   base.Greet();
来源：http://lsj.jqgfzy.top

[G08] 静态方法与属性
来源：http://wdt.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dch.ybcxt.top

PHP:  public static function f() {}
来源：http://zpk.yj20258.top

JS:   static f() {}
来源：http://irm.zhoulong.xyz

TS:   static f(): void {}
来源：http://lfg.vehdjk.com

Java: static void f() {}
来源：http://jzi.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://htu.shuidangran.top

Ruby: def self.f; end
来源：http://nxo.sjlbkw.cn

C#:   public static void F() {}
来源：http://npp.redwolf501.top

[G09] 接口 / 抽象类
来源：http://uxq.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://iup.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://wtn.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vyp.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://nhf.hywenlv.cn


<!-- 参考信息 -->