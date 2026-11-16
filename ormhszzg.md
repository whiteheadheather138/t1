代发 wailian999

JS:   [...s].reverse().join("")
来源：http://xgg.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://kyu.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sah.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://npw.haohaochexian.top

Ruby: s.reverse
来源：http://hdl.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yrs.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://wfk.52xcode.cn

Py:   s.count("a")
来源：http://czs.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://kpo.ybcxt.top

JS:   s.split("a").length - 1
来源：http://pau.xziqi.cn

TS:   s.split("a").length - 1
来源：http://tdm.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://grp.yj202588.top

Go:   strings.Count(s, "a")
来源：http://qjg.hongshengwenyu.top

Ruby: s.count("a")
来源：http://lzb.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://crs.havefunace.top

[E13] 逐字符遍历
来源：http://pkg.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://vnc.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rdt.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qes.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zfs.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mwf.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gxh.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cmz.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dhj.epnwcf.com

[E14] URL 编码与 Base64
来源：http://hcm.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oco.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://tft.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kml.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jzx.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jsi.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tsk.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mjb.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ihf.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://iqn.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://thd.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nft.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://har.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://due.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kwj.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://icq.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ygc.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqj.cucudq.cn

[E16] 数字千分位
来源：http://cgb.yj20258.top

Py:   f"{1234567:,}"
来源：http://llb.uphjek.com

PHP:  number_format(1234567);
来源：http://dsi.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uzk.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qfa.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azg.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zzz.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfs.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://qgj.aibaodan.cn

[E17] 首字母大写
来源：http://zqu.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzt.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ulv.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yus.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcm.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ikm.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rqv.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://avz.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhf.jianghu66.top

[E18] 模板占位符替换
来源：http://emj.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vox.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tql.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ney.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://wpc.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ehm.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iiv.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gxw.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vxf.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://hmz.birdmap.top

Py:   s.splitlines()
来源：http://ohx.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dvg.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://dze.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://kpz.chenjidiqi.icu

Java: s.lines().toList()
来源：http://jut.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://nah.meibo888.top

Ruby: s.lines
来源：http://exd.nanxinkj.top

C#:   s.Split('\n')
来源：http://itm.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://uyp.yuanzhike.top

Py:   if not s:
来源：http://mra.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rqo.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eor.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://jwf.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://elk.svipenyu.cn

Go:   if s == "" {}
来源：http://lkr.epnwcf.com

Ruby: if s.empty?
来源：http://wdv.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hrp.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://zuh.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hes.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vrb.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyq.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzo.zhoulong.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qwj.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://spf.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwg.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wid.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://igz.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uou.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klt.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://czt.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nve.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xxo.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ekv.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://byl.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hkp.hammf.cn

================================================================================
来源：http://wcd.andypj.xyz

F. 文件与目录
来源：http://ktk.birdmap.top

================================================================================
来源：http://qki.meibo888.top

[F01] 读取整个文件
来源：http://onb.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rsq.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://ram.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qta.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mtx.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hmm.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zvq.iojbl.cn

Ruby: File.read("a.txt")
来源：http://igh.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://hfx.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://ubr.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vak.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xso.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ryn.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vfg.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pkh.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nju.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ckb.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mre.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://eet.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ccl.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dnz.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwe.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://roa.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pcu.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://djq.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://vzm.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ovf.haohaochexian.top

[F04] 追加写入文件
来源：http://elu.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfr.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tim.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rpu.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwf.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rwc.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pli.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eed.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ygv.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://kxz.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nwq.meibo888.top

PHP:  file_exists("a.txt");
来源：http://neu.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://adu.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://jok.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lfc.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ppf.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://crc.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://tpf.xylfe.cn

[F06] 删除文件
来源：http://qyp.mhx1999.top

Py:   os.remove("a.txt")
来源：http://omi.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://mtf.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://kfg.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://beh.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sbi.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://zsk.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://iyt.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://dqv.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://hyf.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://khj.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bst.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ull.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adv.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pts.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iub.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rzk.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uti.yangfankeji.com

[F08] 遍历目录
来源：http://igr.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://jlh.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mpb.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://lxj.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://ejk.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hrq.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://crn.shuidangran.top

Ruby: Dir.children("dir")
来源：http://xop.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://ypb.tanke756.top

[F09] 获取文件大小
来源：http://oiw.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://ipt.tarul.cn

