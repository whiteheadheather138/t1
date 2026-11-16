代发 wailian999

Go:   strings.Count(s, "a")
来源：http://qey.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://lbt.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://brh.zhijiandao.cn

[E13] 逐字符遍历
来源：http://mzp.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://cmb.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rcg.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://atu.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rnt.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tgl.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://evj.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kwt.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sza.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://zct.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpa.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kau.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ago.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mmg.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nxy.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tvn.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wtj.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lui.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://csv.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gke.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://whg.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://clm.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mfm.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://veg.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://afa.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kse.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eun.cashguo.top

[E16] 数字千分位
来源：http://deq.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://fgn.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://bjz.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zty.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://thf.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://saw.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://roi.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zha.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://xak.feifeiyinyue.top

[E17] 首字母大写
来源：http://jhb.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xis.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gju.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mgw.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pky.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://owo.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ymh.hnxiangtu.top

Ruby: s.capitalize
来源：http://oyf.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kci.ppjwa.cn

[E18] 模板占位符替换
来源：http://aqy.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://apt.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cpo.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tey.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://epr.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://myo.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zbc.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xuk.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sew.tarul.cn

[E19] 多行文本按行拆分
来源：http://pzy.jyoumei.cn

Py:   s.splitlines()
来源：http://shl.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kai.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://uqt.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://wfy.snrcjt.cn

Java: s.lines().toList()
来源：http://hhn.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://sad.zycfv.cn

Ruby: s.lines
来源：http://sym.yuanzhike.top

C#:   s.Split('\n')
来源：http://sww.yvedp.cn

[E20] 判断字符串是否为空
来源：http://pki.yongpay.top

Py:   if not s:
来源：http://mbz.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpc.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tkz.sweek.top

TS:   if (s === "") {}
来源：http://myr.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://zno.iojbl.cn

Go:   if s == "" {}
来源：http://gag.andypj.xyz

Ruby: if s.empty?
来源：http://fdz.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eql.ppjwa.cn

[E21] 超长截断加省略号
来源：http://fua.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rlj.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://obz.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogi.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdp.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dlj.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://fpf.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aqo.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hmu.ybcxt.top

[E22] 字节长度与字符长度
来源：http://cyu.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ctu.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://afp.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yls.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fyk.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vtq.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://stw.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://lro.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nko.hammf.cn

================================================================================
来源：http://crh.ctjpmb.com

F. 文件与目录
来源：http://dnc.52xcode.cn

================================================================================
来源：http://ivr.hnqzz.top

[F01] 读取整个文件
来源：http://lfo.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qzc.meibo888.top

PHP:  file_get_contents("a.txt");
来源：http://dxe.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://npc.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bwb.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pte.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lxh.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://dhz.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://wei.ppjwa.cn

[F02] 逐行读取文件
来源：http://eko.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pbl.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dee.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lak.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgk.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://phw.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xcd.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bjk.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mti.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://dvh.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://igu.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gps.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovg.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bty.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://str.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://obo.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://ayz.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sql.iojbl.cn

[F04] 追加写入文件
来源：http://ful.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jvl.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sfs.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sti.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebu.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lza.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dsj.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://czz.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tcy.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://ytd.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oky.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://ggr.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://ibl.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://coo.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vht.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pew.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://wxg.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://kdz.zhongyouzk.top

[F06] 删除文件
来源：http://rsf.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://bpm.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://bmr.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://osx.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://jsw.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wdc.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://fml.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://ahg.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://zqb.vehdjk.com

[F07] 创建目录（含多级）
来源：http://odf.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mme.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vwk.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbr.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://amk.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ebp.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://scv.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgd.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lvj.sweek.top

[F08] 遍历目录
来源：http://mqz.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ibf.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zfw.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://bms.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://xjl.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://thb.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ihr.316326.xyz

Ruby: Dir.children("dir")
来源：http://nra.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://ngy.sjlbkw.cn

[F09] 获取文件大小
来源：http://kqs.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://rmh.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://zfj.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://wtz.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://mue.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yxk.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bkw.yvedp.cn

Ruby: File.size("a.txt")
来源：http://nqp.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://xus.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://qce.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jxt.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wut.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ayz.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://cyx.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vej.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ixp.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ftp.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cbg.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://ogh.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rme.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dph.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eyi.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://izy.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rmq.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yux.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kjg.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sji.tarul.cn

[F12] CSV 读写
来源：http://hfq.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nge.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://umu.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wfc.52xcode.cn

