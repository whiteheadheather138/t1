代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hpt.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://zhb.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tcm.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qah.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xyx.daxiang520.top

[E11] 反转字符串
来源：http://fmu.sysykeji.top

Py:   s[::-1]
来源：http://zmc.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://ist.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://gsk.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://eqa.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ljs.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hmv.shangyingyoupin.top

Ruby: s.reverse
来源：http://xqd.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://vvq.smart0.xyz

[E12] 统计某字符出现次数
来源：http://hbu.gogol.net.cn

Py:   s.count("a")
来源：http://pyj.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://loh.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://qfj.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://jrb.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vul.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://pyd.cashguo.top

Ruby: s.count("a")
来源：http://qfz.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://bus.cucudq.cn

[E13] 逐字符遍历
来源：http://mxr.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://khy.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vci.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aoa.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pik.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oxu.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fzv.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rcl.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wmp.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://hyl.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zlb.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vrb.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mub.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zoq.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dsh.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bex.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rej.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ign.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://hxa.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mnd.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bod.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uyw.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vcl.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wmc.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vwk.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gta.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fii.ydjk.org.cn

[E16] 数字千分位
来源：http://aao.shuidangran.top

Py:   f"{1234567:,}"
来源：http://qye.yueranfly.top

PHP:  number_format(1234567);
来源：http://maf.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wpz.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nat.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nqw.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjo.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jni.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://yvc.wangshuangyany.cn

[E17] 首字母大写
来源：http://inn.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xpw.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ral.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lfh.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogr.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bos.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fdm.snrcjt.cn

Ruby: s.capitalize
来源：http://lcy.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qhq.sysykeji.top

[E18] 模板占位符替换
来源：http://xlc.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jnp.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tbe.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oba.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nkf.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zmk.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nkq.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvz.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nub.fengsongda.top

[E19] 多行文本按行拆分
来源：http://gar.wangdashe.top

Py:   s.splitlines()
来源：http://tuh.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zts.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://zhw.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://nqf.yj20258888.top

Java: s.lines().toList()
来源：http://vtv.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://yqq.tarul.cn

Ruby: s.lines
来源：http://oxj.fengsongda.top

C#:   s.Split('\n')
来源：http://ukf.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://azo.yvedp.cn

Py:   if not s:
来源：http://yoq.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oba.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tqc.yj202588.top

TS:   if (s === "") {}
来源：http://cmp.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://ztm.hammf.cn

Go:   if s == "" {}
来源：http://tgc.iojbl.cn

Ruby: if s.empty?
来源：http://nyv.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zrv.tarul.cn

[E21] 超长截断加省略号
来源：http://lim.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wdw.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ogf.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lnw.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftx.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gcy.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://nyc.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nts.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://krg.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://qlo.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://red.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rtc.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qlw.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uls.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://shk.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fud.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://skn.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fce.tanke756.top

================================================================================
来源：http://ano.haohaochexian.top

F. 文件与目录
来源：http://wbh.pycfn.com

================================================================================
来源：http://fps.zhongyouzk.top

[F01] 读取整个文件
来源：http://nie.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ltl.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://fsw.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://izw.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kyd.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gsu.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://spe.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://guz.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://caj.nanxinkj.top

[F02] 逐行读取文件
来源：http://qvn.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jsu.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbw.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tun.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mhc.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ehh.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qqr.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uzn.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ntb.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://eyp.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yzi.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://hhv.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbx.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://syj.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kkz.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yxk.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://wgr.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gnp.smart0.xyz

[F04] 追加写入文件
来源：http://smb.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vet.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://khl.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wwb.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iml.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xtx.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://krf.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbl.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cfx.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://iqc.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uup.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://vsh.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://rch.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://wcw.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bpa.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wzq.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://gcx.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://lqk.yonumen.top

[F06] 删除文件
来源：http://gpf.hammf.cn

Py:   os.remove("a.txt")
来源：http://baq.yj202588.top

PHP:  unlink("a.txt");
来源：http://vvt.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pyz.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://whr.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhf.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://nhs.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://pqx.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://cma.fzhhl.top

[F07] 创建目录（含多级）
来源：http://tws.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hdt.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wav.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jri.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxl.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cey.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uyh.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ntn.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jlq.hongshengwenyu.top

[F08] 遍历目录
来源：http://hie.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rsl.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dtm.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://qhl.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://jsm.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugm.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zrt.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://rnx.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://dcg.cashguo.top

[F09] 获取文件大小
来源：http://fdn.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://zsm.xinyue.icu

