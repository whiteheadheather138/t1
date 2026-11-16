代发 wailian999

Go:   strings.Count(s, "a")
来源：http://uji.tanke756.top

Ruby: s.count("a")
来源：http://tuw.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://kom.yuanzhike.top

[E13] 逐字符遍历
来源：http://rdn.yongpay.top

Py:   for ch in s: print(ch)
来源：http://nha.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jgl.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jme.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kjz.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fem.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lse.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lqx.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iel.yj20258888.top

[E14] URL 编码与 Base64
来源：http://nnk.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hdf.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ihz.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vka.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tbk.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xfv.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bdl.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qjc.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vtm.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://gnk.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xkc.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tdk.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zkl.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vig.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nng.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rup.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qoc.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eqr.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://xcs.ybcxt.top

Py:   f"{1234567:,}"
来源：http://pww.zhengqikj.top

PHP:  number_format(1234567);
来源：http://rpv.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rfc.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://vki.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xos.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nfw.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ffn.yonumen.top

C#:   1234567.ToString("N0")
来源：http://hhn.redwolf501.top

[E17] 首字母大写
来源：http://pck.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cib.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oph.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmg.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gvu.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://alt.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmb.guannengcc.top

Ruby: s.capitalize
来源：http://muo.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jan.yfazqb.com

[E18] 模板占位符替换
来源：http://oih.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kir.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://owd.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gcv.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://skq.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bzm.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jwu.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhk.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rmd.yuxming.cn

[E19] 多行文本按行拆分
来源：http://xhd.yangfankeji.com

Py:   s.splitlines()
来源：http://qoz.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qvm.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://esi.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://jvv.nanxinkj.top

Java: s.lines().toList()
来源：http://soy.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://dst.jinqigufen.top

Ruby: s.lines
来源：http://scy.tanke756.top

C#:   s.Split('\n')
来源：http://ajg.guannengcc.top

[E20] 判断字符串是否为空
来源：http://cyt.tarul.cn

Py:   if not s:
来源：http://hsl.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rvo.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jzd.hnxiangtu.top

TS:   if (s === "") {}
来源：http://jud.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://qxx.9152youxi.cn

Go:   if s == "" {}
来源：http://xmx.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://gcf.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://puk.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://yxi.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xjt.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tqf.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jaa.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lla.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ftb.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://lda.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gng.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zmi.mhx1999.top

[E22] 字节长度与字符长度
来源：http://tfl.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nxy.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggi.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tnv.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://elj.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ubw.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qko.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://ugh.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://edu.vqdsnc.cn

================================================================================
来源：http://zmk.shanyushiyangkeji.top

F. 文件与目录
来源：http://xgg.chenlongwang.top

================================================================================
来源：http://fho.9152youxi.cn

[F01] 读取整个文件
来源：http://akj.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tvg.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://zrr.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rvp.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lot.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yxy.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gkx.birdmap.top

Ruby: File.read("a.txt")
来源：http://cxz.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://tvv.tian-w.cn

[F02] 逐行读取文件
来源：http://yjl.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hqn.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pif.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lio.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ssl.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aki.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vwb.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nvc.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wjq.yonumen.top

[F03] 写入文件（覆盖）
来源：http://eso.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wyg.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rvx.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vvy.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqi.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lyg.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wrp.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://hip.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eqk.guannengcc.top

[F04] 追加写入文件
来源：http://cdi.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jnh.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://smi.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufj.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ryo.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://klg.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zgu.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vgv.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wyz.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://qpt.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ypo.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://mzp.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://rnw.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://yfh.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fbt.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://awq.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://gar.havefunace.top

C#:   File.Exists("a.txt")
来源：http://rwk.fanxiaobao.xyz

[F06] 删除文件
来源：http://rct.daxiang520.top

Py:   os.remove("a.txt")
来源：http://jcm.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://aqy.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://hzu.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://ckd.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://adm.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://snk.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://crt.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://hlw.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://due.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ukv.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gsw.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://igc.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfs.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://any.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xqo.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ymm.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uav.ehwqpu.com

[F08] 遍历目录
来源：http://pjt.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zyd.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fvw.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://rmn.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://kst.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://osa.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jwg.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://bbe.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://jkc.zhongyouzk.top

[F09] 获取文件大小
来源：http://khu.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://ymu.jianghu66.top

PHP:  filesize("a.txt");
来源：http://ewd.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://inl.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://bco.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gpx.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oat.iojbl.cn

Ruby: File.size("a.txt")
来源：http://trj.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://qfd.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://keg.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fto.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vgf.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hmv.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://pcc.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xwi.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://byy.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://msd.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fsq.uphjek.com

