代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qon.ivvv.top

[E11] 反转字符串
来源：http://zti.feifeiyinyue.top

Py:   s[::-1]
来源：http://gdt.ydjk.org.cn

PHP:  strrev($s);
来源：http://tsb.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://mwc.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://son.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jvg.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dvv.nanxuanxn.top

Ruby: s.reverse
来源：http://dwx.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://szk.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://uwk.birdmap.top

Py:   s.count("a")
来源：http://ayr.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://ote.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://gii.yj20258888.top

TS:   s.split("a").length - 1
来源：http://fit.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fzw.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://vhu.shangyingyoupin.top

Ruby: s.count("a")
来源：http://twx.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://spg.ppjwa.cn

[E13] 逐字符遍历
来源：http://nty.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://ysz.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://imw.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oyk.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mjy.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fjc.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://emg.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gjm.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oha.yuxming.cn

[E14] URL 编码与 Base64
来源：http://dra.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wnw.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://phz.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://css.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wnx.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dln.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ohj.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ovs.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tev.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://mdx.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rpj.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gxk.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eeh.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kse.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qdr.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uga.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yvu.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://brx.sxryk.cn

[E16] 数字千分位
来源：http://iva.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://kri.sufxvd.cn

PHP:  number_format(1234567);
来源：http://iyt.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://iqk.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hcl.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ldp.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rsr.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fmg.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://hwi.jinqigufen.top

[E17] 首字母大写
来源：http://dnb.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://neu.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xan.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lij.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wdp.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rmg.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://noe.jlsjyb.cn

Ruby: s.capitalize
来源：http://cqv.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mpx.fzhhl.top

[E18] 模板占位符替换
来源：http://zam.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cpo.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fwp.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ydr.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://poa.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmo.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mro.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gqk.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jyg.hesvh.cn

[E19] 多行文本按行拆分
来源：http://ugp.epnwcf.com

Py:   s.splitlines()
来源：http://hwz.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swf.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://tdi.sweek.top

TS:   s.split(/\r?\n/)
来源：http://rab.jinqigfzy.top

Java: s.lines().toList()
来源：http://ygj.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://jql.gzhubu.top

Ruby: s.lines
来源：http://cke.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://ghw.hcnkem.com

[E20] 判断字符串是否为空
来源：http://nuw.nanxuanxn.top

Py:   if not s:
来源：http://qyj.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kqh.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nlv.sxryk.cn

TS:   if (s === "") {}
来源：http://ptj.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://dgu.ydzc1.top

Go:   if s == "" {}
来源：http://wnq.ivvv.top

Ruby: if s.empty?
来源：http://orl.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mvw.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://dpu.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nhm.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cga.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijr.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xia.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ewf.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://qhs.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qbb.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://drx.vehdjk.com

[E22] 字节长度与字符长度
来源：http://scl.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzt.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pfn.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://glj.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yob.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gst.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pqn.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://mza.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zxu.0kj1m.cn

================================================================================
来源：http://huf.jlsjyb.cn

F. 文件与目录
来源：http://uob.chenjidiqi.icu

================================================================================
来源：http://wuk.sjlbkw.cn

[F01] 读取整个文件
来源：http://zov.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://asg.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://soe.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ies.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbi.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bcb.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vil.sweek.top

Ruby: File.read("a.txt")
来源：http://weq.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://dob.dashuyun.cn

[F02] 逐行读取文件
来源：http://pel.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yrz.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tow.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vxe.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prj.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ojf.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lfv.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lkp.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sqj.meibo888.top

[F03] 写入文件（覆盖）
来源：http://gqb.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cds.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdf.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpl.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xsy.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dad.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wid.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://dcb.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tav.jlsjyb.cn

[F04] 追加写入文件
来源：http://atu.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://snm.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pqi.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gxj.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uax.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bnm.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ioy.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vkn.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqt.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://hzc.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvm.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://eao.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://nub.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://nxr.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://loi.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fsu.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://qcb.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://heo.yongpay.top

[F06] 删除文件
来源：http://jaw.sweek.top

Py:   os.remove("a.txt")
来源：http://ovt.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://zlj.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nfk.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://cdh.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yis.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://ujo.pycfn.com

Ruby: File.delete("a.txt")
来源：http://iji.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://cxi.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://tnh.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rix.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jqt.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkl.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gix.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://euw.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ket.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ulz.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hsf.ivvv.top

[F08] 遍历目录
来源：http://dnm.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fsd.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zra.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://rzw.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://lgt.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gjl.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dit.52xcode.cn

