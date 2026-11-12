代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ucy.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rln.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dhu.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hle.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eap.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://twy.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://yft.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://khf.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://yii.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wlu.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cwv.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swi.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pkn.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyz.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sbw.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ixe.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pia.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://inh.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://roo.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lsi.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zye.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cco.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qdo.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fbp.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwa.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rur.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://lbw.sweek.top

Py:   f"{1234567:,}"
来源：http://gqr.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://mvz.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://nwz.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zrg.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ija.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://url.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wdu.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://bag.hnxiangtu.top

[E17] 首字母大写
来源：http://ubh.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://its.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mpn.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ooc.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqo.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yzv.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://spo.nwbrower.top

Ruby: s.capitalize
来源：http://crk.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ewj.yfazqb.com

[E18] 模板占位符替换
来源：http://ikf.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ety.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lga.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cmc.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kxi.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kqx.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fgw.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bwv.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://got.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://knw.hongshengwenyu.top

Py:   s.splitlines()
来源：http://qks.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cmb.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://nme.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://mes.gotoacloud.top

Java: s.lines().toList()
来源：http://opz.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://tzs.guowangkeji.top

Ruby: s.lines
来源：http://coh.yuanzhike.top

C#:   s.Split('\n')
来源：http://aop.bbcook.cn

[E20] 判断字符串是否为空
来源：http://gfk.uphjek.com

Py:   if not s:
来源：http://ysk.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ucv.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yfp.hysaishi.cn

TS:   if (s === "") {}
来源：http://jbf.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://nbz.svipenyu.cn

Go:   if s == "" {}
来源：http://zjx.jinqigfzy.top

Ruby: if s.empty?
来源：http://www.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jab.cqqwz.cn

[E21] 超长截断加省略号
来源：http://wqj.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xfn.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://luh.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gni.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jia.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gft.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://zyu.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ydi.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wfq.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://yrl.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yur.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jcv.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgk.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://urt.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ynb.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gxr.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://rvn.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqc.cdnleiting.top

================================================================================
来源：http://wip.ydzc1.top

F. 文件与目录
来源：http://bji.zhijiandao.cn

================================================================================
来源：http://wud.haohaochexian.top

[F01] 读取整个文件
来源：http://qjz.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nda.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://qqu.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bso.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://idi.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bta.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pnb.pycfn.com

Ruby: File.read("a.txt")
来源：http://nvl.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://bwt.chenlongwang.top

[F02] 逐行读取文件
来源：http://haj.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wcj.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://efz.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kig.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffy.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odd.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qds.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kwo.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://idz.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://vwk.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eus.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ued.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eru.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjl.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://idm.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ger.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://qxc.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwt.guannengcc.top

[F04] 追加写入文件
来源：http://xrg.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mtq.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://juv.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcm.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwo.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jxn.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kmb.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qig.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kci.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://sfe.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://urt.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://sny.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://atl.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://ysm.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qqg.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kfl.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://plz.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://myq.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://mpp.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://jkc.mhx1999.top

PHP:  unlink("a.txt");
来源：http://gga.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://whz.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://whv.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nvf.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://rhg.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://hzi.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://tos.meibo888.top

[F07] 创建目录（含多级）
来源：http://krk.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ydh.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbp.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qfs.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvu.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wes.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rnm.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwa.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://esz.dashuyun.cn

[F08] 遍历目录
来源：http://ttr.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmo.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xxa.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://yhf.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://wef.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uhb.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lqg.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://rjk.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://hlh.sjlbkw.cn

[F09] 获取文件大小
来源：http://krp.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://woi.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://ajn.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://cfy.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://mua.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pej.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ano.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://egw.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://nri.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://yam.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ikr.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fos.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hrs.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://bli.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qjz.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oth.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ylf.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://inh.kuanghao11.cn

[F11] 复制与移动文件
来源：http://jpp.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fea.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tuo.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhl.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vwc.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://knf.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qmp.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ywb.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://acm.gotoacloud.top

[F12] CSV 读写
来源：http://yyr.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tkw.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://awi.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zdi.jinyuanbaomall.cn

TS:   // 同上
来源：http://avy.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://whu.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rkh.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jxj.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hti.gotoacloud.top

================================================================================
来源：http://rwq.tianlin.xyz

G. 面向对象
来源：http://gjk.zhoulong.xyz

================================================================================
来源：http://qya.shanyushiyangtech.top

