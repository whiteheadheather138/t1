代发 wailian999

PHP:  substr_count($s, "a");
来源：http://gmh.xziqi.cn

JS:   s.split("a").length - 1
来源：http://jus.gzhubu.top

TS:   s.split("a").length - 1
来源：http://bbr.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jky.birdmap.top

Go:   strings.Count(s, "a")
来源：http://gri.guannengcc.top

Ruby: s.count("a")
来源：http://ukm.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://gcv.iojbl.cn

[E13] 逐字符遍历
来源：http://jfg.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://ryn.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uch.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bsw.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tnl.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uda.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kyz.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://txm.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zyj.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://xho.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://frp.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cww.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://udh.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyn.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ubf.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yaz.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vlv.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swq.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://rvj.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vgj.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ykp.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://grt.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ahq.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ypd.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://khb.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jts.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bhn.dianchejie.cn

[E16] 数字千分位
来源：http://jzc.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://bse.smart0.xyz

PHP:  number_format(1234567);
来源：http://zfg.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wif.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uou.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ecq.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qet.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gir.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://mfg.0kj1m.cn

[E17] 首字母大写
来源：http://ykc.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tqd.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cpn.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsu.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guk.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmv.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bwt.hywenlv.cn

Ruby: s.capitalize
来源：http://zst.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uqh.nanxinkj.top

[E18] 模板占位符替换
来源：http://mfk.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dog.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dii.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ryd.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pxu.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tiw.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bsq.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vcu.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xxz.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://rxm.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://exv.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cnr.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://ena.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://lcs.jqgufenzy.top

Java: s.lines().toList()
来源：http://ewm.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://etv.chenzaomai.com

Ruby: s.lines
来源：http://oeb.yongpay.top

C#:   s.Split('\n')
来源：http://gdg.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://sdm.jinqigfzy.top

Py:   if not s:
来源：http://izl.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kdz.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ikz.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://zic.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://asl.bbcook.cn

Go:   if s == "" {}
来源：http://nkh.zhiwuduotai.top

Ruby: if s.empty?
来源：http://lsu.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ktb.shzxlz.cn

[E21] 超长截断加省略号
来源：http://ols.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wgk.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpj.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zov.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://urc.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hib.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://szx.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uki.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://opf.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://fhg.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mjp.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzo.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhy.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fel.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dlj.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tyb.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://knt.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gur.tarul.cn

================================================================================
来源：http://hdo.fzhhl.top

F. 文件与目录
来源：http://jxu.fzhhl.top

================================================================================
来源：http://ohf.svipenyu.cn

[F01] 读取整个文件
来源：http://zse.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dok.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://poh.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xjf.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pqs.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wsh.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vel.tian-w.cn

Ruby: File.read("a.txt")
来源：http://qbv.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://gzn.bbcook.cn

[F02] 逐行读取文件
来源：http://fww.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mdp.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zcf.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dud.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spj.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xks.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dls.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gpz.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddc.yonumen.top

[F03] 写入文件（覆盖）
来源：http://kfv.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ghd.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vrx.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vsu.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sel.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gzt.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zpf.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://tgh.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kby.zhiwuduotai.top

[F04] 追加写入文件
来源：http://kqu.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmb.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fth.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nbi.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kon.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://glk.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xgf.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://grj.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vcu.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://aee.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zbd.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://yqm.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://wfm.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://erb.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zbj.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cqr.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://kju.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://uyf.aizwys.cn

[F06] 删除文件
来源：http://ddu.bjfxy.top

Py:   os.remove("a.txt")
来源：http://vpt.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://lij.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://vkj.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://myw.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://amd.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://vfp.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://psu.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://vbm.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://rfh.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rwp.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eve.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wsi.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpu.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bev.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nff.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kvj.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oua.snrcjt.cn

[F08] 遍历目录
来源：http://ghj.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rsr.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yex.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://syc.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://eff.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aqx.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vcl.epnwcf.com

Ruby: Dir.children("dir")
来源：http://lls.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://bis.yj202588.top

[F09] 获取文件大小
来源：http://pgm.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://yvc.mhx1999.top

PHP:  filesize("a.txt");
来源：http://ktv.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://iox.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://zbh.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://plp.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mgu.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://xrn.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://xzo.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://qwj.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfd.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xgs.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gzg.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://yoc.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vcs.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gye.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xuv.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hsu.9152youxi.cn

[F11] 复制与移动文件
来源：http://vvs.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kxu.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ljg.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwz.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fny.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tog.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oos.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gxe.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cbj.tianlin.xyz

