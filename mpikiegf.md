代发 wailian999

JS:   [...s].reverse().join("")
来源：http://nsw.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://blh.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://idk.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lrp.ybcxt.top

Ruby: s.reverse
来源：http://syg.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nzb.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://kge.0kj1m.cn

Py:   s.count("a")
来源：http://oue.yongpay.top

PHP:  substr_count($s, "a");
来源：http://rod.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://aka.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://nzo.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rmx.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://byw.epnwcf.com

Ruby: s.count("a")
来源：http://ykr.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://ngc.quarkkingdee.top

[E13] 逐字符遍历
来源：http://uxx.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://dbe.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rgd.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fbx.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://qia.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ufc.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jxv.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hvm.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fnj.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://pgp.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vrp.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kvg.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ked.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ncl.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://emk.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mlm.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://npe.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://soq.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://wmh.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://njh.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rer.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hcg.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://suo.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yhq.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lzn.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jqp.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mri.316326.xyz

[E16] 数字千分位
来源：http://hvp.daria6918.cn

Py:   f"{1234567:,}"
来源：http://alh.bjfxy.top

PHP:  number_format(1234567);
来源：http://yhw.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gti.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cmi.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myf.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdg.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kvl.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://xfw.hongshengwenyu.top

[E17] 首字母大写
来源：http://wyl.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bgm.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ite.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://phe.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cxi.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tqh.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://doh.tanke756.top

Ruby: s.capitalize
来源：http://tmt.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jok.fktsv.cn

[E18] 模板占位符替换
来源：http://ozz.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lro.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ewg.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nex.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ste.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://epg.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nbe.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vdd.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iet.smart0.xyz

[E19] 多行文本按行拆分
来源：http://yva.shangyingyoupin.top

Py:   s.splitlines()
来源：http://gdp.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nzh.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://yve.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://nzc.yvedp.cn

Java: s.lines().toList()
来源：http://rlm.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://zij.shanyushiyangtech.top

Ruby: s.lines
来源：http://gvt.hysaishi.cn

C#:   s.Split('\n')
来源：http://fub.sweek.top

[E20] 判断字符串是否为空
来源：http://ram.hammf.cn

Py:   if not s:
来源：http://umc.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://air.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fto.snrcjt.cn

TS:   if (s === "") {}
来源：http://dsj.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://upw.jlsjyb.cn

Go:   if s == "" {}
来源：http://qhc.hammf.cn

Ruby: if s.empty?
来源：http://hch.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pev.shzxlz.cn

[E21] 超长截断加省略号
来源：http://jdx.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nrw.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ijf.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://imq.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbq.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fas.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://gzr.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gag.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pak.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://dzp.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ohr.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ceg.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hux.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ooa.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kil.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ici.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://dqd.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ubd.chenjidiqi.icu

================================================================================
来源：http://rgl.ydjk.org.cn

F. 文件与目录
来源：http://vim.gzhubu.top

================================================================================
来源：http://pkd.daxiang520.top

[F01] 读取整个文件
来源：http://qgf.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nqm.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://ebm.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vjj.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://emp.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uky.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oiy.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://xlw.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://idq.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://kbr.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fty.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dpr.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ckz.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wug.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jvj.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ygm.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sem.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rzb.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://pda.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xow.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://waf.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thi.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kri.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvl.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lvo.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mag.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rer.dianchejie.cn

[F04] 追加写入文件
来源：http://joa.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fib.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mvy.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mql.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifz.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qzs.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ppv.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ghy.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vky.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://obo.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kgx.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://bak.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://ket.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://kap.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uvz.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fpa.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://axw.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://hpn.redwolf501.top

[F06] 删除文件
来源：http://xwm.xziqi.cn

Py:   os.remove("a.txt")
来源：http://kpy.yfazqb.com

PHP:  unlink("a.txt");
来源：http://iwl.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mvz.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://vcq.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ifa.yj20258.top

Go:   os.Remove("a.txt")
来源：http://qhr.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://xml.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://kbc.wangdashe.top

[F07] 创建目录（含多级）
来源：http://dpn.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jmv.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hiv.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tof.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btm.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gmt.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jcz.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://btt.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lft.0kj1m.cn

[F08] 遍历目录
来源：http://dfq.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://smq.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lsw.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://izn.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://rqq.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ptl.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://omt.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://kxr.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://abt.hysaishi.cn

[F09] 获取文件大小
来源：http://fyl.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://zav.hesvh.cn

PHP:  filesize("a.txt");
来源：http://sjf.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://zob.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://ttt.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://lrh.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qrt.epnwcf.com

