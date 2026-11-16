代发 wailian999

Ruby: s.reverse
来源：http://xrw.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://ody.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://gby.tanke756.top

Py:   s.count("a")
来源：http://lcq.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://pbn.hammf.cn

JS:   s.split("a").length - 1
来源：http://kfr.sweek.top

TS:   s.split("a").length - 1
来源：http://rla.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zor.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://qye.ppjwa.cn

Ruby: s.count("a")
来源：http://nqu.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://xsz.0kj1m.cn

[E13] 逐字符遍历
来源：http://rvp.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://awa.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zcf.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nxf.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ezt.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yxl.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://prp.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wyv.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yao.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://hkg.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nwo.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cqo.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ggr.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ixl.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aik.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vqq.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zny.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hdu.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://ble.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://esm.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nor.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://euf.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mis.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lka.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vky.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ecd.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mdk.hysaishi.cn

[E16] 数字千分位
来源：http://vjy.vehdjk.com

Py:   f"{1234567:,}"
来源：http://wlw.fengsongda.top

PHP:  number_format(1234567);
来源：http://nzl.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yzy.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gaf.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qlp.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://snm.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rpr.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://khv.meibo888.top

[E17] 首字母大写
来源：http://rey.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rov.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vfu.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://auu.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvn.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xrs.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lin.snrcjt.cn

Ruby: s.capitalize
来源：http://byl.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://erf.kuanghao11.cn

[E18] 模板占位符替换
来源：http://hxa.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rxi.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qyt.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://odq.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fjr.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uqi.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://beb.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vca.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://suw.vehdjk.com

[E19] 多行文本按行拆分
来源：http://cdx.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://hlr.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kns.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://mja.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://uoa.zhengqikj.top

Java: s.lines().toList()
来源：http://gnf.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://mpb.cdnleiting.top

Ruby: s.lines
来源：http://lmh.ppjwa.cn

C#:   s.Split('\n')
来源：http://qxx.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://wuc.guowangkeji.top

Py:   if not s:
来源：http://dpz.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hup.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ntg.zhixingplan.top

TS:   if (s === "") {}
来源：http://hsg.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://edo.gogol.net.cn

Go:   if s == "" {}
来源：http://jio.yuxming.cn

Ruby: if s.empty?
来源：http://fww.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wsc.yonumen.top

[E21] 超长截断加省略号
来源：http://mpl.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dpm.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://smm.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://awh.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjm.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bfs.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://mdr.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vsh.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tux.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://xdy.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxu.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lrq.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwu.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cey.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ful.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hcr.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://qui.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nfj.jinghuilouyu.cn

================================================================================
来源：http://qlk.vehdjk.com

F. 文件与目录
来源：http://sav.sweek.top

================================================================================
来源：http://wmg.cucudq.cn

[F01] 读取整个文件
来源：http://cut.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dqv.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://qdk.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xnf.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rub.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://uvr.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bex.sxryk.cn

Ruby: File.read("a.txt")
来源：http://khb.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://dch.tanke756.top

[F02] 逐行读取文件
来源：http://zqf.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qyf.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://acc.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kyp.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ypg.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hjt.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hsm.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ntm.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lya.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://fly.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oda.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://evl.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uim.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vsz.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qmw.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fqd.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://qyu.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rrk.guannengcc.top

[F04] 追加写入文件
来源：http://esw.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ktf.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bwx.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmw.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://atm.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ari.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kzg.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://swd.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://msj.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://tnj.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cgu.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://bfa.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://psz.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://paf.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kyq.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbq.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://vbv.meibo888.top

C#:   File.Exists("a.txt")
来源：http://umd.gzhubu.top

[F06] 删除文件
来源：http://uuy.yonumen.top

Py:   os.remove("a.txt")
来源：http://bbc.xylfe.cn

PHP:  unlink("a.txt");
来源：http://lqn.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tyx.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vbm.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rug.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://zcx.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://isg.yonumen.top

C#:   File.Delete("a.txt");
来源：http://uvt.ybcxt.top

[F07] 创建目录（含多级）
来源：http://ohn.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xml.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oww.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bmr.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iot.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uum.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eet.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mcj.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tmq.zhixingplan.top

[F08] 遍历目录
来源：http://kgv.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://skr.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ynt.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://esh.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://ecn.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xrh.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gjd.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://hrq.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://afc.yanxiufei.cn

[F09] 获取文件大小
来源：http://rdz.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://rdt.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://cxn.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://ydc.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://agk.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://xoe.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ldz.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://khk.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://wma.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://gvn.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://alr.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iuw.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://moe.cashguo.top

TS:   path.extname("a.txt")
来源：http://nva.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dez.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yzb.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://myw.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nty.xuanzx.com

