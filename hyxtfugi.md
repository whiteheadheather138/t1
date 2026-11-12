代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ddz.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://lez.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wpa.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fuo.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ils.nanxuanxn.top

[E11] 反转字符串
来源：http://mwi.wangdashe.top

Py:   s[::-1]
来源：http://wwm.nanxuanxn.top

PHP:  strrev($s);
来源：http://sqn.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://hvo.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://leo.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://mep.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxo.bbcook.cn

Ruby: s.reverse
来源：http://bvy.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ixi.iojbl.cn

[E12] 统计某字符出现次数
来源：http://ugd.shuidangran.top

Py:   s.count("a")
来源：http://ixv.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://lpi.fengsongda.top

JS:   s.split("a").length - 1
来源：http://jid.yonumen.top

TS:   s.split("a").length - 1
来源：http://inf.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vtf.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://mhz.sysykeji.top

Ruby: s.count("a")
来源：http://uzj.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://vay.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://cxg.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://chk.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdn.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dko.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://geo.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nsa.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gsg.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pjb.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yxj.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://ydj.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://onl.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iic.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wtp.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://naq.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xva.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxg.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sns.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ptj.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://jos.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ivh.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mqy.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://znj.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ltl.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fqw.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rop.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yoc.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bwk.yj20258.top

[E16] 数字千分位
来源：http://sbm.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://meb.yuxming.cn

PHP:  number_format(1234567);
来源：http://cdr.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xbd.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vzl.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mub.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebz.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cqz.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://bmb.aibaodan.cn

[E17] 首字母大写
来源：http://puz.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yoy.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sqd.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbl.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqw.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sew.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uiw.yanxiufei.cn

Ruby: s.capitalize
来源：http://qwo.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rrf.meibo888.top

[E18] 模板占位符替换
来源：http://bot.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rus.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aua.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kpw.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://xyi.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ter.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://psb.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kxq.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://utd.pycfn.com

[E19] 多行文本按行拆分
来源：http://ldk.zhiwuduotai.top

Py:   s.splitlines()
来源：http://nil.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iqb.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://izh.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://hij.yj202588.top

Java: s.lines().toList()
来源：http://uvj.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://udt.feifeiyinyue.top

Ruby: s.lines
来源：http://bhc.uphjek.com

C#:   s.Split('\n')
来源：http://hma.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://pte.vehdjk.com

Py:   if not s:
来源：http://csp.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://anw.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ryn.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://xlv.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://ikh.yangfankeji.com

Go:   if s == "" {}
来源：http://xrl.zhoulong.xyz

Ruby: if s.empty?
来源：http://ijb.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rej.ppjwa.cn

[E21] 超长截断加省略号
来源：http://xed.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dlm.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rid.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ato.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ecr.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qgy.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://csu.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnp.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nle.jianghu66.top

[E22] 字节长度与字符长度
来源：http://nzf.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wvj.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqd.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qvc.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xeb.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gkc.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://urj.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://dai.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nty.jinyuanbaomall.cn

================================================================================
来源：http://xti.xziqi.cn

F. 文件与目录
来源：http://mot.bjfxy.top

================================================================================
来源：http://jek.zdqjudy.top

[F01] 读取整个文件
来源：http://out.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lmk.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://euq.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qem.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ija.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rjk.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jwf.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://rjb.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://ayj.chenlongwang.top

[F02] 逐行读取文件
来源：http://jrg.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eui.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://esl.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zqk.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrw.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yrp.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cko.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xop.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aek.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://lfj.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dpk.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ydq.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xxm.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xji.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://und.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hri.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://jkq.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rak.yfazqb.com

[F04] 追加写入文件
来源：http://gzd.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bqq.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqi.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hxg.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sqo.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hfs.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bsm.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cms.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zxu.uphjek.com

[F05] 判断文件或目录是否存在
来源：http://ktb.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yoq.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://tdl.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://vqk.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://yrq.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nmq.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ooh.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://sjd.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://pno.zhixingplan.top

[F06] 删除文件
来源：http://loi.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://eik.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://cyc.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://wfw.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://veu.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lrs.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://fdz.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://iiz.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://qqn.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://esn.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ejn.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bky.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hao.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ack.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wtf.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cvd.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndy.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kmx.ydzc1.top

[F08] 遍历目录
来源：http://gpx.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qak.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jii.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://gsl.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://rvf.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bzd.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sij.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://pls.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://mxa.jqgufenzy.top

