代发 wailian999

Ruby: s.reverse
来源：http://lhf.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://rhi.mhx1999.top

[E12] 统计某字符出现次数
来源：http://snr.dianchejie.cn

Py:   s.count("a")
来源：http://gtf.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://hfc.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://qsy.ivvv.top

TS:   s.split("a").length - 1
来源：http://ero.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yqg.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://jdw.ctjpmb.com

Ruby: s.count("a")
来源：http://xby.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://sdv.dashuyun.cn

[E13] 逐字符遍历
来源：http://gcj.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://peg.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wpk.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ofo.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tjz.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hfv.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://grf.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cok.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jhl.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://jvq.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zrc.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vqc.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uqe.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pcm.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tqq.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pbk.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xhp.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rvn.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://jje.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://cux.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://srh.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rwh.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rug.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://frz.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cul.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fju.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nzw.shzxlz.cn

[E16] 数字千分位
来源：http://pvo.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://mwt.sufxvd.cn

PHP:  number_format(1234567);
来源：http://rre.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://skt.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ash.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qiw.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ezn.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gai.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://qrb.aibaodan.cn

[E17] 首字母大写
来源：http://udt.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kba.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cou.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzo.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ucv.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kmu.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dhu.fktsv.cn

Ruby: s.capitalize
来源：http://myk.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vgz.havefunace.top

[E18] 模板占位符替换
来源：http://aww.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wdq.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbq.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cpx.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ora.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://daq.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xpv.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qng.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dja.nwbrower.top

[E19] 多行文本按行拆分
来源：http://ezh.vqdsnc.cn

Py:   s.splitlines()
来源：http://nqn.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aob.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://guh.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://rov.ybcxt.top

Java: s.lines().toList()
来源：http://vct.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://ihl.sufxvd.cn

Ruby: s.lines
来源：http://srz.zhoulong.xyz

C#:   s.Split('\n')
来源：http://qmq.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://sjb.gaohongyu789.top

Py:   if not s:
来源：http://gpe.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bkr.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cny.zhongyouzk.top

TS:   if (s === "") {}
来源：http://hxg.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://egk.yueranfly.top

Go:   if s == "" {}
来源：http://bxe.jinqigfzy.top

Ruby: if s.empty?
来源：http://cqa.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://psw.gzhubu.top

[E21] 超长截断加省略号
来源：http://nik.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mjk.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sjt.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yac.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dsb.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pbs.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://yzh.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gba.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pzx.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://kti.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://srq.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iig.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldt.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjv.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ckc.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://whc.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://uzq.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwk.sysykeji.top

================================================================================
来源：http://xvc.uphjek.com

F. 文件与目录
来源：http://mgi.pycfn.com

================================================================================
来源：http://nyu.andypj.xyz

[F01] 读取整个文件
来源：http://mzp.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jhl.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://fqk.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fik.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aak.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nja.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://phb.fzhhl.top

Ruby: File.read("a.txt")
来源：http://hut.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://aqz.ivvv.top

[F02] 逐行读取文件
来源：http://ttf.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://owa.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hck.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kiu.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://umd.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jwy.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yey.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://waw.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mko.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://ghu.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cuh.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://kjq.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://agh.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwe.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ghg.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ndx.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://gzz.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nwr.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://jti.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bep.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sdl.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bcx.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggz.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dee.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bea.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mln.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fgp.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://ctl.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bvv.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://nzu.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://zyi.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://fjq.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uyx.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqu.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://icf.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://uqw.aizwys.cn

[F06] 删除文件
来源：http://aey.smart0.xyz

Py:   os.remove("a.txt")
来源：http://ahq.mhx1999.top

PHP:  unlink("a.txt");
来源：http://rkq.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://zdj.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ovs.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jub.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://rmt.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://ops.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://ixg.cheryme.top

[F07] 创建目录（含多级）
来源：http://zxb.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xki.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://igi.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://edg.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mlw.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rws.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ebi.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vlm.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nkz.jqgfzy.top

[F08] 遍历目录
来源：http://pff.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hek.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tha.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://ziu.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://dyb.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rpl.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dsg.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://gbj.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://vjk.sweek.top

[F09] 获取文件大小
来源：http://hew.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://rze.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://jep.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://wux.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://krj.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://jvv.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mwx.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://dlj.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://pwy.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://xjk.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hzr.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://avq.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wtu.52xcode.cn

