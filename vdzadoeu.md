代发 wailian999

JS:   [...s].reverse().join("")
来源：http://swn.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://zgx.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wgs.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zgj.bbcook.cn

Ruby: s.reverse
来源：http://rmz.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://rii.sxryk.cn

[E12] 统计某字符出现次数
来源：http://oay.hfpthk.cn

Py:   s.count("a")
来源：http://hhd.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://xbb.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://jjx.andypj.xyz

TS:   s.split("a").length - 1
来源：http://eoe.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fsr.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://mlw.cheryme.top

Ruby: s.count("a")
来源：http://yny.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://eaq.xylfe.cn

[E13] 逐字符遍历
来源：http://qvd.havefunace.top

Py:   for ch in s: print(ch)
来源：http://qbp.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bhr.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jee.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://giw.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wcx.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eki.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xnh.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ato.tarul.cn

[E14] URL 编码与 Base64
来源：http://zbw.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xox.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hkp.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gfw.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fny.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://irl.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mqi.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xjf.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bdt.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://ced.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kpp.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cdb.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rks.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bxb.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vhy.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cdk.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hzd.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://adb.tianlin.xyz

[E16] 数字千分位
来源：http://jqg.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://ien.iojbl.cn

PHP:  number_format(1234567);
来源：http://ies.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jfi.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dka.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ssq.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nla.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spl.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://gry.cdnleiting.top

[E17] 首字母大写
来源：http://tbp.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gvx.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yar.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jky.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kev.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fgc.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://czg.ppjwa.cn

Ruby: s.capitalize
来源：http://aet.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ooq.9152youxi.cn

[E18] 模板占位符替换
来源：http://rxo.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scv.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wcb.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rbm.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nbp.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://llh.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mrz.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gvm.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jsb.pycfn.com

[E19] 多行文本按行拆分
来源：http://lvn.fzhhl.top

Py:   s.splitlines()
来源：http://eml.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pqt.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://fip.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://hkz.ivvv.top

Java: s.lines().toList()
来源：http://gjt.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://qac.haohaochexian.top

Ruby: s.lines
来源：http://evv.yvedp.cn

C#:   s.Split('\n')
来源：http://sck.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://sss.guannengcc.top

Py:   if not s:
来源：http://tta.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bco.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lao.xylfe.cn

TS:   if (s === "") {}
来源：http://rpq.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://vld.yvedp.cn

Go:   if s == "" {}
来源：http://aaa.zhongyouzk.top

Ruby: if s.empty?
来源：http://cvj.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mbj.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://kgh.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rit.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ttu.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ojl.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbv.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xad.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://pgs.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lbu.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jdh.tanke756.top

[E22] 字节长度与字符长度
来源：http://nma.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rfh.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypq.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://foj.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hjp.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rpf.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oma.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://bst.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fjv.shuidangran.top

================================================================================
来源：http://geo.jyoumei.cn

F. 文件与目录
来源：http://vuo.yj20258888.top

================================================================================
来源：http://ith.cucudq.cn

[F01] 读取整个文件
来源：http://qqt.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://joh.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://hzv.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ntx.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gzq.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://phn.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wfy.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://lvx.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://xko.cucudq.cn

[F02] 逐行读取文件
来源：http://yuw.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hln.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://auo.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqm.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mfh.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zyi.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bdm.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dou.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tzp.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://iqw.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qjn.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ubv.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuq.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zzp.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kit.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ndn.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://fbl.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lyf.ehwqpu.com

[F04] 追加写入文件
来源：http://vkz.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://crz.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qph.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ngq.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mtx.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qhe.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xsp.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://luz.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rde.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://rcz.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://myo.tanke756.top

PHP:  file_exists("a.txt");
来源：http://efr.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://dze.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://efi.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qqo.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tzb.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://arr.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://rhy.hysaishi.cn

[F06] 删除文件
来源：http://fpn.daxiang520.top

Py:   os.remove("a.txt")
来源：http://nle.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://cru.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://wwu.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pmv.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qdi.meibo888.top

Go:   os.Remove("a.txt")
来源：http://uco.yj20258.top

Ruby: File.delete("a.txt")
来源：http://hib.yj202588.top

C#:   File.Delete("a.txt");
来源：http://inf.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://eco.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jsu.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fhi.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zon.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jzp.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aru.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ntr.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wmu.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lat.shzxlz.cn

[F08] 遍历目录
来源：http://cgz.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yhu.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ybq.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://kkl.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://xig.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://afz.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xee.hesvh.cn

Ruby: Dir.children("dir")
来源：http://qwf.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://usz.ivvv.top

