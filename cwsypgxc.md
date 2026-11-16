代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ljo.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tji.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vgi.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nbe.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xkh.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://zot.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mwj.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ynb.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tva.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nlk.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uvh.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bte.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uoa.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ccf.jqgfzy.top

[E16] 数字千分位
来源：http://kik.hesvh.cn

Py:   f"{1234567:,}"
来源：http://jcj.mhx1999.top

PHP:  number_format(1234567);
来源：http://hpy.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mev.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qew.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vae.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rxb.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://opk.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://lmz.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://von.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://anw.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ewh.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ysf.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yxc.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jhg.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rvi.yj20258.top

Ruby: s.capitalize
来源：http://var.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jnj.tarul.cn

[E18] 模板占位符替换
来源：http://vie.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ypd.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://suf.dianchejie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bhw.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nqx.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uqo.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qlh.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tgv.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ios.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://jkn.aibaodan.cn

Py:   s.splitlines()
来源：http://xwh.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qid.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://hps.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://acw.dashuyun.cn

Java: s.lines().toList()
来源：http://dtu.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://jzv.wangdashe.top

Ruby: s.lines
来源：http://dfy.zhixingplan.top

C#:   s.Split('\n')
来源：http://cmc.xuanzx.com

[E20] 判断字符串是否为空
来源：http://uba.yueranfly.top

Py:   if not s:
来源：http://jfw.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ioj.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zsc.epnwcf.com

TS:   if (s === "") {}
来源：http://crq.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://bah.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://cry.yuxming.cn

Ruby: if s.empty?
来源：http://ylz.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kqq.guannengcc.top

[E21] 超长截断加省略号
来源：http://mng.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqd.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jsg.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bdf.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://swk.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://utf.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ryg.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://chz.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://enj.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://iap.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ton.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oun.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nag.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xuf.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcn.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mqq.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://cxn.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ovo.zhoulong.xyz

================================================================================
来源：http://hvn.jinghuilouyu.cn

F. 文件与目录
来源：http://cpb.52xcode.cn

================================================================================
来源：http://cgw.gotoacloud.top

[F01] 读取整个文件
来源：http://qrw.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jeu.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://nac.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xjh.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://txq.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oir.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xzv.cucudq.cn

Ruby: File.read("a.txt")
来源：http://ziq.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://hed.hywenlv.cn

[F02] 逐行读取文件
来源：http://zuy.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pwb.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://deu.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eih.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilk.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jtb.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tcv.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ofd.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ink.cheryme.top

[F03] 写入文件（覆盖）
来源：http://iav.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uch.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://dxw.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lgt.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tul.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aln.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://asu.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://bus.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bej.ydjk.org.cn

[F04] 追加写入文件
来源：http://yyx.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://apk.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eil.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mtd.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbl.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gny.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gxm.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jwo.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spu.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://fvh.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kvq.pycfn.com

PHP:  file_exists("a.txt");
来源：http://xbu.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://kka.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://vzz.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kmz.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qpo.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://rcg.havefunace.top

C#:   File.Exists("a.txt")
来源：http://jcf.nanxinkj.top

[F06] 删除文件
来源：http://bkx.ydzc1.top

Py:   os.remove("a.txt")
来源：http://trj.sysykeji.top

PHP:  unlink("a.txt");
来源：http://oaz.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://yqa.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://dtk.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ymz.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://phc.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://vug.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://szp.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://jhu.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sat.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wom.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khd.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgf.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kpb.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mes.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bgc.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zub.9152youxi.cn

[F08] 遍历目录
来源：http://ipv.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://haz.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://euk.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://lua.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://bkw.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vbv.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvu.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://vsf.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://zdf.vehdjk.com

[F09] 获取文件大小
来源：http://les.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://tbt.bbcook.cn

PHP:  filesize("a.txt");
来源：http://afl.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://oxi.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://cry.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://syb.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehi.yonumen.top

Ruby: File.size("a.txt")
来源：http://heq.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://snb.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://goa.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://emg.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cme.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vyy.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://qjj.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://soc.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wvj.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tgd.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bam.jinqigfzy.top

[F11] 复制与移动文件
来源：http://gzv.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jvb.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sgu.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqh.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iaz.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cau.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nra.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nnd.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rox.zhiwuduotai.top

[F12] CSV 读写
来源：http://mfp.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zch.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tzs.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jge.52xcode.cn

TS:   // 同上
来源：http://ioy.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oca.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxl.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mem.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yyd.dianchejie.cn

================================================================================
来源：http://qsq.andypj.xyz

G. 面向对象
来源：http://eos.zhixingplan.top

================================================================================
来源：http://cjm.shangyingyoupin.top

[G01] 定义类
来源：http://whb.kuanghao11.cn

Py:   class User: pass
来源：http://cbs.pengpengdd.cyou

