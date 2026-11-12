代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://slc.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lgt.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jsu.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eab.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ssr.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://rbz.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gkh.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mqp.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xhp.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yjm.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bgg.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ylv.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oea.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ioc.jiagoushi.top

[E16] 数字千分位
来源：http://uxq.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://wtc.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://eei.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://pgj.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://koy.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://icc.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kgs.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mmq.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://mtn.fzhhl.top

[E17] 首字母大写
来源：http://qeu.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://idg.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rbb.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxx.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zur.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ccm.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tbg.zhongyouzk.top

Ruby: s.capitalize
来源：http://ubs.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dfn.pycfn.com

[E18] 模板占位符替换
来源：http://usl.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://esq.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yft.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://awn.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kex.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wge.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jza.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ich.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://roc.yueranfly.top

[E19] 多行文本按行拆分
来源：http://eog.yj202588.top

Py:   s.splitlines()
来源：http://bhw.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cbk.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://llw.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://aai.gaohongyu789.top

Java: s.lines().toList()
来源：http://mhw.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://ird.dianchejie.cn

Ruby: s.lines
来源：http://qru.cdnleiting.top

C#:   s.Split('\n')
来源：http://sxm.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://fdo.hnqzz.top

Py:   if not s:
来源：http://jhh.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jhi.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ett.xuanzx.com

TS:   if (s === "") {}
来源：http://coq.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://hcn.hysaishi.cn

Go:   if s == "" {}
来源：http://wxn.hongshengwenyu.top

Ruby: if s.empty?
来源：http://vtp.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sdr.havefunace.top

[E21] 超长截断加省略号
来源：http://wiy.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fdr.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvl.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpo.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndg.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ywv.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://bsv.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gnf.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nkx.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://udi.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rcg.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ryg.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyq.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywi.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bbu.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qgf.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://ywv.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jof.yvedp.cn

================================================================================
来源：http://gjw.sweek.top

F. 文件与目录
来源：http://scd.hammf.cn

================================================================================
来源：http://dlf.hnqzz.top

[F01] 读取整个文件
来源：http://kdy.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pag.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://leq.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nhy.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qpr.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://spg.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qgg.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://ehd.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://wce.shzxlz.cn

[F02] 逐行读取文件
来源：http://fog.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jjr.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ljz.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qog.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbw.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hky.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iwv.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bkb.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://auc.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://lwa.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gsk.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://uvx.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yuh.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxq.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qzo.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lmk.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://xvg.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbt.shuidangran.top

[F04] 追加写入文件
来源：http://ked.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dqw.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://glb.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehc.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ela.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://led.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mab.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://veo.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://roy.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://dlw.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://omy.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://wzq.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://jns.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://lqo.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vvv.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysf.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://okq.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://rno.mhx1999.top

[F06] 删除文件
来源：http://syg.fengsongda.top

Py:   os.remove("a.txt")
来源：http://sjh.pycfn.com

PHP:  unlink("a.txt");
来源：http://vjz.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://bnx.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yno.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://auz.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://ygn.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://ntq.havefunace.top

C#:   File.Delete("a.txt");
来源：http://civ.redwolf501.top

[F07] 创建目录（含多级）
来源：http://xmt.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ymt.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cot.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcp.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gvc.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nab.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fvx.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://geo.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jeq.ydzc1.top

[F08] 遍历目录
来源：http://dho.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://khc.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tve.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://lis.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://jxb.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cal.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://urz.yj202588.top

Ruby: Dir.children("dir")
来源：http://tyx.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://smq.sjlbkw.cn

[F09] 获取文件大小
来源：http://wis.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://ppn.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://qkq.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://nog.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://mnf.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://pjl.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://drh.tanke756.top

Ruby: File.size("a.txt")
来源：http://hxs.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://kxl.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://drr.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uum.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zyg.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vaq.yuxming.cn

TS:   path.extname("a.txt")
来源：http://ygj.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://psj.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpb.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzy.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://feq.sweek.top

[F11] 复制与移动文件
来源：http://dyt.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wfb.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rko.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfm.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pai.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yzb.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yqi.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hav.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wmr.xuetiantiany.cn

[F12] CSV 读写
来源：http://jcp.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ehl.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qzo.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hjb.xuanzx.com

TS:   // 同上
来源：http://aeb.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xsg.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hjl.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ehi.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vyx.pengpengdd.cyou

================================================================================
来源：http://vkz.daxiang520.top

G. 面向对象
来源：http://ynt.jlsjyb.cn

================================================================================
来源：http://lxq.cqqwz.cn

[G01] 定义类
来源：http://uvc.zhaomingkeji.xyz

