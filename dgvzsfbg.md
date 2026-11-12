代发 wailian999

JS:   [...s].reverse().join("")
来源：http://ona.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://lkw.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nwu.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://aul.birdmap.top

Ruby: s.reverse
来源：http://weh.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vra.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://itw.vehdjk.com

Py:   s.count("a")
来源：http://glf.yonumen.top

PHP:  substr_count($s, "a");
来源：http://uje.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://roi.vehdjk.com

TS:   s.split("a").length - 1
来源：http://ncg.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kdz.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://ohu.yuanzhike.top

Ruby: s.count("a")
来源：http://aut.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://eku.hesvh.cn

[E13] 逐字符遍历
来源：http://lzl.yj202588.top

Py:   for ch in s: print(ch)
来源：http://qug.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lxr.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://anb.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vyo.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xnq.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://txz.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://stw.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uvd.iojbl.cn

[E14] URL 编码与 Base64
来源：http://uwl.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vac.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bnt.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhc.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fyn.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vqt.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lrm.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dit.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://foy.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://jdg.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eof.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ejs.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ppm.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wsi.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gkn.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cmf.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bnp.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://whz.shanyushiyangtech.top

[E16] 数字千分位
来源：http://auj.316326.xyz

Py:   f"{1234567:,}"
来源：http://ybh.gotoacloud.top

PHP:  number_format(1234567);
来源：http://kny.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eit.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hef.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yxt.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jnn.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxc.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://jyt.hesvh.cn

[E17] 首字母大写
来源：http://vel.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lve.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tkd.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ckv.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umo.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tpc.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qxa.hcnkem.com

Ruby: s.capitalize
来源：http://etv.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bxb.zycfv.cn

[E18] 模板占位符替换
来源：http://bif.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://anu.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gfz.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hgc.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qzq.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://avr.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yfh.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aev.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uus.guannengcc.top

[E19] 多行文本按行拆分
来源：http://hzp.yongpay.top

Py:   s.splitlines()
来源：http://oik.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zbd.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://tsl.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://rft.guannengcc.top

Java: s.lines().toList()
来源：http://xkj.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://njs.yuanzhike.top

Ruby: s.lines
来源：http://tkc.sysykeji.top

C#:   s.Split('\n')
来源：http://elp.cheryme.top

[E20] 判断字符串是否为空
来源：http://aml.hnxiangtu.top

Py:   if not s:
来源：http://hgw.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fyf.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nqw.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://mob.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://fsj.tarul.cn

Go:   if s == "" {}
来源：http://mdb.snrcjt.cn

Ruby: if s.empty?
来源：http://kjv.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nzo.jinqigufen.top

[E21] 超长截断加省略号
来源：http://ohz.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zsp.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nvn.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvq.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iaq.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ywe.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://ugt.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omj.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aix.hcnkem.com

[E22] 字节长度与字符长度
来源：http://ogx.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ynm.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rqj.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jpw.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwn.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uob.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xlp.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://uqp.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sup.daria6918.cn

================================================================================
来源：http://pbd.jiagoushi.top

F. 文件与目录
来源：http://bbn.hesvh.cn

================================================================================
来源：http://zdb.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://guw.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pbt.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://ana.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zxm.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wds.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://onx.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acz.yuxming.cn

Ruby: File.read("a.txt")
来源：http://ddh.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://gem.xylfe.cn

[F02] 逐行读取文件
来源：http://xik.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqc.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wge.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pna.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hzt.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://anr.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://emp.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://edb.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dxj.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://riw.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jvk.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wpe.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgq.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gyr.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://itt.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ukc.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://ieq.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lre.chenjidiqi.icu

[F04] 追加写入文件
来源：http://xqr.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ols.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jap.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afr.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgj.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pcw.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wov.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xbe.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tfe.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://rak.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://puw.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://inw.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://ngj.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://vgl.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://keu.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nue.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://dkc.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://szq.yj20258888.top

[F06] 删除文件
来源：http://srf.bbcook.cn

Py:   os.remove("a.txt")
来源：http://tgn.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://boa.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbe.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eri.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bzr.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://drd.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://eck.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://qhg.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://qvr.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fjy.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glh.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lva.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hrz.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://str.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://neh.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xvl.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fde.cdnleiting.top

[F08] 遍历目录
来源：http://rdg.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yis.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lsb.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://avf.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://thz.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpd.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://now.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://hwx.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://duw.birdmap.top