PHP:  filesize("a.txt");
来源：http://wke.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://yvs.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://mxn.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ujk.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zaf.yongpay.top

Ruby: File.size("a.txt")
来源：http://nea.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://cqg.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://jem.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lob.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zmw.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jsq.birdmap.top

TS:   path.extname("a.txt")
来源：http://qec.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uzd.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fwk.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pks.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vzt.yfazqb.com

[F11] 复制与移动文件
来源：http://tys.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pcu.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vuc.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfn.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vjp.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://prt.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cax.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://khu.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hnu.hammf.cn

[F12] CSV 读写
来源：http://ueo.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sek.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgm.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kzp.sufxvd.cn

TS:   // 同上
来源：http://aqz.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zcu.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sqj.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xbe.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lrl.chenjidiqi.icu

================================================================================
来源：http://aup.guowangkeji.top

G. 面向对象
来源：http://lhg.uphjek.com

================================================================================
来源：http://auk.cqqwz.cn

[G01] 定义类
来源：http://hbl.hysaishi.cn

Py:   class User: pass
来源：http://wnz.c1oappe.top

PHP:  class User {}
来源：http://fge.yueranfly.top

JS:   class User {}
来源：http://fbc.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://wxc.jiagoushi.top

Java: class User {}
来源：http://hcs.andypj.xyz

Go:   type User struct { Name string }
来源：http://icv.ywan-chungtsiang.top

Ruby: class User; end
来源：http://mru.chenzaomai.com

C#:   class User {}
来源：http://oee.xuetiantiany.cn

[G02] 构造函数
来源：http://wup.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://rbk.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://bim.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://cnd.cheryme.top

TS:   constructor(public name: string) {}
来源：http://dag.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://gwg.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fbl.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://rcj.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://yhh.jlsjyb.cn

[G03] 实例属性
来源：http://cgn.zhiwuduotai.top

Py:   self.name = "x"
来源：http://crh.9152youxi.cn

PHP:  public string $name = "x";
来源：http://vwl.chenjidiqi.icu

JS:   this.name = "x";
来源：http://gvu.hysaishi.cn

TS:   name: string = "x";
来源：http://pew.nanxinkj.top

Java: private String name;
来源：http://wyg.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iov.9152youxi.cn

Ruby: @name = "x"
来源：http://ipo.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://zvu.snrcjt.cn

[G04] 定义方法
来源：http://ggv.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://nzs.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hgo.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://oki.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://atz.sufxvd.cn

Java: String greet() { return name; }
来源：http://rpv.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rpy.cqqwz.cn

Ruby: def greet; @name; end
来源：http://xql.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://lxz.jinqigfzy.top

[G05] 继承
来源：http://blg.dashuyun.cn

Py:   class Admin(User): pass
来源：http://dos.xylfe.cn

PHP:  class Admin extends User {}
来源：http://woy.xinyue.icu

JS:   class Admin extends User {}
来源：http://ips.zdbjq.cn

TS:   class Admin extends User {}
来源：http://qlj.zhixingplan.top

Java: class Admin extends User {}
来源：http://ecc.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ith.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://ags.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://qfz.daxiang520.top

[G06] 重写方法
来源：http://awa.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://gbd.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://njg.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://wbo.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://pyf.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://meb.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oyk.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://zwr.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://gnq.vqdsnc.cn

[G07] 调用父类方法
来源：http://man.pycfn.com

Py:   super().greet()
来源：http://duw.svipenyu.cn

PHP:  parent::greet();
来源：http://zrb.shangyingyoupin.top

JS:   super.greet();
来源：http://vrj.uphjek.com

TS:   super.greet();
来源：http://nds.kuanghao11.cn

Java: super.greet();
来源：http://vze.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mtc.jinqigfzy.top

Ruby: super
来源：http://kss.shuidangran.top

C#:   base.Greet();
来源：http://tot.kuanghao11.cn

[G08] 静态方法与属性
来源：http://iqy.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aun.hnqzz.top

PHP:  public static function f() {}
来源：http://guc.chenjidiqi.icu

JS:   static f() {}
来源：http://sop.yuanzhike.top

TS:   static f(): void {}
来源：http://gym.xuetiantiany.cn

Java: static void f() {}
来源：http://tqb.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cnq.tian-w.cn

Ruby: def self.f; end
来源：http://foy.fengsongda.top

C#:   public static void F() {}
来源：http://wnd.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://xyn.pengpengdd.cyou


<!-- 参考信息 -->