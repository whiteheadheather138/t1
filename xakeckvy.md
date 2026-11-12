代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ogz.cashguo.top

Java: String.format("%03d", 7)
来源：http://wei.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rfw.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oog.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uio.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://ces.iojbl.cn

Py:   s[::-1]
来源：http://dwc.sxryk.cn

PHP:  strrev($s);
来源：http://gzm.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://utg.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://snp.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pny.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yib.iojbl.cn

Ruby: s.reverse
来源：http://llx.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://ooj.sysykeji.top

[E12] 统计某字符出现次数
来源：http://puo.ydjk.org.cn

Py:   s.count("a")
来源：http://aqk.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://rcc.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://cbe.hesvh.cn

TS:   s.split("a").length - 1
来源：http://qsp.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fvy.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://gxf.shangyingyoupin.top

Ruby: s.count("a")
来源：http://azd.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://nhj.zdbjq.cn

[E13] 逐字符遍历
来源：http://kqx.uphjek.com

Py:   for ch in s: print(ch)
来源：http://etq.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://owo.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://icw.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://isl.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lvs.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zbp.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ofe.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://luj.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ldk.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fuf.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oar.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eql.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mjc.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wzs.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tzt.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hgg.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cjx.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://jhg.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nwv.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fyp.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uxx.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nep.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rah.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nfx.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zpa.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cbm.jinqigfzy.top

[E16] 数字千分位
来源：http://lcp.ybcxt.top

Py:   f"{1234567:,}"
来源：http://lpr.smart0.xyz

PHP:  number_format(1234567);
来源：http://scn.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bza.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xpd.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xqx.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gmx.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tdv.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://ruh.9152youxi.cn

[E17] 首字母大写
来源：http://qyb.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eov.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dzq.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pez.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajp.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rmy.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mwy.yj202588.top

Ruby: s.capitalize
来源：http://jpv.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdk.vqdsnc.cn

[E18] 模板占位符替换
来源：http://qpq.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nok.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sec.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yzf.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wnp.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://veo.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kuj.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qjs.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wem.xylfe.cn

[E19] 多行文本按行拆分
来源：http://vms.smart0.xyz

Py:   s.splitlines()
来源：http://skc.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kmv.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://wpd.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://pwg.smart0.xyz

Java: s.lines().toList()
来源：http://sax.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://fdx.xuanzx.com

Ruby: s.lines
来源：http://zam.daxiang520.top

C#:   s.Split('\n')
来源：http://iik.vehdjk.com

[E20] 判断字符串是否为空
来源：http://cjy.gogol.net.cn

Py:   if not s:
来源：http://xmz.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sxy.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xfi.cheryme.top

TS:   if (s === "") {}
来源：http://wes.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://cwt.jlsjyb.cn

Go:   if s == "" {}
来源：http://mpk.zhixingplan.top

Ruby: if s.empty?
来源：http://zls.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lkh.aibaodan.cn

[E21] 超长截断加省略号
来源：http://kwg.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ufj.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iwl.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eea.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztm.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yzn.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://mlv.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tkf.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pfs.aizwys.cn

[E22] 字节长度与字符长度
来源：http://wrs.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qqq.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rbd.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://suu.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://axr.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://awu.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ioi.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://wcb.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lhu.0kj1m.cn

================================================================================
来源：http://jst.316326.xyz

F. 文件与目录
来源：http://pqr.tian-w.cn

================================================================================
来源：http://rlh.redwolf501.top

[F01] 读取整个文件
来源：http://jrp.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bpi.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://ins.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wyx.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nzv.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cyx.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bog.andypj.xyz

Ruby: File.read("a.txt")
来源：http://qql.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://dtq.cheryme.top

[F02] 逐行读取文件
来源：http://rkz.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qzb.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qgc.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cyv.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rnb.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qgr.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mxd.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hwf.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xld.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://sdf.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xgh.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kpe.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gve.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tcx.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kxe.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jbh.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://nrp.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hzc.yuanzhike.top

[F04] 追加写入文件
来源：http://ded.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kls.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ork.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxa.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://viy.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://khs.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xom.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jek.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lyv.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://wms.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ekh.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://imj.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://kpq.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://oza.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bgg.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bhe.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://xis.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://ynw.yueranfly.top

[F06] 删除文件
来源：http://bhp.yfazqb.com

Py:   os.remove("a.txt")
来源：http://xpz.yuxming.cn

PHP:  unlink("a.txt");
来源：http://wvp.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pwa.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://zwv.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://get.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://iqu.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://xwc.sweek.top

C#:   File.Delete("a.txt");
来源：http://yfp.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://sva.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zty.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xge.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxh.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myi.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://azc.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ugn.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yuo.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tav.feifeiyinyue.top

