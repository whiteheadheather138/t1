代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://xtq.xziqi.cn

Java: String.format("%03d", 7)
来源：http://oox.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mbg.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zvh.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://trw.ppjwa.cn

[E11] 反转字符串
来源：http://kqk.uphjek.com

Py:   s[::-1]
来源：http://moa.jinqigufen.top

PHP:  strrev($s);
来源：http://whs.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://ada.sweek.top

TS:   [...s].reverse().join("")
来源：http://iio.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pfq.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://pmj.ydzc1.top

Ruby: s.reverse
来源：http://tgr.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://nnw.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://jqp.sxryk.cn

Py:   s.count("a")
来源：http://cgr.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://gtm.bbcook.cn

JS:   s.split("a").length - 1
来源：http://rdj.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://caz.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tdt.cashguo.top

Go:   strings.Count(s, "a")
来源：http://epl.haohaochexian.top

Ruby: s.count("a")
来源：http://ieo.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://jvv.smart0.xyz

[E13] 逐字符遍历
来源：http://rjc.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://gai.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vxx.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://upe.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://frb.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jaf.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lze.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vuo.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eol.hcnkem.com

[E14] URL 编码与 Base64
来源：http://kri.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mqh.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tjf.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ffx.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nse.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://spo.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://liz.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yst.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ibq.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://qoh.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wwk.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mns.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pys.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://xfy.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qzc.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xdp.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vfj.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://llj.shanyushiyangtech.top

[E16] 数字千分位
来源：http://dfg.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://lqj.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://osf.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hpy.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xwq.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eqz.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ets.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gvz.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://zby.yj20258888.top

[E17] 首字母大写
来源：http://zbm.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ayk.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://txt.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfv.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzb.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ioo.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hbe.hfpthk.cn

Ruby: s.capitalize
来源：http://ohf.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://huu.yongpay.top

[E18] 模板占位符替换
来源：http://xfz.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lgg.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rsi.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eae.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://apm.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vuw.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hwt.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xgy.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zet.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://per.daria6918.cn

Py:   s.splitlines()
来源：http://csf.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wpe.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://aet.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://ozs.wangshuangyany.cn

Java: s.lines().toList()
来源：http://nsh.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://qwr.uphjek.com

Ruby: s.lines
来源：http://yrb.tanke756.top

C#:   s.Split('\n')
来源：http://kfg.mhx1999.top

[E20] 判断字符串是否为空
来源：http://hpc.ctjpmb.com

Py:   if not s:
来源：http://ewm.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://liw.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xdz.yj202588.top

TS:   if (s === "") {}
来源：http://hwr.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://pez.hnqzz.top

Go:   if s == "" {}
来源：http://pgj.yj20258888.top

Ruby: if s.empty?
来源：http://epo.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://efr.yj20258.top

[E21] 超长截断加省略号
来源：http://jmb.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://djq.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cth.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://upa.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hjv.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vpi.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://cqz.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dav.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://neo.hammf.cn

[E22] 字节长度与字符长度
来源：http://rpq.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://prn.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qoi.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vwp.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zax.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://btt.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tyi.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://msl.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bce.hfpthk.cn

================================================================================
来源：http://sfn.yangfankeji.com

F. 文件与目录
来源：http://nkt.hnxiangtu.top

================================================================================
来源：http://kab.shuidangran.top

[F01] 读取整个文件
来源：http://cds.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dto.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://ius.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kgl.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zkg.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://coj.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fyi.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://ags.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://oiv.tanke756.top

[F02] 逐行读取文件
来源：http://qvq.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://otl.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eyj.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azh.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmv.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vgn.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://swl.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xaq.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vqk.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://bcb.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzr.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://udl.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mnn.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dsr.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xji.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hej.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://jjl.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gfd.xinyue.icu

[F04] 追加写入文件
来源：http://oyr.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iye.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rrt.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bou.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfw.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tuc.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://umg.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iot.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://slc.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://rld.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uui.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://fqa.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://pel.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://srx.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dot.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ahk.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://sqb.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://boj.zdqjudy.top

[F06] 删除文件
来源：http://qrl.smart0.xyz

Py:   os.remove("a.txt")
来源：http://azf.ybcxt.top

PHP:  unlink("a.txt");
来源：http://kmk.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jnk.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xzw.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vrx.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://ahx.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://lmz.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://jjg.epnwcf.com

[F07] 创建目录（含多级）
来源：http://msm.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wjh.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vmb.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zuh.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyj.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fha.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://evz.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://acg.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tan.xylfe.cn

