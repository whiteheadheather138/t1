代发 wailian999

Ruby: s.reverse
来源：http://xur.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://nou.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://xxj.jiagoushi.top

Py:   s.count("a")
来源：http://bwz.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://nnp.fktsv.cn

JS:   s.split("a").length - 1
来源：http://jiq.daria6918.cn

TS:   s.split("a").length - 1
来源：http://hdk.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yuq.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://mng.cheryme.top

Ruby: s.count("a")
来源：http://zzd.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://yws.yj20258888.top

[E13] 逐字符遍历
来源：http://awt.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://oor.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wsg.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://diu.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxt.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aux.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fpf.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://crf.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bri.316326.xyz

[E14] URL 编码与 Base64
来源：http://xea.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://egx.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qus.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gwj.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xlj.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dbr.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fws.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://foz.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://alj.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://vhu.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://lof.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mse.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ucj.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xyj.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://slh.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cdy.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nbv.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://msm.cdnleiting.top

[E16] 数字千分位
来源：http://wuo.fzhhl.top

Py:   f"{1234567:,}"
来源：http://pfl.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://yci.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rwf.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mnt.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cwv.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gfp.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tiz.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://zvm.ydzc1.top

[E17] 首字母大写
来源：http://xnh.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qii.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://abi.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcu.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ici.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fag.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://swe.sweek.top

Ruby: s.capitalize
来源：http://xjw.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cug.jqgufenzy.top

[E18] 模板占位符替换
来源：http://xxz.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mpd.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zvw.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://etz.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ilv.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aeh.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://phy.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uhh.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sfl.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://ywd.fengsongda.top

Py:   s.splitlines()
来源：http://cdn.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trl.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://xch.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://dtc.bjfxy.top

Java: s.lines().toList()
来源：http://ceu.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://hdi.yanxiufei.cn

Ruby: s.lines
来源：http://xyu.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://gwk.yj20258.top

[E20] 判断字符串是否为空
来源：http://jmw.sysykeji.top

Py:   if not s:
来源：http://dhm.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qtd.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ljv.ppjwa.cn

TS:   if (s === "") {}
来源：http://vln.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://ofy.ppjwa.cn

Go:   if s == "" {}
来源：http://ejg.sxryk.cn

Ruby: if s.empty?
来源：http://ydv.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gla.aizwys.cn

[E21] 超长截断加省略号
来源：http://vnu.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://byz.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mbd.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bgx.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xir.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vsb.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://knt.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vcx.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nhs.xylfe.cn

[E22] 字节长度与字符长度
来源：http://ite.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://luf.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gqf.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzn.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbq.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jai.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ggc.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://ptv.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vbu.9152youxi.cn

================================================================================
来源：http://zcp.hcnkem.com

F. 文件与目录
来源：http://xey.jinyuanbaomall.cn

================================================================================
来源：http://ein.vqdsnc.cn

[F01] 读取整个文件
来源：http://jwv.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pnb.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://bql.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ubl.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpe.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dqv.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lwv.chenzaomai.com

Ruby: File.read("a.txt")
来源：http://qdk.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ocx.tianlin.xyz

[F02] 逐行读取文件
来源：http://gkx.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xlk.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://shu.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nzu.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxn.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tbh.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wep.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zci.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://onc.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://vdd.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://thf.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cex.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nrx.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nxx.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jhq.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ene.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://swh.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zys.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://ffa.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ggo.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xaq.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvd.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sia.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cbo.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxh.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yxt.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ppf.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://cyc.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ivq.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://gkz.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://ocb.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://jai.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ipy.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://duz.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://lve.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://nzt.sysykeji.top

[F06] 删除文件
来源：http://rse.cashguo.top

Py:   os.remove("a.txt")
来源：http://ond.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://nfo.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ckk.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://trw.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mzd.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://gbr.tanke756.top

Ruby: File.delete("a.txt")
来源：http://cvr.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://rln.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://kbh.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ftq.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kld.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mtp.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwc.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://plm.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lsd.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://evj.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zrc.gaohongyu789.top

[F08] 遍历目录
来源：http://kdj.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wds.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://for.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://gcc.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://mnc.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bex.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://bhq.havefunace.top

Ruby: Dir.children("dir")
来源：http://dug.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://rey.yonumen.top

[F09] 获取文件大小
来源：http://ciq.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://kyr.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://xfg.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://zvh.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://ole.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ijz.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uzo.ydzc1.top

