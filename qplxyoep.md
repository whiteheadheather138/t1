代发 wailian999

Ruby: s.reverse
来源：http://joi.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://guk.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://mnt.52xcode.cn

Py:   s.count("a")
来源：http://ogn.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://vlc.xinyue.icu

JS:   s.split("a").length - 1
来源：http://qba.shuidangran.top

TS:   s.split("a").length - 1
来源：http://adu.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cpu.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://gwc.c1oappe.top

Ruby: s.count("a")
来源：http://lmj.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://wwx.zhixingplan.top

[E13] 逐字符遍历
来源：http://lmh.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://hxm.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pal.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aig.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fhp.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nou.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xeu.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fir.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oqa.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://jdv.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oad.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xoe.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bbt.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zdq.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jmy.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://les.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fay.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://poe.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://nkz.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wie.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://thd.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://apj.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://dqu.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lth.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rvg.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://chg.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kjr.iojbl.cn

[E16] 数字千分位
来源：http://cfm.sxryk.cn

Py:   f"{1234567:,}"
来源：http://vnn.yfazqb.com

PHP:  number_format(1234567);
来源：http://ydz.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uuu.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://doo.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbn.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pzq.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rku.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://efq.chenzaomai.com

[E17] 首字母大写
来源：http://csg.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ygt.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vjx.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pdr.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dgi.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uhw.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sdh.316326.xyz

Ruby: s.capitalize
来源：http://cev.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bjr.mhx1999.top

[E18] 模板占位符替换
来源：http://puv.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oap.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://osg.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://omv.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hkn.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xwb.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://non.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rnd.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyk.fehbvm.com

[E19] 多行文本按行拆分
来源：http://ptq.jlsjyb.cn

Py:   s.splitlines()
来源：http://tra.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lbl.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://ccg.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://boa.haohaochexian.top

Java: s.lines().toList()
来源：http://pxo.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://edr.fktsv.cn

Ruby: s.lines
来源：http://pqr.jianghu66.top

C#:   s.Split('\n')
来源：http://tvr.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://rsy.fzhhl.top

Py:   if not s:
来源：http://jda.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bir.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bsr.jinqigfzy.top

TS:   if (s === "") {}
来源：http://ijf.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://kil.dianchejie.cn

Go:   if s == "" {}
来源：http://iwx.gogol.net.cn

Ruby: if s.empty?
来源：http://tji.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hsn.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://ykx.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uaw.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ses.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://coi.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fmp.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jww.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://kai.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mrg.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ian.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://ori.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ybq.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqg.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zch.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ert.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fis.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jmq.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://mhy.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqg.tanke756.top

================================================================================
来源：http://rme.9152youxi.cn

F. 文件与目录
来源：http://yrp.hcnkem.com

================================================================================
来源：http://cbb.wangshuangyany.cn

[F01] 读取整个文件
来源：http://fjg.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mzp.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://lrm.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://trv.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tyy.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://kox.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://axq.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://uyi.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://iuw.yuxming.cn

[F02] 逐行读取文件
来源：http://tel.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://owa.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wut.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hir.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wfr.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eqx.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sqk.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pqy.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://thp.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://zbh.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lbj.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://wri.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://esl.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfl.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iua.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://clf.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://uae.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kti.yanxiufei.cn

[F04] 追加写入文件
来源：http://rxe.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfo.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xrt.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgg.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wol.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gsa.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://web.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://omd.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://frz.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://qzb.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fpn.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://aks.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://udt.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://ard.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://glp.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etn.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://yzi.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://uio.yfazqb.com

[F06] 删除文件
来源：http://mxg.tian-w.cn

Py:   os.remove("a.txt")
来源：http://csx.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://mhh.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yfn.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://pxx.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://psx.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://jhp.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://rxi.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://uhb.redwolf501.top

[F07] 创建目录（含多级）
来源：http://snz.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://frv.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zmx.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gyq.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfb.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zls.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jih.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bfk.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mjt.snrcjt.cn

[F08] 遍历目录
来源：http://qpv.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aob.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sek.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://yei.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://jag.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zom.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xox.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://kly.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://fde.svipenyu.cn

[F09] 获取文件大小
来源：http://gaf.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://luk.yonumen.top

PHP:  filesize("a.txt");
来源：http://usg.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://wcz.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://ygn.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://rtf.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fbh.fktsv.cn