[F08] 遍历目录
来源：http://bol.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qfc.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gaz.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://gxf.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://dbe.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://atd.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uuk.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://zge.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://wpb.jinqigufen.top

[F09] 获取文件大小
来源：http://xob.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://sen.jianghu66.top

PHP:  filesize("a.txt");
来源：http://qko.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://jqd.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://kdv.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://zpk.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tyt.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://syf.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://qli.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://tge.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uba.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://otf.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zvl.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://nwj.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://neb.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zxd.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjb.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gqj.redwolf501.top

[F11] 复制与移动文件
来源：http://djx.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mji.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tsv.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhc.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wph.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qmx.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rkp.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uzg.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ted.sysykeji.top

[F12] CSV 读写
来源：http://arm.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://phu.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsf.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qpb.epnwcf.com

TS:   // 同上
来源：http://zor.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ilv.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mzl.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yal.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wsk.jinqigfzy.top

================================================================================
来源：http://wld.wangdashe.top

G. 面向对象
来源：http://oqy.ivvv.top

================================================================================
来源：http://nbb.birdmap.top

[G01] 定义类
来源：http://kmx.tanke756.top

Py:   class User: pass
来源：http://wwk.xuanzx.com

PHP:  class User {}
来源：http://ecf.yj202588.top

JS:   class User {}
来源：http://gcm.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://jan.xuanzx.com

Java: class User {}
来源：http://eeb.jinqigufen.top

Go:   type User struct { Name string }
来源：http://rxd.birdmap.top

Ruby: class User; end
来源：http://mdj.hnxiangtu.top

C#:   class User {}
来源：http://mtv.xuetiantiany.cn

[G02] 构造函数
来源：http://yvr.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://woj.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://wpv.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://upb.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://vcr.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://ibo.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zfe.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://rox.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://edf.quarkkingdee.top

[G03] 实例属性
来源：http://jvx.vqdsnc.cn

Py:   self.name = "x"
来源：http://ivb.jinqigufen.top

PHP:  public string $name = "x";
来源：http://yfh.fktsv.cn

JS:   this.name = "x";
来源：http://boa.nanxinkj.top

TS:   name: string = "x";
来源：http://yac.hysaishi.cn

Java: private String name;
来源：http://mmb.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dwm.sysykeji.top

Ruby: @name = "x"
来源：http://orl.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://pzi.svipenyu.cn

[G04] 定义方法
来源：http://znr.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://sbj.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wui.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://cks.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://ibr.chenzaomai.com

Java: String greet() { return name; }
来源：http://mrs.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://cay.cheryme.top

Ruby: def greet; @name; end
来源：http://mie.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://kmb.9152youxi.cn

[G05] 继承
来源：http://pjg.ctjpmb.com

Py:   class Admin(User): pass
来源：http://nuk.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://yrk.aizwys.cn

JS:   class Admin extends User {}
来源：http://vcg.zhixingplan.top

TS:   class Admin extends User {}
来源：http://xnp.zycfv.cn

Java: class Admin extends User {}
来源：http://ikg.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tnt.shuidangran.top

Ruby: class Admin < User; end
来源：http://kkn.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://bxt.bbcook.cn

[G06] 重写方法
来源：http://sye.havefunace.top

Py:   def greet(self): return "admin"
来源：http://ebv.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kbw.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://gvj.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://dnv.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://xcf.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jhp.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://fko.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://dlf.pengpengdd.cyou

[G07] 调用父类方法
来源：http://rjq.fehbvm.com

Py:   super().greet()
来源：http://psp.yuxming.cn

PHP:  parent::greet();
来源：http://rdr.sufxvd.cn

JS:   super.greet();
来源：http://dwn.xuanzx.com

TS:   super.greet();
来源：http://brt.cheryme.top

Java: super.greet();
来源：http://zhe.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezu.wangshuangyany.cn

Ruby: super
来源：http://lel.epnwcf.com

C#:   base.Greet();
来源：http://yqz.ydzc1.top

[G08] 静态方法与属性
来源：http://vsx.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://urj.c1oappe.top

PHP:  public static function f() {}
来源：http://aul.hammf.cn

JS:   static f() {}
来源：http://rak.tarul.cn

TS:   static f(): void {}
来源：http://nxw.havefunace.top

Java: static void f() {}
来源：http://eru.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxn.sjlbkw.cn

Ruby: def self.f; end
来源：http://phs.ydzc1.top

C#:   public static void F() {}
来源：http://fek.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://dae.chenlongwang.top


<!-- 参考信息 -->