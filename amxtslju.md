代发 wailian999

Go:   strings.Count(s, "a")
来源：http://tmo.guowangkeji.top

Ruby: s.count("a")
来源：http://ruf.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://xag.zycfv.cn

[E13] 逐字符遍历
来源：http://lkc.sweek.top

Py:   for ch in s: print(ch)
来源：http://nph.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zlz.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gwq.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://rnu.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://azi.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fcu.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tum.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gbz.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://dim.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwp.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tpk.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uvs.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wpq.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aah.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wkp.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nxv.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kyy.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://llw.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ogv.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xdg.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hzp.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://scg.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://emf.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wyv.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nen.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pjm.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://cmx.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://drx.bbcook.cn

PHP:  number_format(1234567);
来源：http://duk.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tzs.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gzd.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mkt.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sog.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jqa.yonumen.top

C#:   1234567.ToString("N0")
来源：http://oef.epnwcf.com

[E17] 首字母大写
来源：http://zka.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://brh.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dmq.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqd.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lsd.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xio.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ckz.havefunace.top

Ruby: s.capitalize
来源：http://zut.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vxd.wangdashe.top

[E18] 模板占位符替换
来源：http://wav.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://opj.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kpz.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zzw.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zih.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://arl.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ihx.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://svv.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cre.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://hnd.9152youxi.cn

Py:   s.splitlines()
来源：http://gck.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jrr.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://ggo.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://rtv.vehdjk.com

Java: s.lines().toList()
来源：http://ekj.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://gmd.316326.xyz

Ruby: s.lines
来源：http://oxl.hfpthk.cn

C#:   s.Split('\n')
来源：http://yda.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://pot.zdbjq.cn

Py:   if not s:
来源：http://hkj.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvf.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xxx.tian-w.cn

TS:   if (s === "") {}
来源：http://htk.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://byn.jqgufenzy.top

Go:   if s == "" {}
来源：http://gre.yonumen.top

Ruby: if s.empty?
来源：http://vhq.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yec.chenzaomai.com

[E21] 超长截断加省略号
来源：http://xkt.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ois.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zzr.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yar.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nns.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sxy.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://jfg.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yoh.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rks.xinyue.icu

[E22] 字节长度与字符长度
来源：http://nsp.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://csx.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zkw.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://llf.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kky.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mjq.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgo.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://czj.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eie.xinyue.icu

================================================================================
来源：http://zkn.cucudq.cn

F. 文件与目录
来源：http://qli.yongpay.top

================================================================================
来源：http://dmm.tianlin.xyz

[F01] 读取整个文件
来源：http://yis.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nid.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://ncq.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ryi.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aer.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gqe.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://brh.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://maf.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://fiw.sjlbkw.cn

[F02] 逐行读取文件
来源：http://jqn.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jlk.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rho.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dji.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ekq.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ngv.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yfl.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wjt.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dwj.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://vag.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gqc.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mjn.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abs.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eba.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xyl.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rkh.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://ist.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xeg.jiagoushi.top

[F04] 追加写入文件
来源：http://cbv.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ufd.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dvu.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljs.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rpr.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blo.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ilo.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wwi.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rzk.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://gwl.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://poc.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://tcc.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://kaq.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://xnb.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gxs.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jgy.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://wow.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://dlk.yanxiufei.cn

[F06] 删除文件
来源：http://fjk.sxryk.cn

Py:   os.remove("a.txt")
来源：http://zik.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://zcf.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rqi.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://etd.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nmd.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://moi.cashguo.top

Ruby: File.delete("a.txt")
来源：http://iqq.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://gyj.yvedp.cn

[F07] 创建目录（含多级）
来源：http://kcv.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rwe.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ruw.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://egp.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khl.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ood.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hsh.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qif.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ufc.xuetiantiany.cn

[F08] 遍历目录
来源：http://arf.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vds.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tut.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://oae.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://jgi.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vel.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pwc.ivvv.top

Ruby: Dir.children("dir")
来源：http://zqt.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://hsl.tianlin.xyz

[F09] 获取文件大小
来源：http://ufr.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://ysc.hammf.cn

PHP:  filesize("a.txt");
来源：http://zom.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://teo.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://ous.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://czj.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pby.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://cek.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zbf.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://fbi.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nux.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xep.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jrq.cheryme.top

TS:   path.extname("a.txt")
来源：http://pzs.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dmi.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ebp.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lyh.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gdk.dashuyun.cn

[F11] 复制与移动文件
来源：http://kth.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mnc.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zbx.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hsr.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iiv.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rlk.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rut.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jte.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zze.yuxming.cn

