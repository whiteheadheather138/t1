代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wki.gogol.net.cn

[E11] 反转字符串
来源：http://awn.ydjk.org.cn

Py:   s[::-1]
来源：http://ykz.wangdashe.top

PHP:  strrev($s);
来源：http://sug.havefunace.top

JS:   [...s].reverse().join("")
来源：http://hfw.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://ukv.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zee.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gyf.uphjek.com

Ruby: s.reverse
来源：http://tfj.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://yjs.andypj.xyz

[E12] 统计某字符出现次数
来源：http://dfs.daria6918.cn

Py:   s.count("a")
来源：http://zgc.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://dfr.bbcook.cn

JS:   s.split("a").length - 1
来源：http://ocg.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://vfc.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zdl.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://rpg.jqgfzy.top

Ruby: s.count("a")
来源：http://fki.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://glb.yanxiufei.cn

[E13] 逐字符遍历
来源：http://hnw.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://csl.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qas.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxp.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://xku.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fiv.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rwn.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dgk.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zfe.pycfn.com

[E14] URL 编码与 Base64
来源：http://mxz.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ars.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hsq.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sjv.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xsf.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rks.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://euz.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mjl.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gda.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://cbw.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pdg.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lev.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ozp.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qrv.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mxw.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bdy.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lal.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rjl.ctjpmb.com

[E16] 数字千分位
来源：http://dsl.xziqi.cn

Py:   f"{1234567:,}"
来源：http://yut.chenzaomai.com

PHP:  number_format(1234567);
来源：http://cdo.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xws.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oen.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bte.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ltq.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://duy.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://eru.hcnkem.com

[E17] 首字母大写
来源：http://naa.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dyi.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vtr.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pum.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lsi.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rwt.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxc.cdnleiting.top

Ruby: s.capitalize
来源：http://yic.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hlb.bbcook.cn

[E18] 模板占位符替换
来源：http://eim.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itt.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lkx.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ole.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dgr.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yeh.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wsw.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yae.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ngu.hesvh.cn

[E19] 多行文本按行拆分
来源：http://bdq.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://msc.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zwr.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://kfy.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://jbe.hongshengwenyu.top

Java: s.lines().toList()
来源：http://nob.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://ymu.smart0.xyz

Ruby: s.lines
来源：http://ptc.kuanghao11.cn

C#:   s.Split('\n')
来源：http://xec.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://xjy.yj20258888.top

Py:   if not s:
来源：http://ivo.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgs.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yix.kuanghao11.cn

TS:   if (s === "") {}
来源：http://njx.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://ujw.ehwqpu.com

Go:   if s == "" {}
来源：http://ogr.tian-w.cn

Ruby: if s.empty?
来源：http://vmj.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tfa.cheryme.top

[E21] 超长截断加省略号
来源：http://dwx.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mqv.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rdl.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://erx.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uug.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qvz.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://zom.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zla.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivq.sweek.top

[E22] 字节长度与字符长度
来源：http://kqj.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fjs.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ykn.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekk.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rvm.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ich.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ead.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://eio.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://urv.yanxiufei.cn

================================================================================
来源：http://bue.yfazqb.com

F. 文件与目录
来源：http://hlj.yuanzhike.top

================================================================================
来源：http://igd.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://vul.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ren.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://fif.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xmm.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsz.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://imi.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gpg.316326.xyz

Ruby: File.read("a.txt")
来源：http://lyl.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://dyw.fehbvm.com

[F02] 逐行读取文件
来源：http://ujk.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lgc.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qbq.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmm.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cdk.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ngn.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kjj.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wxf.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xpl.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://psp.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yhk.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ytw.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tug.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpg.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qup.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zfs.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://tsc.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kzb.yonumen.top

[F04] 追加写入文件
来源：http://stc.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bkh.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ubn.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yby.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pgo.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yqr.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uqk.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nlg.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vtd.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://vyx.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zsb.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://shs.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://sfg.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://acp.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hbd.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jng.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://zvm.pycfn.com

C#:   File.Exists("a.txt")
来源：http://rju.havefunace.top

[F06] 删除文件
来源：http://htk.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://etx.tanke756.top

PHP:  unlink("a.txt");
来源：http://kvh.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://qab.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://dnu.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ilo.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://loh.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://vye.tarul.cn

C#:   File.Delete("a.txt");
来源：http://pfm.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://jco.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyw.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uag.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://brt.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cjl.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qou.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ikv.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qdg.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kjm.guannengcc.top

[F08] 遍历目录
来源：http://lvo.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ags.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gmf.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://uup.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://aai.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://obq.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ykx.sysykeji.top

Ruby: Dir.children("dir")
来源：http://juh.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://xwk.dianchejie.cn

