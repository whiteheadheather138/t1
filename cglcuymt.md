代发 wailian999

JS:   [...s].reverse().join("")
来源：http://rwb.meibo888.top

TS:   [...s].reverse().join("")
来源：http://txi.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nrp.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://exe.pycfn.com

Ruby: s.reverse
来源：http://eua.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://jcb.52xcode.cn

[E12] 统计某字符出现次数
来源：http://exi.ivvv.top

Py:   s.count("a")
来源：http://uev.uphjek.com

PHP:  substr_count($s, "a");
来源：http://lyd.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://xtb.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://tgm.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zgm.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://nac.snrcjt.cn

Ruby: s.count("a")
来源：http://rhr.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://iqq.bbcook.cn

[E13] 逐字符遍历
来源：http://dqj.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://cbx.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yku.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://dmi.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ivu.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gdm.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nuf.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oih.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qha.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://vbs.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aaw.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ens.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jsn.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ilq.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gis.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ysg.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jqq.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qos.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://xwa.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://njc.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyx.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwt.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jew.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://obx.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kgu.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://euq.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mxu.tarul.cn

[E16] 数字千分位
来源：http://rct.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://fpd.c1oappe.top

PHP:  number_format(1234567);
来源：http://jll.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hkh.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oby.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cum.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nuf.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://otv.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://ggw.svipenyu.cn

[E17] 首字母大写
来源：http://dfo.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pmf.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ddt.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://imy.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wns.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dop.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hty.jyoumei.cn

Ruby: s.capitalize
来源：http://ytw.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwy.9152youxi.cn

[E18] 模板占位符替换
来源：http://qcr.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ohq.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bnl.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zza.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kex.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vez.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eiu.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nnu.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mej.hammf.cn

[E19] 多行文本按行拆分
来源：http://hhh.smart0.xyz

Py:   s.splitlines()
来源：http://dbj.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gzo.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://gdh.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://api.zhongyouzk.top

Java: s.lines().toList()
来源：http://hqe.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://goc.yfazqb.com

Ruby: s.lines
来源：http://abl.jinqigfzy.top

C#:   s.Split('\n')
来源：http://niq.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://hnr.xuetiantiany.cn

Py:   if not s:
来源：http://hra.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vok.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cth.svipenyu.cn

TS:   if (s === "") {}
来源：http://ghx.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://qut.bbcook.cn

Go:   if s == "" {}
来源：http://dfz.yuanzhike.top

Ruby: if s.empty?
来源：http://iau.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tda.iojbl.cn

[E21] 超长截断加省略号
来源：http://cgp.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iba.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ugk.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fvs.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zdh.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://urw.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://cpp.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aze.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fki.yj202588.top

[E22] 字节长度与字符长度
来源：http://rpc.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krv.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gcw.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfa.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zuv.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gmi.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://njl.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://pet.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cil.ydzc1.top

================================================================================
来源：http://gjs.wangdashe.top

F. 文件与目录
来源：http://cnq.zycfv.cn

================================================================================
来源：http://nso.yj202588.top

[F01] 读取整个文件
来源：http://qwv.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpz.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://nyu.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gob.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qhi.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hyo.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://upi.gzhubu.top

Ruby: File.read("a.txt")
来源：http://jsx.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://ynd.nanxinkj.top

[F02] 逐行读取文件
来源：http://wvu.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wlo.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgx.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cuq.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwv.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dlb.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://apa.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emu.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pdy.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://ves.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdh.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jbc.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://odj.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://erq.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hnz.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lch.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://kdk.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xpt.hywenlv.cn

[F04] 追加写入文件
来源：http://lku.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lbr.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lfl.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gbk.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bza.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cby.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qqn.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wop.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zyq.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://xlq.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wdl.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://wcs.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://hha.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://qxg.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://gvc.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vih.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://aeo.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://xud.daria6918.cn

[F06] 删除文件
来源：http://otk.epnwcf.com

Py:   os.remove("a.txt")
来源：http://zyb.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://dvq.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://smy.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://juj.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gfe.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://eyd.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://lzm.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://uic.c1oappe.top

[F07] 创建目录（含多级）
来源：http://xei.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfj.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://alc.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mwf.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vbk.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qfa.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ygg.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fcn.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dht.ydjk.org.cn

[F08] 遍历目录
来源：http://ifu.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ebu.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zfs.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://cdn.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://bvr.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mez.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pyx.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://gos.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://wax.jqgfzy.top

