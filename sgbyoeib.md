代发 wailian999

JS:   [...s].reverse().join("")
来源：http://irm.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://xfg.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ivd.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kpk.aibaodan.cn

Ruby: s.reverse
来源：http://fsc.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zuh.52xcode.cn

[E12] 统计某字符出现次数
来源：http://ljf.zhijiandao.cn

Py:   s.count("a")
来源：http://nsa.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://mom.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://mng.fzhhl.top

TS:   s.split("a").length - 1
来源：http://ekh.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rtk.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://vtr.smart0.xyz

Ruby: s.count("a")
来源：http://vhi.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://tbc.redwolf501.top

[E13] 逐字符遍历
来源：http://knh.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://mrx.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fxp.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xwo.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lms.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oqq.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ofp.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zgb.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ejm.ivvv.top

[E14] URL 编码与 Base64
来源：http://ojx.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oam.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nup.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hdq.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://odn.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qeq.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vhp.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gqn.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jzr.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://tes.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ima.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yjm.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wsv.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://btn.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gfg.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ydw.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://brn.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wzy.zhixingplan.top

[E16] 数字千分位
来源：http://anw.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://wiy.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://umn.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yrj.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rht.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zod.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yvs.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bny.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://vqn.zdqjudy.top

[E17] 首字母大写
来源：http://jow.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxy.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fiq.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://low.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mie.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lth.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rnq.nanxinkj.top

Ruby: s.capitalize
来源：http://ugx.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bti.sjlbkw.cn

[E18] 模板占位符替换
来源：http://wjc.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ztd.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ubh.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ulu.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xwu.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://trs.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jeq.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cmv.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://imc.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://nlo.cqqwz.cn

Py:   s.splitlines()
来源：http://ejx.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xvg.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://buf.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://hwk.cqqwz.cn

Java: s.lines().toList()
来源：http://uqx.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://olc.sysykeji.top

Ruby: s.lines
来源：http://jbp.0kj1m.cn

C#:   s.Split('\n')
来源：http://yzc.yj20258.top

[E20] 判断字符串是否为空
来源：http://kum.jqgfzy.top

Py:   if not s:
来源：http://nbk.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ann.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jje.jinqigfzy.top

TS:   if (s === "") {}
来源：http://adr.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://rit.shuidangran.top

Go:   if s == "" {}
来源：http://tdz.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://dod.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://prt.ybcxt.top

[E21] 超长截断加省略号
来源：http://qri.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxt.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgi.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhc.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdz.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://flb.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://htf.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://unv.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nwk.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://okg.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dvw.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kmd.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpg.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ufp.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gqk.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gdd.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://sxs.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xsx.ydjk.org.cn

================================================================================
来源：http://sob.pengpengdd.cyou

F. 文件与目录
来源：http://lzp.sufxvd.cn

================================================================================
来源：http://pjg.guannengcc.top

[F01] 读取整个文件
来源：http://kwd.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zxz.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://djm.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ttw.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://utd.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tsf.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xku.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://ocp.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://xiu.sjlbkw.cn

[F02] 逐行读取文件
来源：http://isu.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gmw.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://edw.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jkg.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iiq.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vyw.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pnd.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ktl.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nqc.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://gan.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oyt.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pee.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwy.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flq.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://krc.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgi.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://gjm.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hsd.sxryk.cn

[F04] 追加写入文件
来源：http://wel.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vfq.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fhs.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifi.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nhx.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jyi.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vww.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zvh.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tbd.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://sqa.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gts.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://kko.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://upr.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://obc.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lum.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rqp.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://etj.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://rtc.zdbjq.cn

[F06] 删除文件
来源：http://oxw.smart0.xyz

Py:   os.remove("a.txt")
来源：http://sxb.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://jcb.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://pzf.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://enw.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uzi.birdmap.top

Go:   os.Remove("a.txt")
来源：http://ofx.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://qvb.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://hut.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://uow.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jwa.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glt.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjo.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bcv.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zgg.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lgs.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://efu.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uso.bbcook.cn

[F08] 遍历目录
来源：http://ysc.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sue.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zqs.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://xmc.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://wlp.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qyh.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yjr.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://sue.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://gyc.bbcook.cn

[F09] 获取文件大小
来源：http://qpa.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://whf.316326.xyz

PHP:  filesize("a.txt");
来源：http://vcq.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://xie.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://cjs.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://vwc.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xkr.fengsongda.top

Ruby: File.size("a.txt")
来源：http://kil.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://ihp.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://kuc.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vlv.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pjv.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jnh.ivvv.top

