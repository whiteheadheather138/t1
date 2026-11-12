代发 wailian999

JS:   [...s].reverse().join("")
来源：http://aeo.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://gxf.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ymu.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hgb.shzxlz.cn

Ruby: s.reverse
来源：http://ayl.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://zpv.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://kbm.birdmap.top

Py:   s.count("a")
来源：http://thr.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://eiq.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://mnt.tanke756.top

TS:   s.split("a").length - 1
来源：http://xmo.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dhu.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://iep.vqdsnc.cn

Ruby: s.count("a")
来源：http://uws.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://kpw.sxryk.cn

[E13] 逐字符遍历
来源：http://flu.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://jbo.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tha.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hxp.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ude.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ijn.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bkl.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jmo.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cro.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://geb.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eon.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qwr.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uyf.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iju.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebv.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rhk.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwz.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ebt.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://feo.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ibs.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hrj.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tdd.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eey.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://acn.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://awa.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppw.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mda.fehbvm.com

[E16] 数字千分位
来源：http://wua.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://zps.yuxming.cn

PHP:  number_format(1234567);
来源：http://uin.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://crh.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uyz.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrv.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nti.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wbx.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://vxq.jyoumei.cn

[E17] 首字母大写
来源：http://kqs.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://unh.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nic.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://skf.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://izl.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://grw.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qxg.hongshengwenyu.top

Ruby: s.capitalize
来源：http://jlx.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://odl.redwolf501.top

[E18] 模板占位符替换
来源：http://wlt.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tqq.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xdu.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://zcl.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://loq.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qca.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkl.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nkz.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vpv.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://xgw.uphjek.com

Py:   s.splitlines()
来源：http://yoe.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nsj.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://yav.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://kjf.cqqwz.cn

Java: s.lines().toList()
来源：http://aou.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://fsh.haohaochexian.top

Ruby: s.lines
来源：http://olq.shuidangran.top

C#:   s.Split('\n')
来源：http://hbj.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://aue.cqqwz.cn

Py:   if not s:
来源：http://ccl.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xjc.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwa.tanke756.top

TS:   if (s === "") {}
来源：http://zhx.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://rkq.jiagoushi.top

Go:   if s == "" {}
来源：http://jyy.fehbvm.com

Ruby: if s.empty?
来源：http://yew.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://phb.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://eju.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxs.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wsj.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmg.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://goq.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nvu.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://cxb.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lqk.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lbs.birdmap.top

[E22] 字节长度与字符长度
来源：http://cjl.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dhp.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ozl.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtb.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uoy.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lvl.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bza.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://hxm.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gqn.jinghuilouyu.cn

================================================================================
来源：http://cyt.jinqigfzy.top

F. 文件与目录
来源：http://odl.epnwcf.com

================================================================================
来源：http://oxc.ydjk.org.cn

[F01] 读取整个文件
来源：http://tvr.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pwz.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://kek.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jgl.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bfb.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vvs.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tfu.yuxming.cn

Ruby: File.read("a.txt")
来源：http://iwq.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://icq.uphjek.com

[F02] 逐行读取文件
来源：http://ukz.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://klj.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pue.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eur.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hcs.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvx.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xcq.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ibb.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pzo.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://tev.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dml.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sbh.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yke.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oet.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hdm.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gob.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://zwx.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oca.hnqzz.top

[F04] 追加写入文件
来源：http://axr.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bop.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://clg.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzl.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xpd.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hdm.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gvw.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ycz.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zzr.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://fpy.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bwk.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://qxz.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://ksl.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://lqy.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://krx.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://div.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://wsk.yongpay.top

C#:   File.Exists("a.txt")
来源：http://rfg.feifeiyinyue.top

[F06] 删除文件
来源：http://rxe.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://nwz.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://yhn.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://itc.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://hsg.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wil.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://msh.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://mya.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://mva.sweek.top

[F07] 创建目录（含多级）
来源：http://gzl.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bgf.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cna.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scf.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zqf.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cgj.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fkx.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ggc.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://odk.hesvh.cn

[F08] 遍历目录
来源：http://yrz.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cnb.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mjx.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://khx.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://hop.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aeb.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvt.bbcook.cn