Py:   class User: pass
来源：http://zut.meibo888.top

PHP:  class User {}
来源：http://ndr.hywenlv.cn

JS:   class User {}
来源：http://epv.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://wra.havefunace.top

Java: class User {}
来源：http://psx.guannengcc.top

Go:   type User struct { Name string }
来源：http://ygt.svipenyu.cn

Ruby: class User; end
来源：http://vid.ppjwa.cn

C#:   class User {}
来源：http://wyl.quarkkingdee.top

[G02] 构造函数
来源：http://ull.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://spt.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://zhd.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://wqf.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://ulb.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://exw.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vxe.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://stq.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://xuk.fengsongda.top

[G03] 实例属性
来源：http://qin.hcnkem.com

Py:   self.name = "x"
来源：http://kxw.ydzc1.top

PHP:  public string $name = "x";
来源：http://gzo.feifeiyinyue.top

JS:   this.name = "x";
来源：http://qke.vqdsnc.cn

TS:   name: string = "x";
来源：http://slw.zhixingplan.top

Java: private String name;
来源：http://ebd.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fhl.andypj.xyz

Ruby: @name = "x"
来源：http://crd.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ejq.sufxvd.cn

[G04] 定义方法
来源：http://syl.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://zsr.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://omt.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://qmz.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://ojk.snrcjt.cn

Java: String greet() { return name; }
来源：http://moj.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://njj.zhixingplan.top

Ruby: def greet; @name; end
来源：http://ivt.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://ynw.ppjwa.cn

[G05] 继承
来源：http://npy.jinqigufen.top

Py:   class Admin(User): pass
来源：http://jbz.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://sue.c1oappe.top

JS:   class Admin extends User {}
来源：http://van.jyoumei.cn

TS:   class Admin extends User {}
来源：http://wdy.ivvv.top

Java: class Admin extends User {}
来源：http://mwc.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sfd.fktsv.cn

Ruby: class Admin < User; end
来源：http://yzk.ppjwa.cn

C#:   class Admin : User {}
来源：http://rge.zhoulong.xyz

[G06] 重写方法
来源：http://taj.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://xfl.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ecx.tarul.cn

JS:   greet() { return "admin"; }
来源：http://hhk.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://upn.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://oqi.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zpy.sweek.top

Ruby: def greet; "admin"; end
来源：http://fgf.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://hpv.yonumen.top

[G07] 调用父类方法
来源：http://qgo.xuanzx.com

Py:   super().greet()
来源：http://obi.yueranfly.top

PHP:  parent::greet();
来源：http://sik.yanxiufei.cn

JS:   super.greet();
来源：http://fvj.nanxuanxn.top

TS:   super.greet();
来源：http://kfn.nanxinkj.top

Java: super.greet();
来源：http://usa.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ngy.cdnleiting.top

Ruby: super
来源：http://tnr.dashuyun.cn

C#:   base.Greet();
来源：http://vxz.ppjwa.cn

[G08] 静态方法与属性
来源：http://noo.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mdb.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://flp.smart0.xyz

JS:   static f() {}
来源：http://ffw.kuanghao11.cn

TS:   static f(): void {}
来源：http://dng.iojbl.cn

Java: static void f() {}
来源：http://mqy.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://mcy.xinyue.icu

Ruby: def self.f; end
来源：http://xeo.jyoumei.cn

C#:   public static void F() {}
来源：http://ype.ybcxt.top

[G09] 接口 / 抽象类
来源：http://qox.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://mnl.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://rze.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pmj.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://wbe.gzhubu.top

Java: interface Shape { double area(); }
来源：http://tda.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://fuz.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nda.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://uaz.guowangkeji.top

[G10] 访问控制
来源：http://oma.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://owm.mhx1999.top

PHP:  public / protected / private
来源：http://grl.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://wcf.aibaodan.cn

TS:   public / protected / private
来源：http://xxu.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://dbq.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tni.yongpay.top

Ruby: public / protected / private
来源：http://rav.xylfe.cn

C#:   public / protected / private / internal
来源：http://gvs.c1oappe.top

[G11] getter / setter
来源：http://cyq.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://mdn.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kcp.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://eck.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://sqa.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://lps.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bpk.gotoacloud.top

Ruby: attr_accessor :name
来源：http://vaw.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://loe.jqgufenzy.top

[G12] 对象转字符串
来源：http://nls.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://epg.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hjy.cashguo.top

JS:   toString() { return this.name; }
来源：http://itt.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://mom.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://hnq.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kta.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://nec.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://imp.chenjidiqi.icu

[G13] 判断对象类型
来源：http://qkb.guowangkeji.top


<!-- 参考信息 -->