TS:   path.extname("a.txt")
来源：http://jzv.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxj.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mof.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bgo.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://shb.shzxlz.cn

[F11] 复制与移动文件
来源：http://ntm.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://whu.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://swx.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyd.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjs.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bkk.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://knr.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tii.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kcn.sysykeji.top

[F12] CSV 读写
来源：http://xwr.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ynu.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pcb.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://alf.hammf.cn

TS:   // 同上
来源：http://smx.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wgb.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ayp.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sbr.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hwg.shanyushiyangtech.top

================================================================================
来源：http://iep.epnwcf.com

G. 面向对象
来源：http://xyu.shuidangran.top

================================================================================
来源：http://hqx.hcnkem.com

[G01] 定义类
来源：http://qzu.daxiang520.top

Py:   class User: pass
来源：http://cah.cqqwz.cn

PHP:  class User {}
来源：http://akt.iojbl.cn

JS:   class User {}
来源：http://eql.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://fwx.hnqzz.top

Java: class User {}
来源：http://ivv.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://ekp.yongpay.top

Ruby: class User; end
来源：http://epf.yj20258.top

C#:   class User {}
来源：http://prc.shuidangran.top

[G02] 构造函数
来源：http://esx.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://gdm.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://xtt.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://gcm.pycfn.com

TS:   constructor(public name: string) {}
来源：http://qkp.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://nzw.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vsg.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://yaq.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://zjy.yj20258.top

[G03] 实例属性
来源：http://aiz.cheryme.top

Py:   self.name = "x"
来源：http://atj.iojbl.cn

PHP:  public string $name = "x";
来源：http://nsv.gotoacloud.top

JS:   this.name = "x";
来源：http://nnc.meibo888.top

TS:   name: string = "x";
来源：http://umk.hnqzz.top

Java: private String name;
来源：http://jbr.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rlh.yonumen.top

Ruby: @name = "x"
来源：http://zrz.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://opr.ehwqpu.com

[G04] 定义方法
来源：http://cvu.uphjek.com

Py:   def greet(self): return self.name
来源：http://jhv.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://drw.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://kxu.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://xhb.cdnleiting.top

Java: String greet() { return name; }
来源：http://kii.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qwp.yj20258888.top

Ruby: def greet; @name; end
来源：http://eic.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://hka.fanxiaobao.xyz

[G05] 继承
来源：http://vpn.xylfe.cn

Py:   class Admin(User): pass
来源：http://bdp.uphjek.com

PHP:  class Admin extends User {}
来源：http://tab.ydzc1.top

JS:   class Admin extends User {}
来源：http://rjr.jianghu66.top

TS:   class Admin extends User {}
来源：http://fgb.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://gzz.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kwp.ybcxt.top

Ruby: class Admin < User; end
来源：http://yng.yongpay.top

C#:   class Admin : User {}
来源：http://uum.yangfankeji.com

[G06] 重写方法
来源：http://vel.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://jlo.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vbi.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://osp.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://zzl.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://zsg.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pfd.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://lgj.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://esy.xinyue.icu

[G07] 调用父类方法
来源：http://cwl.shanyushiyangkeji.top

Py:   super().greet()
来源：http://cxd.c1oappe.top

PHP:  parent::greet();
来源：http://hqf.sjlbkw.cn

JS:   super.greet();
来源：http://eac.aibaodan.cn

TS:   super.greet();
来源：http://gwv.xuetiantiany.cn

Java: super.greet();
来源：http://zia.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bxi.zhaomingkeji.xyz

Ruby: super
来源：http://rxx.tianlin.xyz

C#:   base.Greet();
来源：http://mtd.yj20258888.top

[G08] 静态方法与属性
来源：http://eri.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hcj.ybcxt.top

PHP:  public static function f() {}
来源：http://emj.zhixingplan.top

JS:   static f() {}
来源：http://zuw.sufxvd.cn

TS:   static f(): void {}
来源：http://rof.yonumen.top

Java: static void f() {}
来源：http://rxk.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxc.hammf.cn

Ruby: def self.f; end
来源：http://jva.tian-w.cn

C#:   public static void F() {}
来源：http://qam.daria6918.cn

[G09] 接口 / 抽象类
来源：http://irf.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://hgu.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uvp.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbp.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://iki.316326.xyz

Java: interface Shape { double area(); }
来源：http://gul.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://zct.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://due.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://iaf.snrcjt.cn


<!-- 参考信息 -->