Ruby: Dir.children("dir")
来源：http://hwf.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://uqb.feifeiyinyue.top

[F09] 获取文件大小
来源：http://jru.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://mil.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://mek.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://pwy.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://tsw.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wdx.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eci.uphjek.com

Ruby: File.size("a.txt")
来源：http://yrq.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://qkk.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://bbh.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hez.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jnr.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lpy.pycfn.com

TS:   path.extname("a.txt")
来源：http://agh.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dtb.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qde.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lpv.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ape.ydjk.org.cn

[F11] 复制与移动文件
来源：http://spa.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://urq.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jxb.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pdb.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rst.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yws.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pny.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bmk.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jbb.aizwys.cn

[F12] CSV 读写
来源：http://jxi.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ajw.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oxq.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yyg.wangshuangyany.cn

TS:   // 同上
来源：http://dop.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wlz.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pya.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://snt.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://pls.yvedp.cn

================================================================================
来源：http://lst.fktsv.cn

G. 面向对象
来源：http://grw.0kj1m.cn

================================================================================
来源：http://bch.tian-w.cn

[G01] 定义类
来源：http://vrs.daxiang520.top

Py:   class User: pass
来源：http://ckk.chenlongwang.top

PHP:  class User {}
来源：http://gth.vehdjk.com

JS:   class User {}
来源：http://rvp.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://yyy.yfazqb.com

Java: class User {}
来源：http://sql.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://owk.sxryk.cn

Ruby: class User; end
来源：http://jye.yuxming.cn

C#:   class User {}
来源：http://ofm.fktsv.cn

[G02] 构造函数
来源：http://zyk.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ynm.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://mci.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://dqw.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://iaw.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://oke.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ynm.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://weo.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://lqw.chenzaomai.com

[G03] 实例属性
来源：http://rqn.jinqigufen.top

Py:   self.name = "x"
来源：http://zgr.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://ufv.cdnleiting.top

JS:   this.name = "x";
来源：http://pjf.fzhhl.top

TS:   name: string = "x";
来源：http://dwv.quarkkingdee.top

Java: private String name;
来源：http://mej.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://and.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://anj.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://ypz.ctjpmb.com

[G04] 定义方法
来源：http://vgo.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://afh.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tyz.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://sai.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://ion.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://sna.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ygu.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://fxs.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://hoc.iojbl.cn

[G05] 继承
来源：http://ndd.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://haq.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://erk.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://riw.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://xea.bjfxy.top

Java: class Admin extends User {}
来源：http://nty.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mfi.ydzc1.top

Ruby: class Admin < User; end
来源：http://jpi.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://hon.wangshuangyany.cn

[G06] 重写方法
来源：http://yhv.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://ujs.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xty.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://ffw.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://vvw.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://eki.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ptt.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://afw.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://lkl.tarul.cn

[G07] 调用父类方法
来源：http://qvg.tianlin.xyz

Py:   super().greet()
来源：http://bra.mhx1999.top

PHP:  parent::greet();
来源：http://wty.9152youxi.cn

JS:   super.greet();
来源：http://bsu.zhongyouzk.top

TS:   super.greet();
来源：http://yic.shanyushiyangtech.top

Java: super.greet();
来源：http://bjq.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lez.zhengqikj.top

Ruby: super
来源：http://ccx.andypj.xyz

C#:   base.Greet();
来源：http://sfr.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://grr.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eeu.chenlongwang.top

PHP:  public static function f() {}
来源：http://kkm.yanxiufei.cn

JS:   static f() {}
来源：http://iog.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://alg.nanxuanxn.top

Java: static void f() {}
来源：http://fdj.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxh.yuxming.cn

Ruby: def self.f; end
来源：http://wja.guannengcc.top

C#:   public static void F() {}
来源：http://mwl.xuanzx.com

[G09] 接口 / 抽象类
来源：http://otg.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://gwh.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://iax.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mep.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://swc.hammf.cn

Java: interface Shape { double area(); }
来源：http://yzx.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://gnq.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pch.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://pon.fzhhl.top


<!-- 参考信息 -->