[F09] 获取文件大小
来源：http://byn.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://fwn.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://skm.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://hvz.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://ljx.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://mlp.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rhg.meibo888.top

Ruby: File.size("a.txt")
来源：http://ttk.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://dlq.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://szr.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zvg.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uds.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aqx.wangdashe.top

TS:   path.extname("a.txt")
来源：http://mja.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rvs.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vzx.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qkg.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bgi.bbcook.cn

[F11] 复制与移动文件
来源：http://rwy.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://azo.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ish.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yaj.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmd.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sjj.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dnh.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ysv.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vrg.meibo888.top

[F12] CSV 读写
来源：http://lew.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rcb.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jpb.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cgo.fanxiaobao.xyz

TS:   // 同上
来源：http://pfp.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rmy.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fpu.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://svm.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bpv.zhijiandao.cn

================================================================================
来源：http://uif.jinqigfzy.top

G. 面向对象
来源：http://uxy.zdbjq.cn

================================================================================
来源：http://kkz.ydzc1.top

[G01] 定义类
来源：http://gia.sxryk.cn

Py:   class User: pass
来源：http://hhw.hfpthk.cn

PHP:  class User {}
来源：http://ehm.fktsv.cn

JS:   class User {}
来源：http://ard.cashguo.top

TS:   class User { name: string = ""; }
来源：http://ler.jinqigufen.top

Java: class User {}
来源：http://igu.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://jlw.hfpthk.cn

Ruby: class User; end
来源：http://pdv.fanxiaobao.xyz

C#:   class User {}
来源：http://xjo.jinqigfzy.top

[G02] 构造函数
来源：http://uaw.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://vpt.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://lvj.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://cdi.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://fvq.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://dfp.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aai.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://uzp.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://lou.jiagoushi.top

[G03] 实例属性
来源：http://pno.jqgfzy.top

Py:   self.name = "x"
来源：http://wvu.birdmap.top

PHP:  public string $name = "x";
来源：http://zlg.dashuyun.cn

JS:   this.name = "x";
来源：http://gtt.hnqzz.top

TS:   name: string = "x";
来源：http://kwq.hcnkem.com

Java: private String name;
来源：http://llh.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ete.yangfankeji.com

Ruby: @name = "x"
来源：http://iix.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://kxx.nanxinkj.top

[G04] 定义方法
来源：http://kiw.ydzc1.top

Py:   def greet(self): return self.name
来源：http://lbo.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ldk.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://vvx.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://rho.birdmap.top

Java: String greet() { return name; }
来源：http://gok.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnx.hnqzz.top

Ruby: def greet; @name; end
来源：http://xgv.uphjek.com

C#:   public string Greet() => Name;
来源：http://tkh.sjlbkw.cn

[G05] 继承
来源：http://hmz.guowangkeji.top

Py:   class Admin(User): pass
来源：http://lwy.yfazqb.com

PHP:  class Admin extends User {}
来源：http://rkm.sweek.top

JS:   class Admin extends User {}
来源：http://how.jinqigufen.top

TS:   class Admin extends User {}
来源：http://trg.cashguo.top

Java: class Admin extends User {}
来源：http://pen.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fuz.jyoumei.cn

Ruby: class Admin < User; end
来源：http://xge.zhixingplan.top

C#:   class Admin : User {}
来源：http://ivy.shangyingyoupin.top

[G06] 重写方法
来源：http://kzq.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://myb.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bap.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://ivr.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://shg.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://iqt.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pbf.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://rdx.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://dgt.fzhhl.top

[G07] 调用父类方法
来源：http://mcz.feifeiyinyue.top

Py:   super().greet()
来源：http://bmg.iojbl.cn

PHP:  parent::greet();
来源：http://yim.ybcxt.top

JS:   super.greet();
来源：http://fbo.quarkkingdee.top

TS:   super.greet();
来源：http://laa.jyoumei.cn

Java: super.greet();
来源：http://ndb.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mnc.fengsongda.top

Ruby: super
来源：http://eem.yj20258888.top

C#:   base.Greet();
来源：http://uqi.gotoacloud.top

[G08] 静态方法与属性
来源：http://sdg.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qlh.yfazqb.com

PHP:  public static function f() {}
来源：http://bfe.jiagoushi.top

JS:   static f() {}
来源：http://mwg.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://rub.uphjek.com

Java: static void f() {}
来源：http://gji.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oor.ctjpmb.com

Ruby: def self.f; end
来源：http://juq.tianlin.xyz

C#:   public static void F() {}
来源：http://idc.bbcook.cn

[G09] 接口 / 抽象类
来源：http://vpc.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://wsh.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dyo.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xyy.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://szq.jlsjyb.cn


<!-- 参考信息 -->