PHP:  filesize("a.txt");
来源：http://kii.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://zzm.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://qwk.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://tex.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fqp.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://smc.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://rmn.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://fea.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://teh.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rtu.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cqh.xinyue.icu

TS:   path.extname("a.txt")
来源：http://kqs.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbj.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yuz.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://del.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hai.cashguo.top

[F11] 复制与移动文件
来源：http://opp.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fqe.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sto.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gro.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gnl.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://odt.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oka.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dor.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oyy.snrcjt.cn

[F12] CSV 读写
来源：http://yse.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://utu.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wmg.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zot.chenjidiqi.icu

TS:   // 同上
来源：http://mih.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ptz.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ofx.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lme.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ojw.yonumen.top

================================================================================
来源：http://occ.chenzaomai.com

G. 面向对象
来源：http://dos.pengpengdd.cyou

================================================================================
来源：http://yer.yj202588.top

[G01] 定义类
来源：http://vae.sxryk.cn

Py:   class User: pass
来源：http://qwe.ctjpmb.com

PHP:  class User {}
来源：http://diu.sweek.top

JS:   class User {}
来源：http://xvs.yj202588.top

TS:   class User { name: string = ""; }
来源：http://sbz.zhengqikj.top

Java: class User {}
来源：http://qnu.ybcxt.top

Go:   type User struct { Name string }
来源：http://ztr.yvedp.cn

Ruby: class User; end
来源：http://ygf.iojbl.cn

C#:   class User {}
来源：http://lnx.svipenyu.cn

[G02] 构造函数
来源：http://oha.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://gsi.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://kkl.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://map.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://bty.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://gcc.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ghe.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://hfm.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://ltp.quarkkingdee.top

[G03] 实例属性
来源：http://zju.hfpthk.cn

Py:   self.name = "x"
来源：http://cjr.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://zzv.svipenyu.cn

JS:   this.name = "x";
来源：http://xma.tanke756.top

TS:   name: string = "x";
来源：http://ckg.gogol.net.cn

Java: private String name;
来源：http://evv.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zet.ctjpmb.com

Ruby: @name = "x"
来源：http://fre.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://lkh.daria6918.cn

[G04] 定义方法
来源：http://zxf.yvedp.cn

Py:   def greet(self): return self.name
来源：http://fzz.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bzj.guannengcc.top

JS:   greet() { return this.name; }
来源：http://zek.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://oga.yonumen.top

Java: String greet() { return name; }
来源：http://vnb.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ehq.daria6918.cn

Ruby: def greet; @name; end
来源：http://gjw.andypj.xyz

C#:   public string Greet() => Name;
来源：http://vaa.jinqigfzy.top

[G05] 继承
来源：http://zcb.yj20258.top

Py:   class Admin(User): pass
来源：http://nvc.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://gco.gotoacloud.top

JS:   class Admin extends User {}
来源：http://oig.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://dke.hesvh.cn

Java: class Admin extends User {}
来源：http://zuu.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sdo.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://zji.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://vit.yangfankeji.com

[G06] 重写方法
来源：http://mgi.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://guc.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ysy.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://gjq.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://din.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://zjh.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hut.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://hvo.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://ovw.xinyue.icu

[G07] 调用父类方法
来源：http://bpl.tanke756.top

Py:   super().greet()
来源：http://ipa.hnqzz.top

PHP:  parent::greet();
来源：http://oil.yuxming.cn

JS:   super.greet();
来源：http://ncd.ehwqpu.com

TS:   super.greet();
来源：http://egl.aibaodan.cn

Java: super.greet();
来源：http://abw.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://afa.snrcjt.cn

Ruby: super
来源：http://qdq.jinghuilouyu.cn

C#:   base.Greet();
来源：http://pct.0kj1m.cn

[G08] 静态方法与属性
来源：http://ehb.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wjo.0kj1m.cn

PHP:  public static function f() {}
来源：http://jtw.aibaodan.cn

JS:   static f() {}
来源：http://ear.aibaodan.cn

TS:   static f(): void {}
来源：http://chx.52xcode.cn

Java: static void f() {}
来源：http://lax.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://krm.tarul.cn

Ruby: def self.f; end
来源：http://qya.fengsongda.top

C#:   public static void F() {}
来源：http://wew.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://qxe.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://spl.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gut.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bye.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://jfa.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://stb.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://tql.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jgp.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://vxm.feifeiyinyue.top


<!-- 参考信息 -->