Ruby: File.size("a.txt")
来源：http://tgs.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://ywl.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://dhl.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://clx.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eqr.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gsw.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://ldu.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wfp.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bfg.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vgx.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yrz.aibaodan.cn

[F11] 复制与移动文件
来源：http://azm.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wvt.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kix.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ndu.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dct.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fdj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hyj.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qkh.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ldp.tarul.cn

[F12] CSV 读写
来源：http://vxr.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xfu.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ldr.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijq.sweek.top

TS:   // 同上
来源：http://rxw.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ibu.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mlg.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dxh.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gix.hnxiangtu.top

================================================================================
来源：http://xsu.jqgfzy.top

G. 面向对象
来源：http://htg.jlsjyb.cn

================================================================================
来源：http://lad.chenlongwang.top

[G01] 定义类
来源：http://krk.jlsjyb.cn

Py:   class User: pass
来源：http://ezp.snrcjt.cn

PHP:  class User {}
来源：http://olk.daria6918.cn

JS:   class User {}
来源：http://jfh.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://fqu.yfazqb.com

Java: class User {}
来源：http://imn.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://ozz.shanyushiyangkeji.top

Ruby: class User; end
来源：http://wdi.hywenlv.cn

C#:   class User {}
来源：http://ere.jinqigfzy.top

[G02] 构造函数
来源：http://ojc.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://scs.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://koe.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://ucw.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://zyi.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://qrs.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gah.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://nsa.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://dyn.sxryk.cn

[G03] 实例属性
来源：http://jml.zhengqikj.top

Py:   self.name = "x"
来源：http://ruy.hcnkem.com

PHP:  public string $name = "x";
来源：http://wcq.birdmap.top

JS:   this.name = "x";
来源：http://mee.0kj1m.cn

TS:   name: string = "x";
来源：http://dre.yj20258888.top

Java: private String name;
来源：http://qxt.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gvx.cheryme.top

Ruby: @name = "x"
来源：http://ltw.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://jnj.nanxinkj.top

[G04] 定义方法
来源：http://yhx.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://bxn.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ixk.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://uaz.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://nvw.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://woq.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cif.aibaodan.cn

Ruby: def greet; @name; end
来源：http://vpi.fengsongda.top

C#:   public string Greet() => Name;
来源：http://pnf.havefunace.top

[G05] 继承
来源：http://bny.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://krq.cashguo.top

PHP:  class Admin extends User {}
来源：http://ouv.hesvh.cn

JS:   class Admin extends User {}
来源：http://hwr.hysaishi.cn

TS:   class Admin extends User {}
来源：http://adu.haohaochexian.top

Java: class Admin extends User {}
来源：http://bdy.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zyw.bbcook.cn

Ruby: class Admin < User; end
来源：http://bgv.9152youxi.cn

C#:   class Admin : User {}
来源：http://ktx.jiagoushi.top

[G06] 重写方法
来源：http://mwn.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://wkv.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://uyp.yj202588.top

JS:   greet() { return "admin"; }
来源：http://qnn.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://ozc.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://qml.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tcm.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://yhm.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://qeg.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://obv.jlsjyb.cn

Py:   super().greet()
来源：http://gdj.birdmap.top

PHP:  parent::greet();
来源：http://zoy.tanke756.top

JS:   super.greet();
来源：http://rpk.hesvh.cn

TS:   super.greet();
来源：http://yry.zhixingplan.top

Java: super.greet();
来源：http://giz.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cui.hammf.cn

Ruby: super
来源：http://ohg.0kj1m.cn

C#:   base.Greet();
来源：http://gqf.snrcjt.cn

[G08] 静态方法与属性
来源：http://lmw.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ufa.yueranfly.top

PHP:  public static function f() {}
来源：http://dst.quarkkingdee.top

JS:   static f() {}
来源：http://aau.zdbjq.cn

TS:   static f(): void {}
来源：http://lla.yuxming.cn

Java: static void f() {}
来源：http://kkf.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://skz.svipenyu.cn

Ruby: def self.f; end
来源：http://nyw.shuidangran.top

C#:   public static void F() {}
来源：http://wxu.tarul.cn

[G09] 接口 / 抽象类
来源：http://kca.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://mxw.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://lsi.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pyb.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://zca.gzhubu.top

Java: interface Shape { double area(); }
来源：http://xtf.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://knr.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://npj.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://pha.meibo888.top

[G10] 访问控制
来源：http://rcs.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://ugj.sweek.top

PHP:  public / protected / private
来源：http://ipa.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://pyo.xuetiantiany.cn


<!-- 参考信息 -->