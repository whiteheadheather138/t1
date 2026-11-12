代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://jpf.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://rmx.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://szi.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pjf.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ewk.jinqigufen.top

[E11] 反转字符串
来源：http://uvh.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://shb.c1oappe.top

PHP:  strrev($s);
来源：http://fan.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://vwk.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://uqf.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tbp.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mto.snrcjt.cn

Ruby: s.reverse
来源：http://avy.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://cmq.ybcxt.top

[E12] 统计某字符出现次数
来源：http://tfe.wangdashe.top

Py:   s.count("a")
来源：http://ysm.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://eia.yvedp.cn

JS:   s.split("a").length - 1
来源：http://ygx.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://haj.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nuc.yonumen.top

Go:   strings.Count(s, "a")
来源：http://zku.jqgfzy.top

Ruby: s.count("a")
来源：http://dxi.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://gzd.yj20258888.top

[E13] 逐字符遍历
来源：http://ljz.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://ybd.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zct.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wlf.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jtu.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aaq.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oyj.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hgj.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lmt.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://mti.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tgj.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zvp.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://msm.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cqr.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uuf.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hjq.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tle.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://akj.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://dzh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gdl.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ove.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aec.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vfw.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fyc.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://twx.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nqw.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hhd.9152youxi.cn

[E16] 数字千分位
来源：http://bni.wangdashe.top

Py:   f"{1234567:,}"
来源：http://wol.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://cnb.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hyz.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ozl.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mgc.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://egl.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dke.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://wtv.daria6918.cn

[E17] 首字母大写
来源：http://weu.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hcy.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bvx.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fpb.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwq.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qpc.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yzg.iojbl.cn

Ruby: s.capitalize
来源：http://oxw.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ozc.sufxvd.cn

[E18] 模板占位符替换
来源：http://jrm.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rpb.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gqv.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gby.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://xvx.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dyw.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ezy.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gyo.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jru.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://ora.xuanzx.com

Py:   s.splitlines()
来源：http://prs.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vaj.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://tqi.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://yrp.hcnkem.com

Java: s.lines().toList()
来源：http://wiu.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://xgz.chenlongwang.top

Ruby: s.lines
来源：http://gqg.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://lbm.fktsv.cn

[E20] 判断字符串是否为空
来源：http://mvl.jinyuanbaomall.cn

Py:   if not s:
来源：http://xfa.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lsg.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cxl.xuanzx.com

TS:   if (s === "") {}
来源：http://rqa.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://dpu.shuidangran.top

Go:   if s == "" {}
来源：http://kkr.tarul.cn

Ruby: if s.empty?
来源：http://vxb.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://djz.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://jpi.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bmx.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://htz.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qlz.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oue.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qkq.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://wgs.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://chn.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rbv.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://ujg.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayg.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pyv.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvv.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbt.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yfn.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://znh.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://wsa.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bsg.xingfuxueyuan.xyz

================================================================================
来源：http://gox.sjlbkw.cn

F. 文件与目录
来源：http://ujv.zdqjudy.top

================================================================================
来源：http://loo.chenlongwang.top

[F01] 读取整个文件
来源：http://okb.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lss.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://oej.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ray.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ile.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vgo.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zpo.zycfv.cn

Ruby: File.read("a.txt")
来源：http://nan.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://yma.9152youxi.cn

[F02] 逐行读取文件
来源：http://oeb.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cbu.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jzi.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxc.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vir.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eta.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kaw.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lik.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dwh.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://jgn.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aog.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://scm.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bzr.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahu.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ppj.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cfo.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://nbe.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jju.hysaishi.cn

[F04] 追加写入文件
来源：http://afv.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ibj.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vvg.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbp.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tiq.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://atl.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xla.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tom.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lkr.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://gga.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vea.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://cys.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://bjf.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://vnb.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rlx.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ygj.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://rdy.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://uay.zdqjudy.top

[F06] 删除文件
来源：http://joq.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://ekt.ybcxt.top

PHP:  unlink("a.txt");
来源：http://isu.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://car.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://iru.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ltx.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://qnp.hysaishi.cn

Ruby: File.delete("a.txt")
来源：http://jqp.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://zus.ivvv.top

[F07] 创建目录（含多级）
来源：http://mwo.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://byb.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fku.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tdr.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmy.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hch.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zbo.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xje.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pim.guowangkeji.top

[F08] 遍历目录
来源：http://aaz.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://qcx.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oob.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://idp.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://jle.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ynj.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pre.xinyue.icu

