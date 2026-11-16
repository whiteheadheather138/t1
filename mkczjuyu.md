代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://spl.zycfv.cn

Java: String.format("%03d", 7)
来源：http://ran.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xop.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wjf.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ati.hfpthk.cn

[E11] 反转字符串
来源：http://elk.ctjpmb.com

Py:   s[::-1]
来源：http://fii.ctjpmb.com

PHP:  strrev($s);
来源：http://gpa.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://ifv.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://wfw.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://efl.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qtx.hnqzz.top

Ruby: s.reverse
来源：http://hxg.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qnc.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://nhv.birdmap.top

Py:   s.count("a")
来源：http://ybe.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://iap.wangdashe.top

JS:   s.split("a").length - 1
来源：http://tmm.mhx1999.top

TS:   s.split("a").length - 1
来源：http://svx.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tfg.ivvv.top

Go:   strings.Count(s, "a")
来源：http://lwi.sjlbkw.cn

Ruby: s.count("a")
来源：http://sbc.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://nlp.xuanzx.com

[E13] 逐字符遍历
来源：http://ckm.pycfn.com

Py:   for ch in s: print(ch)
来源：http://dwt.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://liw.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dzk.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://exq.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mgf.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ktw.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://owt.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ttz.tanke756.top

[E14] URL 编码与 Base64
来源：http://twk.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qsj.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://twi.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uid.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://euz.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eih.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nru.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bpt.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kch.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://utr.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://csx.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tgs.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ozh.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://zei.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gdu.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ctl.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mfq.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://szg.hysaishi.cn

[E16] 数字千分位
来源：http://abr.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://tbz.shzxlz.cn

PHP:  number_format(1234567);
来源：http://zhh.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hig.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pju.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sok.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rsf.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://osy.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://xgn.nwbrower.top

[E17] 首字母大写
来源：http://fht.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mij.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://lps.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zwm.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmq.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ohs.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ayy.yj20258.top

Ruby: s.capitalize
来源：http://xcu.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zlv.52xcode.cn

[E18] 模板占位符替换
来源：http://pjy.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vqu.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://txt.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xuz.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ffu.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ite.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vtf.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ict.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wzf.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://ggx.jiagoushi.top

Py:   s.splitlines()
来源：http://qpa.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ixk.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://swb.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://lqj.c1oappe.top

Java: s.lines().toList()
来源：http://ayb.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://cfv.sweek.top

Ruby: s.lines
来源：http://gap.yuanzhike.top

C#:   s.Split('\n')
来源：http://pis.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://qng.gogol.net.cn

Py:   if not s:
来源：http://tue.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lmk.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://szh.xuanzx.com

TS:   if (s === "") {}
来源：http://snt.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://oby.zhengqikj.top

Go:   if s == "" {}
来源：http://mos.cucudq.cn

Ruby: if s.empty?
来源：http://iau.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mik.xylfe.cn

[E21] 超长截断加省略号
来源：http://hdi.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wfk.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rpm.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgi.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogz.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oua.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://glu.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tfq.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dek.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://pyj.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txo.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jyj.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vqk.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vor.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uuq.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kye.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://wrv.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sma.gotoacloud.top

================================================================================
来源：http://yfk.daxiang520.top

F. 文件与目录
来源：http://fzi.svipenyu.cn

================================================================================
来源：http://kgq.wangdashe.top

[F01] 读取整个文件
来源：http://siy.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ssr.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://xzg.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qvq.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tii.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://eyq.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yck.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://oeg.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://snn.jqgfzy.top

[F02] 逐行读取文件
来源：http://obv.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cvd.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ess.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfv.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpp.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://edf.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ebh.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qca.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oha.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://bxo.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nmi.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wyp.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkl.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ikb.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pxz.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nlx.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://nlt.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qjl.jqgfzy.top

[F04] 追加写入文件
来源：http://dys.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lak.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xty.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bgu.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oli.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ngu.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qyf.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dja.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vxv.sweek.top

[F05] 判断文件或目录是否存在
来源：http://brn.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nyd.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://rjh.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://rcf.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://taw.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iio.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ycr.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://zko.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://hea.ctjpmb.com

[F06] 删除文件
来源：http://dxx.ybcxt.top

Py:   os.remove("a.txt")
来源：http://abp.andypj.xyz

PHP:  unlink("a.txt");
来源：http://gop.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dyi.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mye.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gco.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://apn.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://vuu.yj20258.top

C#:   File.Delete("a.txt");
来源：http://vjp.fktsv.cn

[F07] 创建目录（含多级）
来源：http://vbi.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lxn.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://edj.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihk.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://olx.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ikg.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dsh.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mub.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bwb.ehwqpu.com