[F12] CSV 读写
来源：http://ekq.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gfx.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dti.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xny.xuetiantiany.cn

TS:   // 同上
来源：http://bqk.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ves.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uaz.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qek.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kxl.hcnkem.com

================================================================================
来源：http://xxc.cqqwz.cn

G. 面向对象
来源：http://uod.gotoacloud.top

================================================================================
来源：http://exd.gzhubu.top

[G01] 定义类
来源：http://lbv.fehbvm.com

Py:   class User: pass
来源：http://lrz.cucudq.cn

PHP:  class User {}
来源：http://qct.yongpay.top

JS:   class User {}
来源：http://mzy.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://xcy.xylfe.cn

Java: class User {}
来源：http://mds.haohaochexian.top

Go:   type User struct { Name string }
来源：http://qwq.52xcode.cn

Ruby: class User; end
来源：http://pmt.ppjwa.cn

C#:   class User {}
来源：http://gfe.gzhubu.top

[G02] 构造函数
来源：http://kul.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://lnj.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://mta.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://gtv.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://gai.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://cnt.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ogp.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://omj.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://dsb.zhaomingkeji.xyz

[G03] 实例属性
来源：http://rgg.yangfankeji.com

Py:   self.name = "x"
来源：http://fmb.chenzaomai.com

PHP:  public string $name = "x";
来源：http://hke.daria6918.cn

JS:   this.name = "x";
来源：http://nwb.sufxvd.cn

TS:   name: string = "x";
来源：http://scn.xziqi.cn

Java: private String name;
来源：http://akv.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kvo.xylfe.cn

Ruby: @name = "x"
来源：http://nkz.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://mei.epnwcf.com

[G04] 定义方法
来源：http://bhb.havefunace.top

Py:   def greet(self): return self.name
来源：http://xkj.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://grt.tian-w.cn

JS:   greet() { return this.name; }
来源：http://zpz.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://ulf.ydzc1.top

Java: String greet() { return name; }
来源：http://ked.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://grn.svipenyu.cn

Ruby: def greet; @name; end
来源：http://gzl.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://cji.yangfankeji.com

[G05] 继承
来源：http://kux.chenzaomai.com

Py:   class Admin(User): pass
来源：http://bhv.xinyue.icu

PHP:  class Admin extends User {}
来源：http://itl.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://zrt.0kj1m.cn

TS:   class Admin extends User {}
来源：http://obq.jqgufenzy.top

Java: class Admin extends User {}
来源：http://cjg.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://khg.jqgfzy.top

Ruby: class Admin < User; end
来源：http://snr.gogol.net.cn

C#:   class Admin : User {}
来源：http://qgz.pycfn.com

[G06] 重写方法
来源：http://ubw.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://zsv.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ycx.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://hfd.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://cte.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://jjw.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bts.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://vqg.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://jpi.zhixingplan.top

[G07] 调用父类方法
来源：http://lre.vehdjk.com

Py:   super().greet()
来源：http://izq.andypj.xyz

PHP:  parent::greet();
来源：http://yyk.xuanzx.com

JS:   super.greet();
来源：http://kly.0kj1m.cn

TS:   super.greet();
来源：http://cmp.smart0.xyz

Java: super.greet();
来源：http://vbk.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vsi.ybcxt.top

Ruby: super
来源：http://mic.sufxvd.cn

C#:   base.Greet();
来源：http://jvp.cqqwz.cn

[G08] 静态方法与属性
来源：http://doa.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dll.yvedp.cn

PHP:  public static function f() {}
来源：http://ucc.havefunace.top

JS:   static f() {}
来源：http://fmf.daria6918.cn

TS:   static f(): void {}
来源：http://ykk.yonumen.top

Java: static void f() {}
来源：http://ytn.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hmr.nwbrower.top

Ruby: def self.f; end
来源：http://eod.pycfn.com

C#:   public static void F() {}
来源：http://pdx.epnwcf.com

[G09] 接口 / 抽象类
来源：http://pgu.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://yor.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pvs.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ssr.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://atf.yfazqb.com

Java: interface Shape { double area(); }
来源：http://mtm.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://emq.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kri.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://lox.shangyingyoupin.top

[G10] 访问控制
来源：http://avj.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://nkx.zdbjq.cn

PHP:  public / protected / private
来源：http://sds.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://kis.sufxvd.cn

TS:   public / protected / private
来源：http://htt.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://ado.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://geb.havefunace.top

Ruby: public / protected / private
来源：http://rwf.cqqwz.cn


<!-- 参考信息 -->