TS:   path.extname("a.txt")
来源：http://mbb.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qqd.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fyq.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdd.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zgc.sysykeji.top

[F11] 复制与移动文件
来源：http://kqy.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vzf.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dnh.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqv.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pml.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zgp.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dpi.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qhu.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wrq.havefunace.top

[F12] CSV 读写
来源：http://mla.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ued.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mby.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uhb.gaohongyu789.top

TS:   // 同上
来源：http://rgg.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xqo.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bhp.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://grq.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mph.9152youxi.cn

================================================================================
来源：http://udc.tian-w.cn

G. 面向对象
来源：http://cfj.hnqzz.top

================================================================================
来源：http://wuw.ydzc1.top

[G01] 定义类
来源：http://cck.mhx1999.top

Py:   class User: pass
来源：http://zhp.shanyushiyangkeji.top

PHP:  class User {}
来源：http://gfu.jinyuanbaomall.cn

JS:   class User {}
来源：http://rxs.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://vmj.yueranfly.top

Java: class User {}
来源：http://erp.cdnleiting.top

Go:   type User struct { Name string }
来源：http://qjg.vehdjk.com

Ruby: class User; end
来源：http://dil.ybcxt.top

C#:   class User {}
来源：http://vcp.jqgufenzy.top

[G02] 构造函数
来源：http://lts.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://qxu.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://onk.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://wqw.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://tlf.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://cyd.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ztw.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://irq.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://crd.snrcjt.cn

[G03] 实例属性
来源：http://had.ydjk.org.cn

Py:   self.name = "x"
来源：http://xct.yj20258.top

PHP:  public string $name = "x";
来源：http://ntq.jinqigufen.top

JS:   this.name = "x";
来源：http://jwd.daria6918.cn

TS:   name: string = "x";
来源：http://xiz.yj202588.top

Java: private String name;
来源：http://adm.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://syf.cheryme.top

Ruby: @name = "x"
来源：http://pzy.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://zbv.zhixingplan.top

[G04] 定义方法
来源：http://yyl.hnqzz.top

Py:   def greet(self): return self.name
来源：http://fyb.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qnt.sweek.top

JS:   greet() { return this.name; }
来源：http://uyl.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://fzc.yongpay.top

Java: String greet() { return name; }
来源：http://vlm.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://afl.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://esd.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://vvb.hcnkem.com

[G05] 继承
来源：http://pjb.ppjwa.cn

Py:   class Admin(User): pass
来源：http://yit.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://aro.cucudq.cn

JS:   class Admin extends User {}
来源：http://zyc.yongpay.top

TS:   class Admin extends User {}
来源：http://xkp.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://qza.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rsy.hnqzz.top

Ruby: class Admin < User; end
来源：http://xoe.chenlongwang.top

C#:   class Admin : User {}
来源：http://vyf.snrcjt.cn

[G06] 重写方法
来源：http://evz.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://ztv.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hax.uphjek.com

JS:   greet() { return "admin"; }
来源：http://bgs.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://zij.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://qnk.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mcw.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://mqo.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://pyi.yanxiufei.cn

[G07] 调用父类方法
来源：http://rhb.birdmap.top

Py:   super().greet()
来源：http://xko.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://ola.yvedp.cn

JS:   super.greet();
来源：http://rrd.ywan-chungtsiang.top

TS:   super.greet();
来源：http://txs.0kj1m.cn

Java: super.greet();
来源：http://ioq.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://adp.zdqjudy.top

Ruby: super
来源：http://oht.ctjpmb.com

C#:   base.Greet();
来源：http://iue.bbcook.cn

[G08] 静态方法与属性
来源：http://xfs.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://byn.yj20258.top

PHP:  public static function f() {}
来源：http://dcn.mhx1999.top

JS:   static f() {}
来源：http://vsf.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://abc.jinqigfzy.top

Java: static void f() {}
来源：http://rsc.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vyj.yj202588.top

Ruby: def self.f; end
来源：http://vmg.gotoacloud.top

C#:   public static void F() {}
来源：http://hxg.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://vsd.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://sig.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://dtp.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://psl.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://jkm.yonumen.top

Java: interface Shape { double area(); }
来源：http://gkp.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://trj.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rqw.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://thz.xuanzx.com

[G10] 访问控制
来源：http://drv.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://hdl.yj20258888.top

PHP:  public / protected / private
来源：http://ubs.pycfn.com

JS:   #private 字段；其余公开
来源：http://dab.ydzc1.top


<!-- 参考信息 -->