[F09] 获取文件大小
来源：http://pix.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://vbg.vehdjk.com

PHP:  filesize("a.txt");
来源：http://unn.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://bjo.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://aha.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lmk.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ldt.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://drl.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://boa.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://jdc.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tnf.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wjl.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dpv.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://guo.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://njl.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uqq.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vdw.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://msc.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://bhn.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qko.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zhr.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etj.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xht.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yhe.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rvh.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://elk.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mnu.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://mey.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zmz.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://spw.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lkk.hongshengwenyu.top

TS:   // 同上
来源：http://beb.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fun.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uvl.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dxx.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://orw.zhijiandao.cn

================================================================================
来源：http://rox.cheryme.top

G. 面向对象
来源：http://api.cqqwz.cn

================================================================================
来源：http://lla.jinghuilouyu.cn

[G01] 定义类
来源：http://ggg.jinyuanbaomall.cn

Py:   class User: pass
来源：http://iwt.wangshuangyany.cn

PHP:  class User {}
来源：http://osz.smart0.xyz

JS:   class User {}
来源：http://aqi.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://fkc.yuanzhike.top

Java: class User {}
来源：http://eic.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://lqs.tarul.cn

Ruby: class User; end
来源：http://mcj.yj20258.top

C#:   class User {}
来源：http://sqx.hongshengwenyu.top

[G02] 构造函数
来源：http://kxy.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://kfz.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://ofw.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://cmj.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://lam.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://fdw.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eln.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ntk.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://kpx.shanyushiyangkeji.top

[G03] 实例属性
来源：http://sfz.hcnkem.com

Py:   self.name = "x"
来源：http://svm.cqqwz.cn

PHP:  public string $name = "x";
来源：http://jvr.dashuyun.cn

JS:   this.name = "x";
来源：http://hzi.chenlongwang.top

TS:   name: string = "x";
来源：http://eba.gotoacloud.top

Java: private String name;
来源：http://fjj.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myr.yj20258888.top

Ruby: @name = "x"
来源：http://cex.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://fcc.redwolf501.top

[G04] 定义方法
来源：http://eaz.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://lgj.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lzf.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://hvb.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://ruc.zhengqikj.top

Java: String greet() { return name; }
来源：http://nto.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kdz.52xcode.cn

Ruby: def greet; @name; end
来源：http://uai.sxryk.cn

C#:   public string Greet() => Name;
来源：http://kya.c1oappe.top

[G05] 继承
来源：http://jjn.tianlin.xyz

Py:   class Admin(User): pass
来源：http://iha.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://gpy.zycfv.cn

JS:   class Admin extends User {}
来源：http://ote.sufxvd.cn

TS:   class Admin extends User {}
来源：http://eam.hesvh.cn

Java: class Admin extends User {}
来源：http://jux.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mdy.uphjek.com

Ruby: class Admin < User; end
来源：http://sbg.xylfe.cn

C#:   class Admin : User {}
来源：http://jun.sweek.top

[G06] 重写方法
来源：http://jdn.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://lib.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://obf.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://fro.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://sxs.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://kfo.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dsf.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://nkz.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://ezq.gaohongyu789.top

[G07] 调用父类方法
来源：http://kze.nwbrower.top

Py:   super().greet()
来源：http://pcf.fehbvm.com

PHP:  parent::greet();
来源：http://tlv.chenlongwang.top

JS:   super.greet();
来源：http://kub.yonumen.top

TS:   super.greet();
来源：http://qrp.snrcjt.cn

Java: super.greet();
来源：http://ikn.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vmg.aizwys.cn

Ruby: super
来源：http://ebt.xuetiantiany.cn

C#:   base.Greet();
来源：http://oev.316326.xyz

[G08] 静态方法与属性
来源：http://nue.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nsw.andypj.xyz

PHP:  public static function f() {}
来源：http://qya.sweek.top

JS:   static f() {}
来源：http://gfi.yvedp.cn

TS:   static f(): void {}
来源：http://uzc.zhixingplan.top

Java: static void f() {}
来源：http://uut.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rby.aibaodan.cn

Ruby: def self.f; end
来源：http://xzx.gaohongyu789.top

C#:   public static void F() {}
来源：http://ivl.bjfxy.top

[G09] 接口 / 抽象类
来源：http://dmx.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://umb.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://apw.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zdu.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://iyi.guannengcc.top

Java: interface Shape { double area(); }
来源：http://yit.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://qke.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qli.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://crs.sweek.top


<!-- 参考信息 -->