Ruby: Dir.children("dir")
来源：http://xtd.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://xok.hcnkem.com

[F09] 获取文件大小
来源：http://sdq.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://rso.iojbl.cn

PHP:  filesize("a.txt");
来源：http://jlj.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://lbc.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://ohy.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://frl.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efc.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://tem.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://wic.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://ybz.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qzo.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oyh.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://buv.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://ztv.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzr.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bwq.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zqo.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dbf.ydjk.org.cn

[F11] 复制与移动文件
来源：http://xpj.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tda.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://owg.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cig.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cah.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gpb.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmm.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://umu.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yhd.birdmap.top

[F12] CSV 读写
来源：http://rlt.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cyv.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://emq.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wtv.jinghuilouyu.cn

TS:   // 同上
来源：http://tds.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mvd.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://szv.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rpy.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uai.ivvv.top

================================================================================
来源：http://spv.fehbvm.com

G. 面向对象
来源：http://ibi.jianghu66.top

================================================================================
来源：http://cas.andypj.xyz

[G01] 定义类
来源：http://sja.fehbvm.com

Py:   class User: pass
来源：http://igf.tianlin.xyz

PHP:  class User {}
来源：http://xgn.uphjek.com

JS:   class User {}
来源：http://skl.yonumen.top

TS:   class User { name: string = ""; }
来源：http://nqx.yuanzhike.top

Java: class User {}
来源：http://saj.guowangkeji.top

Go:   type User struct { Name string }
来源：http://vlo.tarul.cn

Ruby: class User; end
来源：http://iyb.zhongyouzk.top

C#:   class User {}
来源：http://ogy.shanyushiyangkeji.top

[G02] 构造函数
来源：http://srz.ctjpmb.com

Py:   def __init__(self, name): self.name = name
来源：http://iqj.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://xfm.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://qzo.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://xjh.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://nds.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xyw.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://tje.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://mun.xinyue.icu

[G03] 实例属性
来源：http://trq.ydjk.org.cn

Py:   self.name = "x"
来源：http://tuj.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://nvn.yangfankeji.com

JS:   this.name = "x";
来源：http://ruw.vqdsnc.cn

TS:   name: string = "x";
来源：http://wad.birdmap.top

Java: private String name;
来源：http://tkk.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hhu.xinyue.icu

Ruby: @name = "x"
来源：http://vec.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://dvh.epnwcf.com

[G04] 定义方法
来源：http://myg.xylfe.cn

Py:   def greet(self): return self.name
来源：http://llx.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lgt.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://uns.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://qfa.vehdjk.com

Java: String greet() { return name; }
来源：http://use.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://yqm.meibo888.top

Ruby: def greet; @name; end
来源：http://mts.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://lsi.tian-w.cn

[G05] 继承
来源：http://bqh.yvedp.cn

Py:   class Admin(User): pass
来源：http://hze.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://raa.redwolf501.top

JS:   class Admin extends User {}
来源：http://pjo.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://ali.uphjek.com

Java: class Admin extends User {}
来源：http://qdw.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yge.jyoumei.cn

Ruby: class Admin < User; end
来源：http://ecv.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://jgc.zhaomingkeji.xyz

[G06] 重写方法
来源：http://bwp.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://ahw.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xai.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://rvp.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://ude.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://esr.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sii.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://vae.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://psg.yanxiufei.cn

[G07] 调用父类方法
来源：http://yax.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://cca.zhongyouzk.top

PHP:  parent::greet();
来源：http://uyr.hongshengwenyu.top

JS:   super.greet();
来源：http://wyt.fzhhl.top

TS:   super.greet();
来源：http://lgn.316326.xyz

Java: super.greet();
来源：http://zgs.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fla.zhijiandao.cn

Ruby: super
来源：http://tea.cdnleiting.top

C#:   base.Greet();
来源：http://gol.bjfxy.top

[G08] 静态方法与属性
来源：http://ktp.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vsq.sweek.top

PHP:  public static function f() {}
来源：http://evc.dashuyun.cn

JS:   static f() {}
来源：http://rjf.zhixingplan.top

TS:   static f(): void {}
来源：http://qyz.jqgufenzy.top

Java: static void f() {}
来源：http://bwj.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nem.tarul.cn

Ruby: def self.f; end
来源：http://vme.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://lib.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://zfx.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://woy.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://lsk.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://udp.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://pnx.shzxlz.cn


<!-- 参考信息 -->