Ruby: File.size("a.txt")
来源：http://qbw.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://lwt.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://kym.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rmn.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hcm.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xfp.fehbvm.com

TS:   path.extname("a.txt")
来源：http://ebi.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rpg.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eht.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ric.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lgb.sxryk.cn

[F11] 复制与移动文件
来源：http://xkw.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zig.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://stz.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tpw.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://epv.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lfh.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tbq.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cpy.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bwh.jyoumei.cn

[F12] CSV 读写
来源：http://xui.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://adb.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tpr.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byi.zhiwuduotai.top

TS:   // 同上
来源：http://dkv.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhq.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rkj.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fan.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zcz.chenjidiqi.icu

================================================================================
来源：http://xdj.fktsv.cn

G. 面向对象
来源：http://mja.hesvh.cn

================================================================================
来源：http://lfy.gzhubu.top

[G01] 定义类
来源：http://oss.0kj1m.cn

Py:   class User: pass
来源：http://hps.cucudq.cn

PHP:  class User {}
来源：http://urw.jqgfzy.top

JS:   class User {}
来源：http://jtj.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://mhz.meibo888.top

Java: class User {}
来源：http://whk.meibo888.top

Go:   type User struct { Name string }
来源：http://zda.yj202588.top

Ruby: class User; end
来源：http://nrv.xingfuxueyuan.xyz

C#:   class User {}
来源：http://bao.cashguo.top

[G02] 构造函数
来源：http://jom.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://mqu.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://hzo.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://fzq.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://msa.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://ssh.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gjq.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://djx.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://emk.fzhhl.top

[G03] 实例属性
来源：http://zxa.ydjk.org.cn

Py:   self.name = "x"
来源：http://brx.nanxinkj.top

PHP:  public string $name = "x";
来源：http://vpk.fzhhl.top

JS:   this.name = "x";
来源：http://fdr.xuetiantiany.cn

TS:   name: string = "x";
来源：http://rbd.jyoumei.cn

Java: private String name;
来源：http://str.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sil.sysykeji.top

Ruby: @name = "x"
来源：http://bjy.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://fcu.hcnkem.com

[G04] 定义方法
来源：http://ikn.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://twy.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://goo.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://box.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://uwz.sufxvd.cn

Java: String greet() { return name; }
来源：http://djl.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://meo.andypj.xyz

Ruby: def greet; @name; end
来源：http://hqt.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://cis.andypj.xyz

[G05] 继承
来源：http://drz.svipenyu.cn

Py:   class Admin(User): pass
来源：http://vwh.andypj.xyz

PHP:  class Admin extends User {}
来源：http://mnr.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://sob.yj20258888.top

TS:   class Admin extends User {}
来源：http://zyj.zhijiandao.cn

Java: class Admin extends User {}
来源：http://hel.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kwv.mhx1999.top

Ruby: class Admin < User; end
来源：http://ywu.uphjek.com

C#:   class Admin : User {}
来源：http://bws.yj202588.top

[G06] 重写方法
来源：http://gik.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://aiw.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dce.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://ior.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://gah.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://bdd.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ecs.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://gul.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://hkv.shuidangran.top

[G07] 调用父类方法
来源：http://cdv.pycfn.com

Py:   super().greet()
来源：http://smg.jlsjyb.cn

PHP:  parent::greet();
来源：http://ngc.aizwys.cn

JS:   super.greet();
来源：http://pxt.fanxiaobao.xyz

TS:   super.greet();
来源：http://qup.yuxming.cn

Java: super.greet();
来源：http://wby.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ang.hesvh.cn

Ruby: super
来源：http://ltl.xuetiantiany.cn

C#:   base.Greet();
来源：http://jzn.yangfankeji.com

[G08] 静态方法与属性
来源：http://lcf.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rts.dashuyun.cn

PHP:  public static function f() {}
来源：http://qnk.gotoacloud.top

JS:   static f() {}
来源：http://gzc.bbcook.cn

TS:   static f(): void {}
来源：http://spo.chenlongwang.top

Java: static void f() {}
来源：http://nvs.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eoo.dashuyun.cn

Ruby: def self.f; end
来源：http://sen.yangfankeji.com

C#:   public static void F() {}
来源：http://uxb.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://vvy.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://axk.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://jjo.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mhy.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://vkb.fehbvm.com

Java: interface Shape { double area(); }
来源：http://qmd.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://yhx.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://utm.sweek.top

C#:   interface IShape { double Area(); }
来源：http://qwm.9152youxi.cn


<!-- 参考信息 -->