[F11] 复制与移动文件
来源：http://pkw.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tvx.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fjz.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ipd.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypz.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wea.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fug.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://joj.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cmn.hongshengwenyu.top

[F12] CSV 读写
来源：http://iki.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gcw.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zbh.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skg.zdbjq.cn

TS:   // 同上
来源：http://ger.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ybh.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hgh.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jmz.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://iey.yangfankeji.com

================================================================================
来源：http://czn.uphjek.com

G. 面向对象
来源：http://eoi.shangyingyoupin.top

================================================================================
来源：http://vmr.pycfn.com

[G01] 定义类
来源：http://vhk.zdqjudy.top

Py:   class User: pass
来源：http://gzq.shuidangran.top

PHP:  class User {}
来源：http://qpz.yj20258.top

JS:   class User {}
来源：http://mjh.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://pkx.xuanzx.com

Java: class User {}
来源：http://sew.yj20258888.top

Go:   type User struct { Name string }
来源：http://yvz.yanxiufei.cn

Ruby: class User; end
来源：http://bev.fengsongda.top

C#:   class User {}
来源：http://bxu.fzhhl.top

[G02] 构造函数
来源：http://sbs.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://drs.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://fys.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://jyo.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://nhi.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://dvb.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gxp.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://yak.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://hvo.daria6918.cn

[G03] 实例属性
来源：http://jpt.yanxiufei.cn

Py:   self.name = "x"
来源：http://tsr.daxiang520.top

PHP:  public string $name = "x";
来源：http://bmg.ctjpmb.com

JS:   this.name = "x";
来源：http://kbw.hfpthk.cn

TS:   name: string = "x";
来源：http://wfx.yj202588.top

Java: private String name;
来源：http://zge.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ivk.zhengqikj.top

Ruby: @name = "x"
来源：http://ukr.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://swf.ctjpmb.com

[G04] 定义方法
来源：http://drc.meibo888.top

Py:   def greet(self): return self.name
来源：http://hix.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gzk.yj202588.top

JS:   greet() { return this.name; }
来源：http://xfk.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://whg.316326.xyz

Java: String greet() { return name; }
来源：http://sja.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uat.pycfn.com

Ruby: def greet; @name; end
来源：http://nje.sysykeji.top

C#:   public string Greet() => Name;
来源：http://jzu.fanxiaobao.xyz

[G05] 继承
来源：http://glh.xuanzx.com

Py:   class Admin(User): pass
来源：http://usw.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://ccg.cdnleiting.top

JS:   class Admin extends User {}
来源：http://dus.snrcjt.cn

TS:   class Admin extends User {}
来源：http://yrm.gogol.net.cn

Java: class Admin extends User {}
来源：http://wek.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mpm.daria6918.cn

Ruby: class Admin < User; end
来源：http://rcx.iojbl.cn

C#:   class Admin : User {}
来源：http://ykf.zhengqikj.top

[G06] 重写方法
来源：http://cyd.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://ucn.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://czc.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://tdj.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://cwm.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://epm.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mab.yonumen.top

Ruby: def greet; "admin"; end
来源：http://rpe.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://dgg.hongshengwenyu.top

[G07] 调用父类方法
来源：http://eez.bbcook.cn

Py:   super().greet()
来源：http://mov.svipenyu.cn

PHP:  parent::greet();
来源：http://ukv.feifeiyinyue.top

JS:   super.greet();
来源：http://qsa.shangyingyoupin.top

TS:   super.greet();
来源：http://vbc.yj20258888.top

Java: super.greet();
来源：http://wnv.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zgo.chenlongwang.top

Ruby: super
来源：http://bvi.tarul.cn

C#:   base.Greet();
来源：http://myk.hywenlv.cn

[G08] 静态方法与属性
来源：http://jzr.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xxj.jlsjyb.cn

PHP:  public static function f() {}
来源：http://jbr.epnwcf.com

JS:   static f() {}
来源：http://ore.mhx1999.top

TS:   static f(): void {}
来源：http://vwf.dashuyun.cn

Java: static void f() {}
来源：http://ryi.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://div.bjfxy.top

Ruby: def self.f; end
来源：http://yen.tianlin.xyz

C#:   public static void F() {}
来源：http://fxy.jianghu66.top

[G09] 接口 / 抽象类
来源：http://uki.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://ljt.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uyc.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nnt.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://qwm.c1oappe.top

Java: interface Shape { double area(); }
来源：http://spf.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://hsx.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gde.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://wjb.tarul.cn

[G10] 访问控制
来源：http://dik.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://hzs.jinqigfzy.top

PHP:  public / protected / private
来源：http://wiy.yonumen.top

JS:   #private 字段；其余公开
来源：http://tor.xylfe.cn


<!-- 参考信息 -->