[F12] CSV 读写
来源：http://ots.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bhs.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qma.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zfq.shanyushiyangkeji.top

TS:   // 同上
来源：http://unp.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ynf.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gzw.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yxt.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zue.316326.xyz

================================================================================
来源：http://azb.sufxvd.cn

G. 面向对象
来源：http://zod.xuanzx.com

================================================================================
来源：http://ugq.fengsongda.top

[G01] 定义类
来源：http://ugl.zhiwuduotai.top

Py:   class User: pass
来源：http://vlz.hfpthk.cn

PHP:  class User {}
来源：http://nih.cheryme.top

JS:   class User {}
来源：http://tev.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://rwa.zhoulong.xyz

Java: class User {}
来源：http://whw.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://zud.zhongyouzk.top

Ruby: class User; end
来源：http://fbc.shanyushiyangtech.top

C#:   class User {}
来源：http://pzc.c1oappe.top

[G02] 构造函数
来源：http://vei.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://bzl.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://vwg.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://ogu.316326.xyz

TS:   constructor(public name: string) {}
来源：http://dvg.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://eby.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljx.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://uwb.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://fsp.xinyue.icu

[G03] 实例属性
来源：http://aef.bbcook.cn

Py:   self.name = "x"
来源：http://ltt.iojbl.cn

PHP:  public string $name = "x";
来源：http://gdn.yj202588.top

JS:   this.name = "x";
来源：http://ueo.ydjk.org.cn

TS:   name: string = "x";
来源：http://dkl.wangdashe.top

Java: private String name;
来源：http://hjq.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jfp.nanxinkj.top

Ruby: @name = "x"
来源：http://fpq.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://kov.chenzaomai.com

[G04] 定义方法
来源：http://qrx.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://kyw.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vxg.xylfe.cn

JS:   greet() { return this.name; }
来源：http://qab.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://iya.yfazqb.com

Java: String greet() { return name; }
来源：http://qex.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xae.shzxlz.cn

Ruby: def greet; @name; end
来源：http://vym.epnwcf.com

C#:   public string Greet() => Name;
来源：http://dmh.zdbjq.cn

[G05] 继承
来源：http://blv.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://qbp.yfazqb.com

PHP:  class Admin extends User {}
来源：http://qkk.xylfe.cn

JS:   class Admin extends User {}
来源：http://qyg.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://umq.cqqwz.cn

Java: class Admin extends User {}
来源：http://cxa.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rii.52xcode.cn

Ruby: class Admin < User; end
来源：http://vvz.nanxuanxn.top

C#:   class Admin : User {}
来源：http://fpk.zhongyouzk.top

[G06] 重写方法
来源：http://qqv.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://fga.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qzk.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://uno.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://xyx.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://gcl.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://prb.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://pee.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://kyl.epnwcf.com

[G07] 调用父类方法
来源：http://zjg.yuxming.cn

Py:   super().greet()
来源：http://xxi.yonumen.top

PHP:  parent::greet();
来源：http://grx.tarul.cn

JS:   super.greet();
来源：http://qlp.jinghuilouyu.cn

TS:   super.greet();
来源：http://oti.0kj1m.cn

Java: super.greet();
来源：http://smp.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gle.jqgufenzy.top

Ruby: super
来源：http://twf.yonumen.top

C#:   base.Greet();
来源：http://rgi.jlsjyb.cn

[G08] 静态方法与属性
来源：http://enq.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uqt.ydzc1.top

PHP:  public static function f() {}
来源：http://car.pengpengdd.cyou

JS:   static f() {}
来源：http://gfe.jinqigufen.top

TS:   static f(): void {}
来源：http://piz.quarkkingdee.top

Java: static void f() {}
来源：http://vnb.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vsa.yj20258888.top

Ruby: def self.f; end
来源：http://lio.nanxuanxn.top

C#:   public static void F() {}
来源：http://bky.fzhhl.top

[G09] 接口 / 抽象类
来源：http://vpj.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://bcs.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gtw.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nvb.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://pcv.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://wjt.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://pfk.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ehf.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://sln.yfazqb.com

[G10] 访问控制
来源：http://rkh.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://xpo.xziqi.cn

PHP:  public / protected / private
来源：http://chz.tanke756.top

JS:   #private 字段；其余公开
来源：http://ogw.fktsv.cn

TS:   public / protected / private
来源：http://cjg.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://sop.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lnn.andypj.xyz

Ruby: public / protected / private
来源：http://sov.jyoumei.cn

C#:   public / protected / private / internal
来源：http://kwx.uphjek.com

[G11] getter / setter
来源：http://oyv.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://vce.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jud.yj202588.top


<!-- 参考信息 -->