[F09] 获取文件大小
来源：http://syw.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://gca.yfazqb.com

PHP:  filesize("a.txt");
来源：http://xdj.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://kxl.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://zix.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://ovr.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://teo.mhx1999.top

Ruby: File.size("a.txt")
来源：http://zdd.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://tms.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://vjg.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dox.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mmg.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yrx.sxryk.cn

TS:   path.extname("a.txt")
来源：http://jcl.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uyy.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uzt.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://czj.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bti.yuanzhike.top

[F11] 复制与移动文件
来源：http://nvt.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eok.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://apg.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://njk.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jug.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qay.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://upv.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cdb.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xrd.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://xwb.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gmq.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sdo.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cli.shanyushiyangkeji.top

TS:   // 同上
来源：http://mel.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zai.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zzs.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fex.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ttf.ctjpmb.com

================================================================================
来源：http://cxf.ybcxt.top

G. 面向对象
来源：http://pxu.ydjk.org.cn

================================================================================
来源：http://fvj.chenzaomai.com

[G01] 定义类
来源：http://ivj.cqqwz.cn

Py:   class User: pass
来源：http://lxv.yueranfly.top

PHP:  class User {}
来源：http://pvk.jinqigufen.top

JS:   class User {}
来源：http://bys.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://odh.316326.xyz

Java: class User {}
来源：http://wsy.gotoacloud.top

Go:   type User struct { Name string }
来源：http://vei.xziqi.cn

Ruby: class User; end
来源：http://don.yvedp.cn

C#:   class User {}
来源：http://hab.yanxiufei.cn

[G02] 构造函数
来源：http://spb.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://isw.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://qmb.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://uyr.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://aag.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://low.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://awk.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://hcq.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://kkc.fktsv.cn

[G03] 实例属性
来源：http://qbs.xinyue.icu

Py:   self.name = "x"
来源：http://apw.yvedp.cn

PHP:  public string $name = "x";
来源：http://ytn.hnxiangtu.top

JS:   this.name = "x";
来源：http://hbs.hywenlv.cn

TS:   name: string = "x";
来源：http://epp.yj20258888.top

Java: private String name;
来源：http://tdy.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gjt.316326.xyz

Ruby: @name = "x"
来源：http://xdd.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://pxu.sxryk.cn

[G04] 定义方法
来源：http://clx.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://wqv.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dcu.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://ffh.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://gko.sxryk.cn

Java: String greet() { return name; }
来源：http://sta.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://edp.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://cyc.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://oor.hnxiangtu.top

[G05] 继承
来源：http://wtw.52xcode.cn

Py:   class Admin(User): pass
来源：http://rht.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://vkb.daxiang520.top

JS:   class Admin extends User {}
来源：http://pmq.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://fhu.epnwcf.com

Java: class Admin extends User {}
来源：http://vex.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dkp.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://hle.redwolf501.top

C#:   class Admin : User {}
来源：http://web.yuxming.cn

[G06] 重写方法
来源：http://zbs.sweek.top

Py:   def greet(self): return "admin"
来源：http://gus.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://cow.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://exn.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://zdz.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://dlt.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kfm.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://zkn.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://zct.vqdsnc.cn

[G07] 调用父类方法
来源：http://vcp.hnxiangtu.top

Py:   super().greet()
来源：http://qlp.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://kbm.pycfn.com

JS:   super.greet();
来源：http://exr.xziqi.cn

TS:   super.greet();
来源：http://ekq.cashguo.top

Java: super.greet();
来源：http://vep.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sax.jinghuilouyu.cn

Ruby: super
来源：http://gah.aibaodan.cn

C#:   base.Greet();
来源：http://utp.yanxiufei.cn

[G08] 静态方法与属性
来源：http://uoz.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kok.dashuyun.cn

PHP:  public static function f() {}
来源：http://bcs.gogol.net.cn

JS:   static f() {}
来源：http://adm.cucudq.cn

TS:   static f(): void {}
来源：http://tue.nanxinkj.top

Java: static void f() {}
来源：http://lpi.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zmc.gaohongyu789.top

Ruby: def self.f; end
来源：http://agp.yanxiufei.cn

C#:   public static void F() {}
来源：http://xqf.fktsv.cn

[G09] 接口 / 抽象类
来源：http://ujg.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://soa.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://ktd.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pwe.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://gxy.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://nae.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://uii.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqh.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://nph.shangyingyoupin.top


<!-- 参考信息 -->