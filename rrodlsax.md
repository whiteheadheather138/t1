代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://dzu.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://qwt.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tyu.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pgx.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://atw.andypj.xyz

[E11] 反转字符串
来源：http://cub.316326.xyz

Py:   s[::-1]
来源：http://rdp.jqgfzy.top

PHP:  strrev($s);
来源：http://ncm.meibo888.top

JS:   [...s].reverse().join("")
来源：http://qty.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://ock.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gjg.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gti.aibaodan.cn

Ruby: s.reverse
来源：http://vgg.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://bkp.redwolf501.top

[E12] 统计某字符出现次数
来源：http://ucu.ybcxt.top

Py:   s.count("a")
来源：http://xnp.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://cph.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://obo.cucudq.cn

TS:   s.split("a").length - 1
来源：http://iqm.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qzs.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://uca.yueranfly.top

Ruby: s.count("a")
来源：http://gqa.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://azi.vehdjk.com

[E13] 逐字符遍历
来源：http://voa.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://dou.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://raw.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xgs.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ygy.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hlp.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rhh.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mmq.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yqw.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://zgl.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aal.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uip.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kqn.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ocj.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yyx.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sxx.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dcb.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gzl.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://wrb.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gjk.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kqg.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aox.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kjf.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gor.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ink.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aio.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kqh.316326.xyz

[E16] 数字千分位
来源：http://pzf.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://vxp.yongpay.top

PHP:  number_format(1234567);
来源：http://zic.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uqw.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tqo.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eqd.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fql.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zon.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://abr.jqgufenzy.top

[E17] 首字母大写
来源：http://unk.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wwn.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iyz.hnqzz.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqn.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvb.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dtq.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cil.smart0.xyz

Ruby: s.capitalize
来源：http://wgt.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gie.aibaodan.cn

[E18] 模板占位符替换
来源：http://djs.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eff.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hnk.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nnr.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nfp.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://asd.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ieu.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://elg.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bhg.cucudq.cn

[E19] 多行文本按行拆分
来源：http://avj.zhoulong.xyz

Py:   s.splitlines()
来源：http://tsg.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://anp.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://ldm.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://opy.hysaishi.cn

Java: s.lines().toList()
来源：http://wro.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://qxp.tanke756.top

Ruby: s.lines
来源：http://pdc.jinqigfzy.top

C#:   s.Split('\n')
来源：http://vpn.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://dzw.nwbrower.top

Py:   if not s:
来源：http://kuv.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fnz.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bpf.shuidangran.top

TS:   if (s === "") {}
来源：http://lqf.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://ddx.yueranfly.top

Go:   if s == "" {}
来源：http://dsd.9152youxi.cn

Ruby: if s.empty?
来源：http://ogf.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xwz.dianchejie.cn

[E21] 超长截断加省略号
来源：http://ysi.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sjo.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bbv.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpq.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrd.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bmj.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://rls.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tth.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uoy.fehbvm.com

[E22] 字节长度与字符长度
来源：http://dbx.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tvp.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kci.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pjz.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tee.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xmj.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mfj.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://vig.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sep.hfpthk.cn

================================================================================
来源：http://abm.shzxlz.cn

F. 文件与目录
来源：http://rgu.epnwcf.com

================================================================================
来源：http://vup.epnwcf.com

[F01] 读取整个文件
来源：http://hpg.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gxf.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://uql.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ynr.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oeb.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lcx.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zkv.xuetiantiany.cn

Ruby: File.read("a.txt")
来源：http://oap.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://ycw.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://ngi.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pkd.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vdk.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frr.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfp.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pqq.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jwb.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ilh.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nsl.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://qdk.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wuq.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ztt.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfj.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ina.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnr.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://udd.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://pfn.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://per.hesvh.cn

[F04] 追加写入文件
来源：http://ghv.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ctc.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nxj.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azl.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tmv.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bxy.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jle.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqa.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wlr.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://awx.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oqb.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://pnk.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://akl.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://ukl.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yjh.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ayb.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://ybt.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://hdk.yuanzhike.top

[F06] 删除文件
来源：http://jab.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://ula.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://apx.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://uqq.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tqs.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ooa.yongpay.top

Go:   os.Remove("a.txt")
来源：http://knj.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://srm.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://wdz.guannengcc.top

[F07] 创建目录（含多级）
来源：http://wsw.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hwi.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gdp.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://amv.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mky.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kve.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ynw.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xwd.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pxf.zhixingplan.top