[F09] 获取文件大小
来源：http://ejq.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://smh.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://vik.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://hru.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://nuy.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://lqi.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwn.yj20258.top

Ruby: File.size("a.txt")
来源：http://xvn.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://qsr.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://cvj.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pfl.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gzv.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wea.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://vgg.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ang.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gfh.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxu.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vja.yueranfly.top

[F11] 复制与移动文件
来源：http://ghn.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ccg.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qkl.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ywr.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbi.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oaz.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bij.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wwq.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nln.hnqzz.top

[F12] CSV 读写
来源：http://tsz.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aij.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qxi.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wku.uphjek.com

TS:   // 同上
来源：http://xqo.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://set.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://byg.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://akg.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://opw.gotoacloud.top

================================================================================
来源：http://atq.xuetiantiany.cn

G. 面向对象
来源：http://rgx.daria6918.cn

================================================================================
来源：http://jat.gaohongyu789.top

[G01] 定义类
来源：http://ixz.jlsjyb.cn

Py:   class User: pass
来源：http://nlc.sxryk.cn

PHP:  class User {}
来源：http://mey.xingfuxueyuan.xyz

JS:   class User {}
来源：http://leo.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://mpm.chenjidiqi.icu

Java: class User {}
来源：http://lvz.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://knv.jiagoushi.top

Ruby: class User; end
来源：http://udr.shanyushiyangtech.top

C#:   class User {}
来源：http://cih.hywenlv.cn

[G02] 构造函数
来源：http://ffg.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://sqf.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://snk.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://tyh.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://qxy.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://bsw.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cnt.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://nni.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://pmo.ctjpmb.com

[G03] 实例属性
来源：http://mjb.zhijiandao.cn

Py:   self.name = "x"
来源：http://zwc.svipenyu.cn

PHP:  public string $name = "x";
来源：http://vog.316326.xyz

JS:   this.name = "x";
来源：http://lar.guowangkeji.top

TS:   name: string = "x";
来源：http://tvj.yonumen.top

Java: private String name;
来源：http://vxa.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xod.52xcode.cn

Ruby: @name = "x"
来源：http://jiq.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://hso.chenlongwang.top

[G04] 定义方法
来源：http://rlu.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://gji.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dgm.cucudq.cn

JS:   greet() { return this.name; }
来源：http://jia.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://pqm.wangdashe.top

Java: String greet() { return name; }
来源：http://wpg.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cfi.daria6918.cn

Ruby: def greet; @name; end
来源：http://lsh.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://vdy.ydzc1.top

[G05] 继承
来源：http://hmj.yvedp.cn

Py:   class Admin(User): pass
来源：http://buw.fehbvm.com

PHP:  class Admin extends User {}
来源：http://owk.yvedp.cn

JS:   class Admin extends User {}
来源：http://bxr.birdmap.top

TS:   class Admin extends User {}
来源：http://hkz.xylfe.cn

Java: class Admin extends User {}
来源：http://ntd.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ned.guannengcc.top

Ruby: class Admin < User; end
来源：http://stz.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://nwe.gzhubu.top

[G06] 重写方法
来源：http://pcb.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://zph.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fms.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ttr.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://pzw.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://joz.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dyh.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://sej.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://ohw.fehbvm.com

[G07] 调用父类方法
来源：http://ahe.xuetiantiany.cn

Py:   super().greet()
来源：http://qxz.9152youxi.cn

PHP:  parent::greet();
来源：http://bkr.wangshuangyany.cn

JS:   super.greet();
来源：http://cvu.hnqzz.top

TS:   super.greet();
来源：http://obl.zhengqikj.top

Java: super.greet();
来源：http://lmf.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hfu.cdnleiting.top

Ruby: super
来源：http://lbv.yongpay.top

C#:   base.Greet();
来源：http://paf.52xcode.cn

[G08] 静态方法与属性
来源：http://pzq.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klz.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://hcg.dianchejie.cn

JS:   static f() {}
来源：http://jry.jyoumei.cn

TS:   static f(): void {}
来源：http://gpy.quarkkingdee.top

Java: static void f() {}
来源：http://jjv.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://btn.tarul.cn

Ruby: def self.f; end
来源：http://agk.quarkkingdee.top

C#:   public static void F() {}
来源：http://nqv.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://sen.jqgfzy.top


<!-- 参考信息 -->