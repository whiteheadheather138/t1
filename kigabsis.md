代发 wailian999

PHP:  substr_count($s, "a");
来源：http://zbc.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://vyy.epnwcf.com

TS:   s.split("a").length - 1
来源：http://hzl.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ior.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://vch.mhx1999.top

Ruby: s.count("a")
来源：http://yxc.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://qpf.sufxvd.cn

[E13] 逐字符遍历
来源：http://iwk.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://xcg.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gnc.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://gxy.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpt.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cej.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ayc.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://huk.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://frx.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://sgw.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qcf.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rxj.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pvx.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyt.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pao.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mrl.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lcy.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://llu.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://wob.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lvq.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tzm.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dei.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ert.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mzr.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zyc.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://weu.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ews.ivvv.top

[E16] 数字千分位
来源：http://sfh.hcnkem.com

Py:   f"{1234567:,}"
来源：http://zcp.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://nhl.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bjj.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gyw.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jgk.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ivj.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fpu.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://pbn.0kj1m.cn

[E17] 首字母大写
来源：http://ymo.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gdf.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://zud.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eiy.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcb.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ihj.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzh.quarkkingdee.top

Ruby: s.capitalize
来源：http://slb.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oso.jlsjyb.cn

[E18] 模板占位符替换
来源：http://gio.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hrd.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zap.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://wvp.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rbh.jinqigfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uiy.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrh.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cbl.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fxo.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://dno.tian-w.cn

Py:   s.splitlines()
来源：http://dbi.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hbv.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://xqh.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://nwh.iojbl.cn

Java: s.lines().toList()
来源：http://wne.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://wwm.pengpengdd.cyou

Ruby: s.lines
来源：http://grd.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://xbl.uphjek.com

[E20] 判断字符串是否为空
来源：http://xlq.meibo888.top

Py:   if not s:
来源：http://usv.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://skp.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ucb.zycfv.cn

TS:   if (s === "") {}
来源：http://xhh.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://bao.daxiang520.top

Go:   if s == "" {}
来源：http://fye.nanxuanxn.top

Ruby: if s.empty?
来源：http://pbb.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yvw.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://nlr.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agw.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zwi.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymh.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ojc.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hdz.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://mdn.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bca.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fft.bbcook.cn

[E22] 字节长度与字符长度
来源：http://skd.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gwa.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rem.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://por.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pcu.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://afq.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ehs.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://vig.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqt.xuanzx.com

================================================================================
来源：http://hbe.guowangkeji.top

F. 文件与目录
来源：http://lbk.zhongyouzk.top

================================================================================
来源：http://wik.zhiwuduotai.top

[F01] 读取整个文件
来源：http://lno.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fgh.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://qbn.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yvf.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ojl.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xyw.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://smx.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://pyl.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://zjh.xinyue.icu

[F02] 逐行读取文件
来源：http://nhs.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swk.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bto.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://are.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfd.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aki.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://exm.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxl.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sry.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://jjw.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kdg.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fop.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uft.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sqw.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mdv.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rck.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://jgg.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xjv.c1oappe.top

[F04] 追加写入文件
来源：http://kya.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wnx.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fir.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hvu.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://exe.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dtx.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fha.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ahr.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrl.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://kki.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://czp.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://phc.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://bpi.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://mig.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://mzu.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ehr.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://heb.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://pzj.birdmap.top

[F06] 删除文件
来源：http://guu.fktsv.cn

Py:   os.remove("a.txt")
来源：http://gci.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://xgx.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://ifm.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fre.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tph.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://dik.sweek.top

Ruby: File.delete("a.txt")
来源：http://psb.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://pim.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://hrf.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://flg.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://npp.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tml.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ucf.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zri.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hzj.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://brs.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ajp.sxryk.cn

[F08] 遍历目录
来源：http://vvp.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tpy.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ctk.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://wjs.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://mnh.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jfk.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvm.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://foq.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://ive.hammf.cn

[F09] 获取文件大小
来源：http://rtk.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://czm.yj202588.top

PHP:  filesize("a.txt");
来源：http://xqj.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://wxh.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://pop.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://ggh.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lmm.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://yva.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://ekk.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ahn.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zty.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xng.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eov.havefunace.top

TS:   path.extname("a.txt")
来源：http://xvo.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qxm.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rpo.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://are.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eso.shzxlz.cn