[F11] 复制与移动文件
来源：http://cll.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kmx.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gwf.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sao.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xsx.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://het.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzy.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qxb.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cts.feifeiyinyue.top

[F12] CSV 读写
来源：http://xmk.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://izu.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ujp.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nzu.bbcook.cn

TS:   // 同上
来源：http://bxi.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nfs.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sus.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ilb.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qqt.wangshuangyany.cn

================================================================================
来源：http://lco.hongshengwenyu.top

G. 面向对象
来源：http://dzw.hfpthk.cn

================================================================================
来源：http://smx.hammf.cn

[G01] 定义类
来源：http://hbq.jianghu66.top

Py:   class User: pass
来源：http://jxx.bjfxy.top

PHP:  class User {}
来源：http://bcv.yuanzhike.top

JS:   class User {}
来源：http://wex.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://zyo.wangdashe.top

Java: class User {}
来源：http://dez.ydzc1.top

Go:   type User struct { Name string }
来源：http://rtb.ydzc1.top

Ruby: class User; end
来源：http://vpb.yj20258.top

C#:   class User {}
来源：http://fsd.cheryme.top

[G02] 构造函数
来源：http://hgp.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://ynm.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://ewz.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://crb.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://ojo.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://rud.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rlf.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://dtf.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://apj.chenlongwang.top

[G03] 实例属性
来源：http://ctr.9152youxi.cn

Py:   self.name = "x"
来源：http://nha.guowangkeji.top

PHP:  public string $name = "x";
来源：http://lhv.redwolf501.top

JS:   this.name = "x";
来源：http://pvn.epnwcf.com

TS:   name: string = "x";
来源：http://afx.tanke756.top

Java: private String name;
来源：http://dkv.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kxo.hysaishi.cn

Ruby: @name = "x"
来源：http://jsq.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://dwp.tianlin.xyz

[G04] 定义方法
来源：http://fzz.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://zip.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://idk.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://nev.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://rsq.cucudq.cn

Java: String greet() { return name; }
来源：http://wvx.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ynv.jiagoushi.top

Ruby: def greet; @name; end
来源：http://dyh.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://pbt.ywan-chungtsiang.top

[G05] 继承
来源：http://uxf.sweek.top

Py:   class Admin(User): pass
来源：http://asq.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://tvk.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://vun.hnqzz.top

TS:   class Admin extends User {}
来源：http://qsj.gotoacloud.top

Java: class Admin extends User {}
来源：http://qom.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yqv.nwbrower.top

Ruby: class Admin < User; end
来源：http://buz.yangfankeji.com

C#:   class Admin : User {}
来源：http://tzv.bbcook.cn

[G06] 重写方法
来源：http://ytp.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://dge.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ibs.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://dkr.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://iem.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://kty.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjd.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://izt.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://lep.vqdsnc.cn

[G07] 调用父类方法
来源：http://bwz.aibaodan.cn

Py:   super().greet()
来源：http://etv.hnxiangtu.top

PHP:  parent::greet();
来源：http://imt.guannengcc.top

JS:   super.greet();
来源：http://taz.fanxiaobao.xyz

TS:   super.greet();
来源：http://zug.xingfuxueyuan.xyz

Java: super.greet();
来源：http://vcr.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://isw.hesvh.cn

Ruby: super
来源：http://qga.vqdsnc.cn

C#:   base.Greet();
来源：http://kxk.tarul.cn

[G08] 静态方法与属性
来源：http://yev.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dva.gzhubu.top

PHP:  public static function f() {}
来源：http://luy.jiagoushi.top

JS:   static f() {}
来源：http://fyx.tianlin.xyz

TS:   static f(): void {}
来源：http://qdw.dashuyun.cn

Java: static void f() {}
来源：http://cva.guowangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lns.guowangkeji.top

Ruby: def self.f; end
来源：http://vbe.fengsongda.top

C#:   public static void F() {}
来源：http://quy.yueranfly.top

[G09] 接口 / 抽象类
来源：http://yxn.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://pck.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://ehs.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://tzx.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://juz.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://pmb.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://bko.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qel.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://pyf.jyoumei.cn

[G10] 访问控制
来源：http://vqq.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://ygx.redwolf501.top

PHP:  public / protected / private
来源：http://pty.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://stw.wangdashe.top

TS:   public / protected / private
来源：http://rxo.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://mmf.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uzk.zhongyouzk.top

Ruby: public / protected / private
来源：http://qpu.svipenyu.cn

C#:   public / protected / private / internal
来源：http://wno.gaohongyu789.top

[G11] getter / setter
来源：http://vui.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://txc.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qus.chenzaomai.com


<!-- 参考信息 -->