TS:   // 同上
来源：http://ljm.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iru.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://spw.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://haa.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wwh.jinqigufen.top

================================================================================
来源：http://bba.guowangkeji.top

G. 面向对象
来源：http://kup.tarul.cn

================================================================================
来源：http://mgr.0kj1m.cn

[G01] 定义类
来源：http://fde.yj20258.top

Py:   class User: pass
来源：http://dca.havefunace.top

PHP:  class User {}
来源：http://kfn.vehdjk.com

JS:   class User {}
来源：http://yvl.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://anz.svipenyu.cn

Java: class User {}
来源：http://its.sufxvd.cn

Go:   type User struct { Name string }
来源：http://mfb.yangfankeji.com

Ruby: class User; end
来源：http://cof.shzxlz.cn

C#:   class User {}
来源：http://cvg.shzxlz.cn

[G02] 构造函数
来源：http://vgt.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://qgr.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://pte.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://vbd.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://zio.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://uac.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jpq.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://kro.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://ebg.tanke756.top

[G03] 实例属性
来源：http://ans.redwolf501.top

Py:   self.name = "x"
来源：http://ema.cqqwz.cn

PHP:  public string $name = "x";
来源：http://psq.pycfn.com

JS:   this.name = "x";
来源：http://jao.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://kvj.meibo888.top

Java: private String name;
来源：http://kdu.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jjt.hywenlv.cn

Ruby: @name = "x"
来源：http://lfn.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://xux.jinqigfzy.top

[G04] 定义方法
来源：http://ibi.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://cgg.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hrg.yonumen.top

JS:   greet() { return this.name; }
来源：http://nxz.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://otz.jiagoushi.top

Java: String greet() { return name; }
来源：http://dlx.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lac.wangdashe.top

Ruby: def greet; @name; end
来源：http://oge.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://rof.hesvh.cn

[G05] 继承
来源：http://tlu.aibaodan.cn

Py:   class Admin(User): pass
来源：http://wrz.hnqzz.top

PHP:  class Admin extends User {}
来源：http://wsk.bbcook.cn

JS:   class Admin extends User {}
来源：http://eix.ybcxt.top

TS:   class Admin extends User {}
来源：http://usw.epnwcf.com

Java: class Admin extends User {}
来源：http://rus.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ymu.cheryme.top

Ruby: class Admin < User; end
来源：http://psh.fehbvm.com

C#:   class Admin : User {}
来源：http://mvt.wangdashe.top

[G06] 重写方法
来源：http://tra.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://svh.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gui.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://mit.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://dbf.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://bkx.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jaq.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://idf.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://efe.hywenlv.cn

[G07] 调用父类方法
来源：http://seb.vqdsnc.cn

Py:   super().greet()
来源：http://zsg.ehwqpu.com

PHP:  parent::greet();
来源：http://feu.yangfankeji.com

JS:   super.greet();
来源：http://xkq.yvedp.cn

TS:   super.greet();
来源：http://jci.fzhhl.top

Java: super.greet();
来源：http://cqd.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eke.hesvh.cn

Ruby: super
来源：http://bav.yj202588.top

C#:   base.Greet();
来源：http://can.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://zcy.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cqb.tianlin.xyz

PHP:  public static function f() {}
来源：http://ukf.hywenlv.cn

JS:   static f() {}
来源：http://kdp.feifeiyinyue.top

TS:   static f(): void {}
来源：http://csd.c1oappe.top

Java: static void f() {}
来源：http://pgh.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://mys.zhongyouzk.top

Ruby: def self.f; end
来源：http://sfi.smart0.xyz

C#:   public static void F() {}
来源：http://rrs.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://upm.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://vun.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://lyj.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uku.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://ziu.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://bfx.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://qdl.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vie.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://rlc.sysykeji.top

[G10] 访问控制
来源：http://hqr.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://lmx.9152youxi.cn

PHP:  public / protected / private
来源：http://kdh.c1oappe.top

JS:   #private 字段；其余公开
来源：http://uce.0kj1m.cn

TS:   public / protected / private
来源：http://mji.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://vde.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rwb.wangshuangyany.cn

Ruby: public / protected / private
来源：http://mff.ctjpmb.com

C#:   public / protected / private / internal
来源：http://vvn.shuidangran.top

[G11] getter / setter
来源：http://zoa.andypj.xyz

Py:   @property 与 @x.setter
来源：http://nry.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nlo.meibo888.top


<!-- 参考信息 -->