Ruby: File.size("a.txt")
来源：http://kpd.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://lui.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://olu.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nsw.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xei.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aqa.yonumen.top

TS:   path.extname("a.txt")
来源：http://mpd.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bdi.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hyw.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://biu.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xxt.tanke756.top

[F11] 复制与移动文件
来源：http://him.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fhz.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://huk.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqx.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zrc.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bzk.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ohd.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fpo.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mgw.cucudq.cn

[F12] CSV 读写
来源：http://nzj.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ldc.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://alr.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cgi.daria6918.cn

TS:   // 同上
来源：http://swd.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://twe.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://coy.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sxg.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://blu.c1oappe.top

================================================================================
来源：http://ghy.ivvv.top

G. 面向对象
来源：http://yst.feifeiyinyue.top

================================================================================
来源：http://jng.zycfv.cn

[G01] 定义类
来源：http://vva.xuanzx.com

Py:   class User: pass
来源：http://qoz.andypj.xyz

PHP:  class User {}
来源：http://jbg.tanke756.top

JS:   class User {}
来源：http://urd.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://twp.gzhubu.top

Java: class User {}
来源：http://elf.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://yjb.vehdjk.com

Ruby: class User; end
来源：http://est.zhijiandao.cn

C#:   class User {}
来源：http://lxc.gaohongyu789.top

[G02] 构造函数
来源：http://hqw.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://juq.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://fiq.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://oun.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://smd.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://sbv.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bdu.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://bmg.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://gps.bbcook.cn

[G03] 实例属性
来源：http://gei.yuanzhike.top

Py:   self.name = "x"
来源：http://vow.daria6918.cn

PHP:  public string $name = "x";
来源：http://sfa.dashuyun.cn

JS:   this.name = "x";
来源：http://dac.hnqzz.top

TS:   name: string = "x";
来源：http://rlf.svipenyu.cn

Java: private String name;
来源：http://vxs.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ffi.yonumen.top

Ruby: @name = "x"
来源：http://oit.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://uqw.jiagoushi.top

[G04] 定义方法
来源：http://gzc.hnqzz.top

Py:   def greet(self): return self.name
来源：http://oqt.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://clz.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://beu.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://mpb.xylfe.cn

Java: String greet() { return name; }
来源：http://ixo.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://zwi.yuanzhike.top

Ruby: def greet; @name; end
来源：http://qps.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://vab.xylfe.cn

[G05] 继承
来源：http://iys.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://nox.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://igq.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://lgw.aizwys.cn

TS:   class Admin extends User {}
来源：http://crv.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://ikz.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jke.zycfv.cn

Ruby: class Admin < User; end
来源：http://qtv.havefunace.top

C#:   class Admin : User {}
来源：http://nzp.sweek.top

[G06] 重写方法
来源：http://dbh.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://etg.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vwf.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://xkh.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://imb.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://zeh.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mys.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://piv.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://qjp.pycfn.com

[G07] 调用父类方法
来源：http://ggv.redwolf501.top

Py:   super().greet()
来源：http://vgf.zdbjq.cn

PHP:  parent::greet();
来源：http://eeu.hcnkem.com

JS:   super.greet();
来源：http://opi.dashuyun.cn

TS:   super.greet();
来源：http://syd.smart0.xyz

Java: super.greet();
来源：http://uqe.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gli.mhx1999.top

Ruby: super
来源：http://lya.hesvh.cn

C#:   base.Greet();
来源：http://rbo.dianchejie.cn

[G08] 静态方法与属性
来源：http://ktz.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jsq.zhoulong.xyz

PHP:  public static function f() {}
来源：http://ooz.tarul.cn

JS:   static f() {}
来源：http://zvp.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://gmx.bjfxy.top

Java: static void f() {}
来源：http://hxp.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://crf.xuetiantiany.cn

Ruby: def self.f; end
来源：http://dup.hysaishi.cn

C#:   public static void F() {}
来源：http://xay.pycfn.com

[G09] 接口 / 抽象类
来源：http://rwm.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://gfp.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://pog.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qxu.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://qhl.yvedp.cn

Java: interface Shape { double area(); }
来源：http://lno.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://wkt.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sri.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://zoq.shangyingyoupin.top

[G10] 访问控制
来源：http://ggc.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://hcg.zdbjq.cn

PHP:  public / protected / private
来源：http://qhi.gzhubu.top

JS:   #private 字段；其余公开
来源：http://fmf.nwbrower.top


<!-- 参考信息 -->