[G01] 定义类
来源：http://llg.zhengqikj.top

Py:   class User: pass
来源：http://hhk.uphjek.com

PHP:  class User {}
来源：http://ibc.yonumen.top

JS:   class User {}
来源：http://aor.316326.xyz

TS:   class User { name: string = ""; }
来源：http://olt.zhoulong.xyz

Java: class User {}
来源：http://ffl.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://ymm.jiagoushi.top

Ruby: class User; end
来源：http://zyx.snrcjt.cn

C#:   class User {}
来源：http://pmm.zdqjudy.top

[G02] 构造函数
来源：http://nfz.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://azc.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://zqu.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://bgd.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://fmg.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://und.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tqg.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://lcv.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://ebu.yj202588.top

[G03] 实例属性
来源：http://uof.cucudq.cn

Py:   self.name = "x"
来源：http://efu.zycfv.cn

PHP:  public string $name = "x";
来源：http://bqq.svipenyu.cn

JS:   this.name = "x";
来源：http://nao.sjlbkw.cn

TS:   name: string = "x";
来源：http://bsc.fzhhl.top

Java: private String name;
来源：http://smw.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nyx.zhixingplan.top

Ruby: @name = "x"
来源：http://xkm.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://slj.yuxming.cn

[G04] 定义方法
来源：http://ftu.jianghu66.top

Py:   def greet(self): return self.name
来源：http://ssq.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://blb.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://yus.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://jge.ivvv.top

Java: String greet() { return name; }
来源：http://pea.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hcr.nwbrower.top

Ruby: def greet; @name; end
来源：http://jty.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://blg.meibo888.top

[G05] 继承
来源：http://yuv.epnwcf.com

Py:   class Admin(User): pass
来源：http://skt.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://uis.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://lzf.meibo888.top

TS:   class Admin extends User {}
来源：http://qsd.zhijiandao.cn

Java: class Admin extends User {}
来源：http://fec.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wcb.jinqigufen.top

Ruby: class Admin < User; end
来源：http://alv.hnxiangtu.top

C#:   class Admin : User {}
来源：http://ojy.yuanzhike.top

[G06] 重写方法
来源：http://gtw.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://qza.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aal.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://wjh.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://vab.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://afy.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogw.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://eaj.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://ihn.mhx1999.top

[G07] 调用父类方法
来源：http://vht.zhengqikj.top

Py:   super().greet()
来源：http://cps.jianghu66.top

PHP:  parent::greet();
来源：http://xlt.jinqigufen.top

JS:   super.greet();
来源：http://ygm.havefunace.top

TS:   super.greet();
来源：http://goo.jqgufenzy.top

Java: super.greet();
来源：http://jeh.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sum.0kj1m.cn

Ruby: super
来源：http://nfr.jianghu66.top

C#:   base.Greet();
来源：http://mcz.vqdsnc.cn

[G08] 静态方法与属性
来源：http://avh.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xwh.ydzc1.top

PHP:  public static function f() {}
来源：http://eab.hnqzz.top

JS:   static f() {}
来源：http://qoy.chenlongwang.top

TS:   static f(): void {}
来源：http://txi.ctjpmb.com

Java: static void f() {}
来源：http://xep.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://chy.zhengqikj.top

Ruby: def self.f; end
来源：http://fux.chenjidiqi.icu

C#:   public static void F() {}
来源：http://ilz.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://khy.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://fzu.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://feh.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tix.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://bxl.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://qhi.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://rql.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tlz.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://tsz.sweek.top

[G10] 访问控制
来源：http://nzx.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://qaq.jiagoushi.top

PHP:  public / protected / private
来源：http://jqa.sysykeji.top

JS:   #private 字段；其余公开
来源：http://mjq.aibaodan.cn

TS:   public / protected / private
来源：http://tqz.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://jux.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://try.ydjk.org.cn

Ruby: public / protected / private
来源：http://zsn.cqqwz.cn

C#:   public / protected / private / internal
来源：http://voi.ctjpmb.com

[G11] getter / setter
来源：http://gkw.sxryk.cn

Py:   @property 与 @x.setter
来源：http://edt.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qbc.gzhubu.top

JS:   get name() { return this._name; }
来源：http://qoq.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://ejt.xziqi.cn

Java: public String getName() { return name; }
来源：http://dvz.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kqy.shanyushiyangkeji.top


<!-- 参考信息 -->