PHP:  class User {}
来源：http://aqv.zhengqikj.top

JS:   class User {}
来源：http://gxs.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://aje.fzhhl.top

Java: class User {}
来源：http://zfj.jianghu66.top

Go:   type User struct { Name string }
来源：http://mar.fktsv.cn

Ruby: class User; end
来源：http://dzm.nwbrower.top

C#:   class User {}
来源：http://tbj.cqqwz.cn

[G02] 构造函数
来源：http://cgr.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://kgl.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://qbk.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://nss.316326.xyz

TS:   constructor(public name: string) {}
来源：http://fyb.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://zgk.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wjw.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://kmh.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://mdk.dianchejie.cn

[G03] 实例属性
来源：http://fon.yfazqb.com

Py:   self.name = "x"
来源：http://yfc.52xcode.cn

PHP:  public string $name = "x";
来源：http://qqu.c1oappe.top

JS:   this.name = "x";
来源：http://lxe.kuanghao11.cn

TS:   name: string = "x";
来源：http://rep.c1oappe.top

Java: private String name;
来源：http://pqx.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gom.haohaochexian.top

Ruby: @name = "x"
来源：http://zdu.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://uvc.hammf.cn

[G04] 定义方法
来源：http://qfi.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://dak.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wdm.sweek.top

JS:   greet() { return this.name; }
来源：http://mhp.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://asx.kuanghao11.cn

Java: String greet() { return name; }
来源：http://nhe.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jkk.ybcxt.top

Ruby: def greet; @name; end
来源：http://goc.fehbvm.com

C#:   public string Greet() => Name;
来源：http://gej.yuxming.cn

[G05] 继承
来源：http://irl.cdnleiting.top

Py:   class Admin(User): pass
来源：http://ufr.havefunace.top

PHP:  class Admin extends User {}
来源：http://wpt.aibaodan.cn

JS:   class Admin extends User {}
来源：http://qau.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://ldg.sxryk.cn

Java: class Admin extends User {}
来源：http://tkw.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wpc.sxryk.cn

Ruby: class Admin < User; end
来源：http://dub.yj202588.top

C#:   class Admin : User {}
来源：http://ipj.tianlin.xyz

[G06] 重写方法
来源：http://mlm.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://ucs.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://psq.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://bwo.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://hdf.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://iab.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qqv.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://zvb.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://hfg.tanke756.top

[G07] 调用父类方法
来源：http://hfq.yueranfly.top

Py:   super().greet()
来源：http://orp.guowangkeji.top

PHP:  parent::greet();
来源：http://usz.hnqzz.top

JS:   super.greet();
来源：http://rgc.yj202588.top

TS:   super.greet();
来源：http://iak.chenjidiqi.icu

Java: super.greet();
来源：http://fvo.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ouo.epnwcf.com

Ruby: super
来源：http://kbb.yongpay.top

C#:   base.Greet();
来源：http://iwf.tanke756.top

[G08] 静态方法与属性
来源：http://ldp.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ast.guowangkeji.top

PHP:  public static function f() {}
来源：http://ljl.yj20258.top

JS:   static f() {}
来源：http://oya.zhixingplan.top

TS:   static f(): void {}
来源：http://lmz.bjfxy.top

Java: static void f() {}
来源：http://aop.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ycq.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://bkd.daria6918.cn

C#:   public static void F() {}
来源：http://udr.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://gte.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://nkt.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://dxs.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qpo.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://knh.andypj.xyz

Java: interface Shape { double area(); }
来源：http://pld.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://iom.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xbg.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://euz.nwbrower.top

[G10] 访问控制
来源：http://jnb.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://qrz.9152youxi.cn

PHP:  public / protected / private
来源：http://iiq.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://sgz.jyoumei.cn

TS:   public / protected / private
来源：http://yvy.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://bid.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pgu.cucudq.cn

Ruby: public / protected / private
来源：http://jan.cheryme.top

C#:   public / protected / private / internal
来源：http://ztw.cashguo.top

[G11] getter / setter
来源：http://zsw.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://qco.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pkb.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://ftv.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://nfk.yj202588.top

Java: public String getName() { return name; }
来源：http://fvq.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://god.nanxinkj.top

Ruby: attr_accessor :name
来源：http://yrk.fktsv.cn

C#:   public string Name { get; set; }
来源：http://iiu.aibaodan.cn

[G12] 对象转字符串
来源：http://mft.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://aen.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://onw.shuidangran.top

JS:   toString() { return this.name; }
来源：http://nno.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://dsu.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://zug.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://gnj.yfazqb.com

Ruby: def to_s; @name; end
来源：http://wyk.birdmap.top

C#:   public override string ToString() => Name;
来源：http://txy.smart0.xyz

[G13] 判断对象类型
来源：http://yzd.yanxiufei.cn


<!-- 参考信息 -->