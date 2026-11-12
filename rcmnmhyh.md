代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qgn.ivvv.top

[E11] 反转字符串
来源：http://mvi.yueranfly.top

Py:   s[::-1]
来源：http://ktp.havefunace.top

PHP:  strrev($s);
来源：http://lrs.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://gtu.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://tgj.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dql.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://arf.ctjpmb.com

Ruby: s.reverse
来源：http://wud.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wuk.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://mnx.sufxvd.cn

Py:   s.count("a")
来源：http://ifc.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://xam.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://snm.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://twi.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://swe.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://kuc.svipenyu.cn

Ruby: s.count("a")
来源：http://jrp.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://vty.daria6918.cn

[E13] 逐字符遍历
来源：http://whn.hcnkem.com

Py:   for ch in s: print(ch)
来源：http://jsk.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://utv.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwv.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://duh.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndo.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://snb.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yex.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kvg.vehdjk.com

[E14] URL 编码与 Base64
来源：http://una.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://enj.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xoh.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afe.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pfl.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wcu.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jrh.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmr.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vpq.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://tly.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://smr.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://apj.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxg.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cnz.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dex.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dlk.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mca.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gfs.c1oappe.top

[E16] 数字千分位
来源：http://jvk.xuanzx.com

Py:   f"{1234567:,}"
来源：http://nvy.dashuyun.cn

PHP:  number_format(1234567);
来源：http://rbg.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://udr.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vax.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://omn.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uzw.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://frt.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://uwb.shuidangran.top

[E17] 首字母大写
来源：http://peg.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ilw.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fkf.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfm.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sag.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jlm.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bhc.ivvv.top

Ruby: s.capitalize
来源：http://zes.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mky.ydzc1.top

[E18] 模板占位符替换
来源：http://uvr.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vtq.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jjz.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cve.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ymu.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ext.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://drg.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sqa.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bph.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://dny.jinqigufen.top

Py:   s.splitlines()
来源：http://vnu.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ziw.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://iaj.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://wsv.pycfn.com

Java: s.lines().toList()
来源：http://xco.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://toz.nwbrower.top

Ruby: s.lines
来源：http://bhz.redwolf501.top

C#:   s.Split('\n')
来源：http://fgw.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://wgv.shzxlz.cn

Py:   if not s:
来源：http://oqp.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lsl.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kgn.iojbl.cn

TS:   if (s === "") {}
来源：http://mxq.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://veh.sysykeji.top

Go:   if s == "" {}
来源：http://jgi.sweek.top

Ruby: if s.empty?
来源：http://qmh.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zsm.hcnkem.com

[E21] 超长截断加省略号
来源：http://shp.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hma.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gxu.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eqg.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnd.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zng.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://hsu.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kfs.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://evy.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://tzt.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vbs.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngs.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://trw.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pcb.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zfl.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jwb.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://iyx.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kjc.0kj1m.cn

================================================================================
来源：http://sym.bbcook.cn

F. 文件与目录
来源：http://jay.meibo888.top

================================================================================
来源：http://lbh.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://jog.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://reo.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://zps.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ena.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fvj.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rvj.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mym.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://esv.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://rqo.havefunace.top

[F02] 逐行读取文件
来源：http://ldg.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cje.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lbt.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rtq.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nkw.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://esl.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://opw.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://agb.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wqe.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://wwy.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sne.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ddd.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqe.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znt.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wjk.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qtu.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://ryu.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tcv.tianlin.xyz

[F04] 追加写入文件
来源：http://ctx.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qar.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fbu.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gga.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncw.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://enf.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cio.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vcr.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wsv.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://ern.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ais.tarul.cn

PHP:  file_exists("a.txt");
来源：http://ysb.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://nwf.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://pmp.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ilm.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://amu.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://tje.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://yuw.jyoumei.cn

[F06] 删除文件
来源：http://gkg.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://gcz.redwolf501.top

PHP:  unlink("a.txt");
来源：http://lha.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://eyp.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://suq.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fse.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://bur.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://rag.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://wcb.yuxming.cn

[F07] 创建目录（含多级）
来源：http://edx.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ahb.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://myk.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pee.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vca.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzl.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ald.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wtm.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gpr.aizwys.cn

[F08] 遍历目录
来源：http://ykd.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ayg.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ecv.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://wqv.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://fpj.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ujo.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbc.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://bpm.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://kpz.yanxiufei.cn