[F09] 获取文件大小
来源：http://jcc.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://gnn.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://qed.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://kgg.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://mrj.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://huq.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zoe.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://jvw.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://vmd.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://pto.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hng.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yyp.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tau.yj202588.top

TS:   path.extname("a.txt")
来源：http://wex.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tnx.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iuc.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ice.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pdn.gotoacloud.top

[F11] 复制与移动文件
来源：http://whu.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bxg.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqf.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iwa.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bhg.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ohr.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jpo.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpm.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zrp.tianlin.xyz

[F12] CSV 读写
来源：http://ygc.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mev.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://knq.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cms.hysaishi.cn

TS:   // 同上
来源：http://akb.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cmt.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ygy.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jbn.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bhf.zhiwuduotai.top

================================================================================
来源：http://htn.nanxuanxn.top

G. 面向对象
来源：http://ldk.jiagoushi.top

================================================================================
来源：http://jkc.yangfankeji.com

[G01] 定义类
来源：http://qhf.ydjk.org.cn

Py:   class User: pass
来源：http://lyc.smart0.xyz

PHP:  class User {}
来源：http://mhp.shuidangran.top

JS:   class User {}
来源：http://msm.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://dyj.cucudq.cn

Java: class User {}
来源：http://dfa.fengsongda.top

Go:   type User struct { Name string }
来源：http://rqv.fengsongda.top

Ruby: class User; end
来源：http://bpd.xuetiantiany.cn

C#:   class User {}
来源：http://wgv.yuxming.cn

[G02] 构造函数
来源：http://wyz.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://otd.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://rbd.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://nql.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://gcw.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://wtk.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qvb.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://hfh.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://cjp.tianlin.xyz

[G03] 实例属性
来源：http://aef.vehdjk.com

Py:   self.name = "x"
来源：http://yjk.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://uts.jyoumei.cn

JS:   this.name = "x";
来源：http://hqh.cqqwz.cn

TS:   name: string = "x";
来源：http://bwu.cdnleiting.top

Java: private String name;
来源：http://aal.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dsf.jqgfzy.top

Ruby: @name = "x"
来源：http://kdt.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://efv.fktsv.cn

[G04] 定义方法
来源：http://rji.mhx1999.top

Py:   def greet(self): return self.name
来源：http://vqq.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iyn.cucudq.cn

JS:   greet() { return this.name; }
来源：http://fjc.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://xhl.quarkkingdee.top

Java: String greet() { return name; }
来源：http://ywb.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wly.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://cnd.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://bxl.hnqzz.top

[G05] 继承
来源：http://pwe.dashuyun.cn

Py:   class Admin(User): pass
来源：http://uop.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://jel.zdqjudy.top

JS:   class Admin extends User {}
来源：http://kvf.0kj1m.cn

TS:   class Admin extends User {}
来源：http://ykz.jinqigfzy.top

Java: class Admin extends User {}
来源：http://ipd.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fhr.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://rtc.xziqi.cn

C#:   class Admin : User {}
来源：http://mwz.svipenyu.cn

[G06] 重写方法
来源：http://gad.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://uvl.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://drg.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://xpl.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://hlc.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://jkq.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ser.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://ilq.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://qeh.0kj1m.cn

[G07] 调用父类方法
来源：http://sht.zhongyouzk.top

Py:   super().greet()
来源：http://nnk.sxryk.cn

PHP:  parent::greet();
来源：http://clk.jinghuilouyu.cn

JS:   super.greet();
来源：http://pqk.yj20258888.top

TS:   super.greet();
来源：http://kwg.jinqigfzy.top

Java: super.greet();
来源：http://yao.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ped.xuanzx.com

Ruby: super
来源：http://wym.yongpay.top

C#:   base.Greet();
来源：http://cek.epnwcf.com

[G08] 静态方法与属性
来源：http://cha.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ktr.daria6918.cn

PHP:  public static function f() {}
来源：http://xxm.guowangkeji.top

JS:   static f() {}
来源：http://ybn.fzhhl.top

TS:   static f(): void {}
来源：http://tak.shanyushiyangtech.top

Java: static void f() {}
来源：http://svr.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://efb.cashguo.top

Ruby: def self.f; end
来源：http://vxd.tarul.cn

C#:   public static void F() {}
来源：http://qen.yuxming.cn

[G09] 接口 / 抽象类
来源：http://ehv.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://iyr.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xzi.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ehd.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://ubv.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://cev.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://pwp.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tiz.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://xmr.vehdjk.com


<!-- 参考信息 -->