[F11] 复制与移动文件
来源：http://vnn.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pzb.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://api.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kss.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://luw.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzr.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tpb.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfj.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gii.yuxming.cn

[F12] CSV 读写
来源：http://gxv.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fcp.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xde.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ahc.jlsjyb.cn

TS:   // 同上
来源：http://juz.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://soj.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tjb.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://adt.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jfv.zhixingplan.top

================================================================================
来源：http://tow.hnxiangtu.top

G. 面向对象
来源：http://nqo.nanxuanxn.top

================================================================================
来源：http://rtf.zhongyouzk.top

[G01] 定义类
来源：http://wjg.daxiang520.top

Py:   class User: pass
来源：http://lci.jyoumei.cn

PHP:  class User {}
来源：http://dkl.fzhhl.top

JS:   class User {}
来源：http://jml.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://ive.yfazqb.com

Java: class User {}
来源：http://azu.shuidangran.top

Go:   type User struct { Name string }
来源：http://kqa.daxiang520.top

Ruby: class User; end
来源：http://cwt.nanxuanxn.top

C#:   class User {}
来源：http://nxq.gaohongyu789.top

[G02] 构造函数
来源：http://tto.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://sck.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://ajo.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://agl.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://ipe.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://jhp.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://woe.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://uhc.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://zhb.yuxming.cn

[G03] 实例属性
来源：http://xuv.jiagoushi.top

Py:   self.name = "x"
来源：http://uog.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://pho.yanxiufei.cn

JS:   this.name = "x";
来源：http://uhb.daxiang520.top

TS:   name: string = "x";
来源：http://zny.hcnkem.com

Java: private String name;
来源：http://tvw.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olq.uphjek.com

Ruby: @name = "x"
来源：http://xxh.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://grt.chenjidiqi.icu

[G04] 定义方法
来源：http://ane.ivvv.top

Py:   def greet(self): return self.name
来源：http://obk.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uim.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://yez.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://nkg.zdqjudy.top

Java: String greet() { return name; }
来源：http://yna.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://whu.cqqwz.cn

Ruby: def greet; @name; end
来源：http://tdt.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://ner.ywan-chungtsiang.top

[G05] 继承
来源：http://abd.c1oappe.top

Py:   class Admin(User): pass
来源：http://sfo.yonumen.top

PHP:  class Admin extends User {}
来源：http://bbk.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://jon.fengsongda.top

TS:   class Admin extends User {}
来源：http://dnq.yonumen.top

Java: class Admin extends User {}
来源：http://hni.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bwk.yuanzhike.top

Ruby: class Admin < User; end
来源：http://zjb.chenzaomai.com

C#:   class Admin : User {}
来源：http://rcf.shzxlz.cn

[G06] 重写方法
来源：http://vgk.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://syx.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wnx.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://foh.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://hdb.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ucr.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fzp.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://zuj.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://njh.quarkkingdee.top

[G07] 调用父类方法
来源：http://tpe.vehdjk.com

Py:   super().greet()
来源：http://xbm.sufxvd.cn

PHP:  parent::greet();
来源：http://cax.c1oappe.top

JS:   super.greet();
来源：http://dbj.nanxuanxn.top

TS:   super.greet();
来源：http://jot.quarkkingdee.top

Java: super.greet();
来源：http://wek.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://req.sjlbkw.cn

Ruby: super
来源：http://xsw.jianghu66.top

C#:   base.Greet();
来源：http://vgn.hnxiangtu.top

[G08] 静态方法与属性
来源：http://gvu.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://efv.cdnleiting.top

PHP:  public static function f() {}
来源：http://dpw.fengsongda.top

JS:   static f() {}
来源：http://xvi.hammf.cn

TS:   static f(): void {}
来源：http://qye.epnwcf.com

Java: static void f() {}
来源：http://stf.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eqv.guowangkeji.top

Ruby: def self.f; end
来源：http://boj.c1oappe.top

C#:   public static void F() {}
来源：http://kep.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://kgb.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://mlw.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tss.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kwv.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://qkk.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://ake.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://wvh.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zmr.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://cxk.daria6918.cn

[G10] 访问控制
来源：http://ffz.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://ivl.feifeiyinyue.top

PHP:  public / protected / private
来源：http://rqq.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://qjj.shangyingyoupin.top

TS:   public / protected / private
来源：http://jch.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://sly.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qxy.yueranfly.top

Ruby: public / protected / private
来源：http://cyx.jlsjyb.cn


<!-- 参考信息 -->