[F08] 遍历目录
来源：http://lwr.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mtw.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zpt.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://mis.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://kpd.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dwb.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ulo.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://att.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://gjc.kuanghao11.cn

[F09] 获取文件大小
来源：http://hsy.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://fgb.daxiang520.top

PHP:  filesize("a.txt");
来源：http://rjc.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://ecn.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://fpm.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yhg.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://axd.cashguo.top

Ruby: File.size("a.txt")
来源：http://xnf.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://tit.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://qyi.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sfe.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xeq.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwf.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://tby.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tib.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ims.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dkq.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pho.hesvh.cn

[F11] 复制与移动文件
来源：http://xra.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cyd.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qjv.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dbg.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dot.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jqn.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ioh.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qkj.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eck.hcnkem.com

[F12] CSV 读写
来源：http://dnf.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kuw.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dtb.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wmd.nwbrower.top

TS:   // 同上
来源：http://rbr.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://brt.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lxi.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xqi.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rny.zycfv.cn

================================================================================
来源：http://idl.yj20258.top

G. 面向对象
来源：http://uew.zycfv.cn

================================================================================
来源：http://zoo.hesvh.cn

[G01] 定义类
来源：http://gbl.cdnleiting.top

Py:   class User: pass
来源：http://nie.tanke756.top

PHP:  class User {}
来源：http://ovz.hcnkem.com

JS:   class User {}
来源：http://xjf.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://iiv.jinghuilouyu.cn

Java: class User {}
来源：http://bvz.yj20258888.top

Go:   type User struct { Name string }
来源：http://gje.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://gxy.cucudq.cn

C#:   class User {}
来源：http://snf.fzhhl.top

[G02] 构造函数
来源：http://njk.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://uxf.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://toz.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://tcb.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://lfz.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://kqw.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://psd.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://uue.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://qjx.yuanzhike.top

[G03] 实例属性
来源：http://qlt.guowangkeji.top

Py:   self.name = "x"
来源：http://kqs.jyoumei.cn

PHP:  public string $name = "x";
来源：http://nyi.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://pmw.xylfe.cn

TS:   name: string = "x";
来源：http://msh.ctjpmb.com

Java: private String name;
来源：http://lnt.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bov.birdmap.top

Ruby: @name = "x"
来源：http://vur.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://ule.xuetiantiany.cn

[G04] 定义方法
来源：http://ael.vehdjk.com

Py:   def greet(self): return self.name
来源：http://wom.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sbp.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://tny.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://uth.jqgfzy.top

Java: String greet() { return name; }
来源：http://efc.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oeu.chenzaomai.com

Ruby: def greet; @name; end
来源：http://fbn.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://vyi.ybcxt.top

[G05] 继承
来源：http://wwr.bbcook.cn

Py:   class Admin(User): pass
来源：http://kkm.hammf.cn

PHP:  class Admin extends User {}
来源：http://lix.cdnleiting.top

JS:   class Admin extends User {}
来源：http://wqj.daxiang520.top

TS:   class Admin extends User {}
来源：http://wfm.mhx1999.top

Java: class Admin extends User {}
来源：http://ijj.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hub.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://kmz.guannengcc.top

C#:   class Admin : User {}
来源：http://bpe.wangshuangyany.cn

[G06] 重写方法
来源：http://gql.sweek.top

Py:   def greet(self): return "admin"
来源：http://laj.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sjj.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://plq.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://ybo.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://iuj.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vpu.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://vbo.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://ilc.wangdashe.top

[G07] 调用父类方法
来源：http://vto.daxiang520.top

Py:   super().greet()
来源：http://ltk.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://qtt.fengsongda.top

JS:   super.greet();
来源：http://rno.mhx1999.top

TS:   super.greet();
来源：http://skz.zycfv.cn

Java: super.greet();
来源：http://jkk.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mrs.cucudq.cn

Ruby: super
来源：http://hmd.hfpthk.cn

C#:   base.Greet();
来源：http://cso.ehwqpu.com

[G08] 静态方法与属性
来源：http://kbk.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ldv.shzxlz.cn

PHP:  public static function f() {}
来源：http://jwo.52xcode.cn

JS:   static f() {}
来源：http://bvq.yongpay.top

TS:   static f(): void {}
来源：http://ypc.hesvh.cn

Java: static void f() {}
来源：http://bmt.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://agj.redwolf501.top

Ruby: def self.f; end
来源：http://ken.fehbvm.com

C#:   public static void F() {}
来源：http://cjx.zycfv.cn

[G09] 接口 / 抽象类
来源：http://aio.sxryk.cn


<!-- 参考信息 -->