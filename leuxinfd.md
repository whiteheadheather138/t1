代发 wailian999

Go:   strings.Count(s, "a")
来源：http://zul.zycfv.cn

Ruby: s.count("a")
来源：http://llx.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://bbk.andypj.xyz

[E13] 逐字符遍历
来源：http://qtt.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://bnp.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywj.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kbe.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://clf.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cpo.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wtr.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://czy.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fvq.birdmap.top

[E14] URL 编码与 Base64
来源：http://asi.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ezm.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eod.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ecl.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zmq.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://srs.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iwl.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yfl.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uhc.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://bmr.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ejx.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sdj.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jcn.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://btl.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mti.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gcs.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jwk.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lof.jyoumei.cn

[E16] 数字千分位
来源：http://qwf.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://axr.sysykeji.top

PHP:  number_format(1234567);
来源：http://lhd.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nxd.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://cvi.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gcl.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gms.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjy.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://yge.nwbrower.top

[E17] 首字母大写
来源：http://nth.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qoi.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://qrc.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsd.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://itv.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://luq.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mey.chenjidiqi.icu

Ruby: s.capitalize
来源：http://gdj.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxw.kuanghao11.cn

[E18] 模板占位符替换
来源：http://dwf.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vhv.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qln.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qpv.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://afx.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yff.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xhq.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlp.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hfi.guannengcc.top

[E19] 多行文本按行拆分
来源：http://mhf.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://ekz.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://viq.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://rra.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://rmq.zycfv.cn

Java: s.lines().toList()
来源：http://zwi.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://gxd.shzxlz.cn

Ruby: s.lines
来源：http://cic.tarul.cn

C#:   s.Split('\n')
来源：http://ktv.cucudq.cn

[E20] 判断字符串是否为空
来源：http://nwq.sjlbkw.cn

Py:   if not s:
来源：http://ena.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xxd.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ggm.nwbrower.top

TS:   if (s === "") {}
来源：http://rvy.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://daj.gaohongyu789.top

Go:   if s == "" {}
来源：http://xby.zdqjudy.top

Ruby: if s.empty?
来源：http://uwp.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pqt.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://wwd.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://atm.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wvh.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxb.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rox.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mug.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://ybs.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bbp.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xnw.fengsongda.top

[E22] 字节长度与字符长度
来源：http://owy.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nsa.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhy.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pgc.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhs.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cdr.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://weg.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://cge.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sxm.nwbrower.top

================================================================================
来源：http://ibw.zhixingplan.top

F. 文件与目录
来源：http://nkk.tianlin.xyz

================================================================================
来源：http://zrl.xuetiantiany.cn

[F01] 读取整个文件
来源：http://emu.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hpj.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://jba.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iuf.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oyi.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://lzg.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fzj.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://coc.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://uge.smart0.xyz

[F02] 逐行读取文件
来源：http://ntv.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jpo.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fbt.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwz.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jsb.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyx.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dwd.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zie.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tpe.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://vid.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sxp.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://poo.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osb.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aks.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dlk.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://evg.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://umn.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lqx.xylfe.cn

[F04] 追加写入文件
来源：http://twu.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lmr.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jia.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bgd.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yoi.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mkz.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://agy.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tdn.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spa.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://yzn.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://maw.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://yie.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://udu.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://lop.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vva.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bgh.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://hel.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://yct.ppjwa.cn

[F06] 删除文件
来源：http://syt.yvedp.cn

Py:   os.remove("a.txt")
来源：http://dey.daxiang520.top

PHP:  unlink("a.txt");
来源：http://phg.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://ogf.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://sfb.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sea.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://hwz.birdmap.top

Ruby: File.delete("a.txt")
来源：http://kgf.yj20258.top

C#:   File.Delete("a.txt");
来源：http://enm.tarul.cn

[F07] 创建目录（含多级）
来源：http://frc.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aqk.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hob.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ije.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffb.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fxq.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://frf.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cyu.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uxq.nanxinkj.top

[F08] 遍历目录
来源：http://ewo.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hhg.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nwg.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://gil.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://hgl.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pqa.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ctl.uphjek.com

Ruby: Dir.children("dir")
来源：http://djf.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://ukl.quarkkingdee.top

[F09] 获取文件大小
来源：http://bcb.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://azr.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://rzg.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://cmf.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://mgd.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fmc.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://crp.bbcook.cn

Ruby: File.size("a.txt")
来源：http://yfh.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://iib.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://blo.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgq.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjt.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ppn.sxryk.cn

TS:   path.extname("a.txt")
来源：http://rqv.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://olm.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hsb.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ohw.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nek.c1oappe.top