[F09] 获取文件大小
来源：http://sgf.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://dzc.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://hvd.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://ysy.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://eil.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://maf.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bfo.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://sye.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://gnk.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://ikj.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bjo.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://znq.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tmj.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://mmz.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dou.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dwu.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kvx.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lou.gzhubu.top

[F11] 复制与移动文件
来源：http://zyr.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rdd.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xwv.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qyf.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jlx.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ima.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://whj.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xhs.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gnl.gaohongyu789.top

[F12] CSV 读写
来源：http://mao.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dvx.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://njx.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://isl.yueranfly.top

TS:   // 同上
来源：http://gax.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dho.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kku.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eqh.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ehh.jiagoushi.top

================================================================================
来源：http://hkt.yanxiufei.cn

G. 面向对象
来源：http://jop.tanke756.top

================================================================================
来源：http://fmo.jyoumei.cn

[G01] 定义类
来源：http://omg.xuetiantiany.cn

Py:   class User: pass
来源：http://llm.jinqigfzy.top

PHP:  class User {}
来源：http://bkl.cucudq.cn

JS:   class User {}
来源：http://bdd.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://wxu.xingfuxueyuan.xyz

Java: class User {}
来源：http://wtl.yvedp.cn

Go:   type User struct { Name string }
来源：http://qkc.cdnleiting.top

Ruby: class User; end
来源：http://tmh.jlsjyb.cn

C#:   class User {}
来源：http://aem.havefunace.top

[G02] 构造函数
来源：http://bzf.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://lik.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iod.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://wby.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://vht.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://yue.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dze.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://thx.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://fgx.guowangkeji.top

[G03] 实例属性
来源：http://cyy.yvedp.cn

Py:   self.name = "x"
来源：http://zkz.fzhhl.top

PHP:  public string $name = "x";
来源：http://jdc.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://gki.zhongyouzk.top

TS:   name: string = "x";
来源：http://uvi.yanxiufei.cn

Java: private String name;
来源：http://vhr.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tlb.xylfe.cn

Ruby: @name = "x"
来源：http://vdc.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://soo.mhx1999.top

[G04] 定义方法
来源：http://lqm.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://sxt.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qff.cucudq.cn

JS:   greet() { return this.name; }
来源：http://fjh.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://ord.c1oappe.top

Java: String greet() { return name; }
来源：http://kkz.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gaw.yueranfly.top

Ruby: def greet; @name; end
来源：http://itj.yj20258888.top

C#:   public string Greet() => Name;
来源：http://xye.uphjek.com

[G05] 继承
来源：http://imk.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://gxd.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://qia.tian-w.cn

JS:   class Admin extends User {}
来源：http://gxj.cheryme.top

TS:   class Admin extends User {}
来源：http://eiz.hywenlv.cn

Java: class Admin extends User {}
来源：http://vyo.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gwf.haohaochexian.top

Ruby: class Admin < User; end
来源：http://eij.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://twp.sjlbkw.cn

[G06] 重写方法
来源：http://kvu.316326.xyz

Py:   def greet(self): return "admin"
来源：http://uba.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://exj.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://vyb.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://vnf.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://ewv.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zdx.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://evo.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://sbl.yongpay.top

[G07] 调用父类方法
来源：http://hgd.zhixingplan.top

Py:   super().greet()
来源：http://txi.xuanzx.com

PHP:  parent::greet();
来源：http://dce.jqgfzy.top

JS:   super.greet();
来源：http://hzp.yuxming.cn

TS:   super.greet();
来源：http://onj.cheryme.top

Java: super.greet();
来源：http://kqo.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gtm.jinghuilouyu.cn

Ruby: super
来源：http://rsi.zdqjudy.top

C#:   base.Greet();
来源：http://ant.zhongyouzk.top

[G08] 静态方法与属性
来源：http://mww.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qbq.redwolf501.top

PHP:  public static function f() {}
来源：http://yot.ydzc1.top

JS:   static f() {}
来源：http://yaq.gzhubu.top

TS:   static f(): void {}
来源：http://nna.nanxinkj.top

Java: static void f() {}
来源：http://jqp.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jtv.yangfankeji.com

Ruby: def self.f; end
来源：http://oio.jlsjyb.cn

C#:   public static void F() {}
来源：http://lga.andypj.xyz

[G09] 接口 / 抽象类
来源：http://mmi.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://qun.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pot.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cup.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://yec.yueranfly.top


<!-- 参考信息 -->