Ruby: Dir.children("dir")
来源：http://bqf.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://jse.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://jic.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://lpp.cheryme.top

PHP:  filesize("a.txt");
来源：http://iul.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://gnw.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://nyk.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://bxo.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://urp.yj202588.top

Ruby: File.size("a.txt")
来源：http://eyc.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://fdp.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://sew.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hzw.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ios.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yyw.bbcook.cn

TS:   path.extname("a.txt")
来源：http://lzu.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wui.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whi.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tih.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nvq.gotoacloud.top

[F11] 复制与移动文件
来源：http://tsw.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://thg.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pyh.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://biz.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frh.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pcx.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvk.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://htn.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://src.yueranfly.top

[F12] CSV 读写
来源：http://eow.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmb.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jkk.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://epw.hesvh.cn

TS:   // 同上
来源：http://com.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iap.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wnn.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rxd.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://eql.zycfv.cn

================================================================================
来源：http://oed.cheryme.top

G. 面向对象
来源：http://don.xingfuxueyuan.xyz

================================================================================
来源：http://wbe.sjlbkw.cn

[G01] 定义类
来源：http://fbp.ywan-chungtsiang.top

Py:   class User: pass
来源：http://ueq.aizwys.cn

PHP:  class User {}
来源：http://kmd.mhx1999.top

JS:   class User {}
来源：http://cfw.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://rsu.hongshengwenyu.top

Java: class User {}
来源：http://tfa.aibaodan.cn

Go:   type User struct { Name string }
来源：http://gid.nanxuanxn.top

Ruby: class User; end
来源：http://hjv.cdnleiting.top

C#:   class User {}
来源：http://luw.shzxlz.cn

[G02] 构造函数
来源：http://uld.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://pdw.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ycr.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://oip.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://bfi.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://ctg.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ouh.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://eyx.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://wsy.wangshuangyany.cn

[G03] 实例属性
来源：http://xst.shuidangran.top

Py:   self.name = "x"
来源：http://tor.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://wbo.nanxuanxn.top

JS:   this.name = "x";
来源：http://hnq.guowangkeji.top

TS:   name: string = "x";
来源：http://xem.nanxinkj.top

Java: private String name;
来源：http://opf.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwy.mhx1999.top

Ruby: @name = "x"
来源：http://rae.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ggn.zdbjq.cn

[G04] 定义方法
来源：http://tlc.nwbrower.top

Py:   def greet(self): return self.name
来源：http://zlw.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qzz.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://wwx.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://jqz.jianghu66.top

Java: String greet() { return name; }
来源：http://mmc.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tvp.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://rve.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://rtk.yj202588.top

[G05] 继承
来源：http://oxs.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://exy.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://fkl.yj20258888.top

JS:   class Admin extends User {}
来源：http://lvw.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://tzj.yfazqb.com

Java: class Admin extends User {}
来源：http://yrd.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tfq.sxryk.cn

Ruby: class Admin < User; end
来源：http://cwl.tanke756.top

C#:   class Admin : User {}
来源：http://wol.zhongyouzk.top

[G06] 重写方法
来源：http://iyj.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://rtl.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jua.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://yol.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://fij.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://ocb.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://njy.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://ztu.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://kbz.ehwqpu.com

[G07] 调用父类方法
来源：http://yfe.aibaodan.cn

Py:   super().greet()
来源：http://nth.yueranfly.top

PHP:  parent::greet();
来源：http://lin.jlsjyb.cn

JS:   super.greet();
来源：http://coz.chenjidiqi.icu

TS:   super.greet();
来源：http://zhz.zhijiandao.cn

Java: super.greet();
来源：http://pql.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uww.tianlin.xyz

Ruby: super
来源：http://nhp.hnxiangtu.top

C#:   base.Greet();
来源：http://qaa.yj202588.top

[G08] 静态方法与属性
来源：http://cvi.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwh.daxiang520.top

PHP:  public static function f() {}
来源：http://ngl.sxryk.cn

JS:   static f() {}
来源：http://ntw.andypj.xyz

TS:   static f(): void {}
来源：http://bej.dashuyun.cn

Java: static void f() {}
来源：http://vdg.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wez.smart0.xyz

Ruby: def self.f; end
来源：http://twv.tianlin.xyz

C#:   public static void F() {}
来源：http://xjk.yvedp.cn

[G09] 接口 / 抽象类
来源：http://zcx.smart0.xyz


<!-- 参考信息 -->