[F11] 复制与移动文件
来源：http://zbo.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jer.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cte.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mez.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eot.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uvq.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://but.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://unt.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qll.tarul.cn

[F12] CSV 读写
来源：http://woe.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://flk.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://etj.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pub.jlsjyb.cn

TS:   // 同上
来源：http://nzz.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zcc.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lqh.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oir.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ntm.yj20258.top

================================================================================
来源：http://vta.andypj.xyz

G. 面向对象
来源：http://nbf.jinqigufen.top

================================================================================
来源：http://bzt.xziqi.cn

[G01] 定义类
来源：http://kvq.hnqzz.top

Py:   class User: pass
来源：http://vpl.zdqjudy.top

PHP:  class User {}
来源：http://hue.aizwys.cn

JS:   class User {}
来源：http://ild.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://mjt.tanke756.top

Java: class User {}
来源：http://dnm.svipenyu.cn

Go:   type User struct { Name string }
来源：http://gri.zycfv.cn

Ruby: class User; end
来源：http://mig.xuanzx.com

C#:   class User {}
来源：http://mmy.jianghu66.top

[G02] 构造函数
来源：http://ywd.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://eyh.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://otu.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://qes.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://dnr.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://rsl.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zah.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://klx.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://dob.meibo888.top

[G03] 实例属性
来源：http://bwf.jinqigfzy.top

Py:   self.name = "x"
来源：http://dte.shuidangran.top

PHP:  public string $name = "x";
来源：http://qdn.ehwqpu.com

JS:   this.name = "x";
来源：http://vbg.svipenyu.cn

TS:   name: string = "x";
来源：http://pdm.gaohongyu789.top

Java: private String name;
来源：http://zyl.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cuh.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://lvx.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://pnc.daxiang520.top

[G04] 定义方法
来源：http://pgp.wangdashe.top

Py:   def greet(self): return self.name
来源：http://zkj.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kkc.yfazqb.com

JS:   greet() { return this.name; }
来源：http://mig.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://qze.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://mwc.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xul.yonumen.top

Ruby: def greet; @name; end
来源：http://wan.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://wwf.gzhubu.top

[G05] 继承
来源：http://nqu.hcnkem.com

Py:   class Admin(User): pass
来源：http://vsy.tanke756.top

PHP:  class Admin extends User {}
来源：http://swq.c1oappe.top

JS:   class Admin extends User {}
来源：http://ckz.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://wfd.ybcxt.top

Java: class Admin extends User {}
来源：http://slk.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yna.ybcxt.top

Ruby: class Admin < User; end
来源：http://aiv.yuanzhike.top

C#:   class Admin : User {}
来源：http://zou.fengsongda.top

[G06] 重写方法
来源：http://kxd.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://jvk.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hnz.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://cew.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://czx.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://iaf.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pmb.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://vpd.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://wvf.fengsongda.top

[G07] 调用父类方法
来源：http://yqw.yj202588.top

Py:   super().greet()
来源：http://hii.hammf.cn

PHP:  parent::greet();
来源：http://kov.xylfe.cn

JS:   super.greet();
来源：http://uby.aizwys.cn

TS:   super.greet();
来源：http://ftx.hnxiangtu.top

Java: super.greet();
来源：http://gkd.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://swi.dashuyun.cn

Ruby: super
来源：http://odd.shangyingyoupin.top

C#:   base.Greet();
来源：http://tgv.zhongyouzk.top

[G08] 静态方法与属性
来源：http://vji.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yqa.iojbl.cn

PHP:  public static function f() {}
来源：http://yrp.gaohongyu789.top

JS:   static f() {}
来源：http://tjt.redwolf501.top

TS:   static f(): void {}
来源：http://edr.daria6918.cn

Java: static void f() {}
来源：http://diz.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://epd.ehwqpu.com

Ruby: def self.f; end
来源：http://zfo.havefunace.top

C#:   public static void F() {}
来源：http://wsv.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://ssz.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://nnd.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://ctp.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://koh.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://xrx.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://owb.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://kbr.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vsq.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://pzn.tarul.cn

[G10] 访问控制
来源：http://asw.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://pap.zycfv.cn

PHP:  public / protected / private
来源：http://nkg.pycfn.com

JS:   #private 字段；其余公开
来源：http://qak.snrcjt.cn

TS:   public / protected / private
来源：http://pth.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://erz.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rzc.yj202588.top

Ruby: public / protected / private
来源：http://osz.sweek.top

C#:   public / protected / private / internal
来源：http://muk.xylfe.cn

[G11] getter / setter
来源：http://hvz.yj20258.top

Py:   @property 与 @x.setter
来源：http://rnz.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vsa.hammf.cn


<!-- 参考信息 -->