[F08] 遍历目录
来源：http://slz.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xvs.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ghn.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://kdk.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://hqm.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yro.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ewa.jianghu66.top

Ruby: Dir.children("dir")
来源：http://pwz.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://toj.havefunace.top

[F09] 获取文件大小
来源：http://jzj.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://jkt.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://jmc.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://avz.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://lab.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://dvw.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ftz.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://jeh.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://wbl.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://eql.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://byn.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kiw.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wex.redwolf501.top

TS:   path.extname("a.txt")
来源：http://qcp.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ikj.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://efb.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://byv.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://onq.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://cgy.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://znz.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fnt.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xer.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lcb.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bwi.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mez.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ikt.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aqw.sjlbkw.cn

[F12] CSV 读写
来源：http://sqy.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qyt.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbb.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xfz.gotoacloud.top

TS:   // 同上
来源：http://vni.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ofv.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uzn.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ebg.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://duk.xuanzx.com

================================================================================
来源：http://xcb.smart0.xyz

G. 面向对象
来源：http://loq.jinghuilouyu.cn

================================================================================
来源：http://sce.iojbl.cn

[G01] 定义类
来源：http://xdg.hnxiangtu.top

Py:   class User: pass
来源：http://umo.yuanzhike.top

PHP:  class User {}
来源：http://iiv.yj20258.top

JS:   class User {}
来源：http://jtu.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://bqm.xziqi.cn

Java: class User {}
来源：http://wci.yj20258.top

Go:   type User struct { Name string }
来源：http://fdm.hfpthk.cn

Ruby: class User; end
来源：http://spx.zdqjudy.top

C#:   class User {}
来源：http://ydd.yongpay.top

[G02] 构造函数
来源：http://uly.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://dil.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://ueq.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://isn.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://kqp.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://kkk.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://drk.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://egt.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://eau.zhengqikj.top

[G03] 实例属性
来源：http://isw.cdnleiting.top

Py:   self.name = "x"
来源：http://wuj.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://wfi.yj20258888.top

JS:   this.name = "x";
来源：http://esx.hesvh.cn

TS:   name: string = "x";
来源：http://kta.xziqi.cn

Java: private String name;
来源：http://ggo.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ewo.zhixingplan.top

Ruby: @name = "x"
来源：http://ppn.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://sjp.sweek.top

[G04] 定义方法
来源：http://jve.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://wzb.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nln.aizwys.cn

JS:   greet() { return this.name; }
来源：http://dsf.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://zqi.hywenlv.cn

Java: String greet() { return name; }
来源：http://zmq.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iny.shzxlz.cn

Ruby: def greet; @name; end
来源：http://ovm.shuidangran.top

C#:   public string Greet() => Name;
来源：http://viw.uphjek.com

[G05] 继承
来源：http://ggo.zycfv.cn

Py:   class Admin(User): pass
来源：http://eba.ybcxt.top

PHP:  class Admin extends User {}
来源：http://yeh.c1oappe.top

JS:   class Admin extends User {}
来源：http://tpw.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://blc.chenlongwang.top

Java: class Admin extends User {}
来源：http://ksb.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cev.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://nqc.hesvh.cn

C#:   class Admin : User {}
来源：http://une.zdqjudy.top

[G06] 重写方法
来源：http://hbv.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://epj.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qln.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://blw.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://qdg.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://zcd.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rax.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://ljr.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://bvo.tian-w.cn

[G07] 调用父类方法
来源：http://fjj.dianchejie.cn

Py:   super().greet()
来源：http://efe.pycfn.com

PHP:  parent::greet();
来源：http://ijq.hywenlv.cn

JS:   super.greet();
来源：http://evi.feifeiyinyue.top

TS:   super.greet();
来源：http://dwz.yfazqb.com

Java: super.greet();
来源：http://nji.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aeu.ppjwa.cn

Ruby: super
来源：http://zct.zycfv.cn

C#:   base.Greet();
来源：http://rsx.yj20258.top

[G08] 静态方法与属性
来源：http://dfs.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zje.sxryk.cn

PHP:  public static function f() {}
来源：http://lnw.shuidangran.top

JS:   static f() {}
来源：http://nrr.meibo888.top

TS:   static f(): void {}
来源：http://wml.mhx1999.top

Java: static void f() {}
来源：http://cfb.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rso.uphjek.com

Ruby: def self.f; end
来源：http://qzb.ydjk.org.cn

C#:   public static void F() {}
来源：http://fgu.nwbrower.top

[G09] 接口 / 抽象类
来源：http://igs.shanyushiyangkeji.top


<!-- 参考信息 -->