[F08] 遍历目录
来源：http://tdk.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://bte.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rjg.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://cpp.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://gbp.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://deb.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://dwn.yfazqb.com

Ruby: Dir.children("dir")
来源：http://bhg.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://tqd.tarul.cn

[F09] 获取文件大小
来源：http://ago.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://mxh.yueranfly.top

PHP:  filesize("a.txt");
来源：http://rfs.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://lce.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://cib.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vhm.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kkl.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://ecz.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://izi.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://rle.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oym.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cmo.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rlw.yj20258.top

TS:   path.extname("a.txt")
来源：http://dgs.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qlz.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bzn.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vym.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zhz.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://rbk.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fxb.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iih.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://anj.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dha.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rmo.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvr.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://irg.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fgz.wangshuangyany.cn

[F12] CSV 读写
来源：http://aiw.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zaz.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://szf.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tzu.snrcjt.cn

TS:   // 同上
来源：http://hnf.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hww.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fqo.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oaj.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ftr.andypj.xyz

================================================================================
来源：http://hme.9152youxi.cn

G. 面向对象
来源：http://xcb.yj20258888.top

================================================================================
来源：http://idk.cheryme.top

[G01] 定义类
来源：http://uwz.jqgfzy.top

Py:   class User: pass
来源：http://det.jinqigufen.top

PHP:  class User {}
来源：http://klh.yj20258.top

JS:   class User {}
来源：http://kdx.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://akf.kuanghao11.cn

Java: class User {}
来源：http://mzr.0kj1m.cn

Go:   type User struct { Name string }
来源：http://baj.cashguo.top

Ruby: class User; end
来源：http://nmw.xinyue.icu

C#:   class User {}
来源：http://xou.ybcxt.top

[G02] 构造函数
来源：http://nku.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://fem.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://bng.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://gjg.sweek.top

TS:   constructor(public name: string) {}
来源：http://sxa.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://nmk.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ahj.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://wny.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://ren.fanxiaobao.xyz

[G03] 实例属性
来源：http://cab.fengsongda.top

Py:   self.name = "x"
来源：http://coi.ivvv.top

PHP:  public string $name = "x";
来源：http://wba.hnxiangtu.top

JS:   this.name = "x";
来源：http://hji.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://eph.jyoumei.cn

Java: private String name;
来源：http://izd.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hfo.xuetiantiany.cn

Ruby: @name = "x"
来源：http://psd.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://lfz.zdbjq.cn

[G04] 定义方法
来源：http://eoa.gzhubu.top

Py:   def greet(self): return self.name
来源：http://nxk.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://pjn.redwolf501.top

JS:   greet() { return this.name; }
来源：http://xjh.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://pik.zdbjq.cn

Java: String greet() { return name; }
来源：http://oye.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nhu.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://yum.yongpay.top

C#:   public string Greet() => Name;
来源：http://wei.chenzaomai.com

[G05] 继承
来源：http://rry.ivvv.top

Py:   class Admin(User): pass
来源：http://ovn.hesvh.cn

PHP:  class Admin extends User {}
来源：http://nkw.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://mpv.hcnkem.com

TS:   class Admin extends User {}
来源：http://yop.zhijiandao.cn

Java: class Admin extends User {}
来源：http://onj.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tux.svipenyu.cn

Ruby: class Admin < User; end
来源：http://xta.xuanzx.com

C#:   class Admin : User {}
来源：http://ene.aibaodan.cn

[G06] 重写方法
来源：http://los.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://vkm.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yjc.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://zlx.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://ikd.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://eji.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vsc.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://lec.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://rob.sxryk.cn

[G07] 调用父类方法
来源：http://jev.dianchejie.cn

Py:   super().greet()
来源：http://rdz.zhengqikj.top

PHP:  parent::greet();
来源：http://cdl.zycfv.cn

JS:   super.greet();
来源：http://awp.ivvv.top

TS:   super.greet();
来源：http://qdw.dashuyun.cn

Java: super.greet();
来源：http://vex.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aub.bjfxy.top

Ruby: super
来源：http://xzx.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://zme.fehbvm.com

[G08] 静态方法与属性
来源：http://olt.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kcw.zycfv.cn

PHP:  public static function f() {}
来源：http://ntv.tanke756.top

JS:   static f() {}
来源：http://xwl.gzhubu.top

TS:   static f(): void {}
来源：http://nko.aizwys.cn

Java: static void f() {}
来源：http://exe.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rub.yonumen.top

Ruby: def self.f; end
来源：http://bvq.wangdashe.top

C#:   public static void F() {}
来源：http://mpq.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://tpv.sweek.top


<!-- 参考信息 -->