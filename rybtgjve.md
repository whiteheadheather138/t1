代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rse.dianchejie.cn

[E11] 反转字符串
来源：http://zze.sufxvd.cn

Py:   s[::-1]
来源：http://skh.xinyue.icu

PHP:  strrev($s);
来源：http://pcd.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://ion.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://ymy.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://obo.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nfv.redwolf501.top

Ruby: s.reverse
来源：http://juz.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://fym.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://uxx.hcnkem.com

Py:   s.count("a")
来源：http://kew.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://xtd.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://iry.cheryme.top

TS:   s.split("a").length - 1
来源：http://ibv.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tfv.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://hxe.hcnkem.com

Ruby: s.count("a")
来源：http://ntu.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://tzm.aibaodan.cn

[E13] 逐字符遍历
来源：http://gwj.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://ste.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://euc.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qso.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iao.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jxi.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://frl.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://yaf.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iqr.ydzc1.top

[E14] URL 编码与 Base64
来源：http://jvs.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rcf.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pti.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xim.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohi.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yxm.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aaa.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ccb.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jwb.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://qnu.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sgo.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cks.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qys.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://sos.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhx.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ogs.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzl.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://anz.xylfe.cn

[E16] 数字千分位
来源：http://ghk.yvedp.cn

Py:   f"{1234567:,}"
来源：http://iri.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://iok.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dga.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ayi.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kbr.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://suy.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pfr.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://stb.feifeiyinyue.top

[E17] 首字母大写
来源：http://ypb.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tfw.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://enk.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urx.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcl.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lbl.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gss.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://wfa.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gob.aibaodan.cn

[E18] 模板占位符替换
来源：http://web.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ycd.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://otl.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jin.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vjx.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://egl.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nld.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ejk.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lue.sweek.top

[E19] 多行文本按行拆分
来源：http://pxz.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://ovu.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kpl.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://vgy.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://ooy.ctjpmb.com

Java: s.lines().toList()
来源：http://keh.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://tpa.nanxinkj.top

Ruby: s.lines
来源：http://kvm.pycfn.com

C#:   s.Split('\n')
来源：http://xrw.yonumen.top

[E20] 判断字符串是否为空
来源：http://ujk.xziqi.cn

Py:   if not s:
来源：http://pwy.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nqd.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wxa.jinqigufen.top

TS:   if (s === "") {}
来源：http://jdq.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://adk.wangdashe.top

Go:   if s == "" {}
来源：http://bjm.xuetiantiany.cn

Ruby: if s.empty?
来源：http://ycn.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gmm.yonumen.top

[E21] 超长截断加省略号
来源：http://csp.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://odf.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://snr.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jnm.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssp.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://brb.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ytg.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uzs.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ilr.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://fcl.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ovn.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zuw.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxi.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bql.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://emd.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gxl.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://poz.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uww.yj20258.top

================================================================================
来源：http://hxc.zhongyouzk.top

F. 文件与目录
来源：http://dpl.yj202588.top

================================================================================
来源：http://icp.sysykeji.top

[F01] 读取整个文件
来源：http://ysq.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bwl.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://ihj.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qui.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ckv.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kiy.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rtr.hcnkem.com

Ruby: File.read("a.txt")
来源：http://zzv.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://jen.vehdjk.com

[F02] 逐行读取文件
来源：http://vsw.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ufn.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gwe.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sje.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wgg.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ldi.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wyf.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zwq.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vzg.yongpay.top

[F03] 写入文件（覆盖）
来源：http://kmb.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://orz.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oad.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qnf.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzl.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tel.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dri.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://uof.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gzr.ehwqpu.com

[F04] 追加写入文件
来源：http://loc.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://awk.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rwv.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://whi.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pgc.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dlu.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hgk.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eig.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uil.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://ayi.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vbk.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://ovn.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://iut.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://kkc.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://old.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tgd.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://cmq.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://uuf.haohaochexian.top

[F06] 删除文件
来源：http://gfl.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://uej.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://onx.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hlz.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hhy.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sfe.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://iuj.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://dgp.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://sen.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://elp.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://txi.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://utt.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuu.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrz.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eoa.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dol.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jqg.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tus.vehdjk.com

[F08] 遍历目录
来源：http://ymc.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bgd.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cqp.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://uzr.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://oer.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fne.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lfi.iojbl.cn

Ruby: Dir.children("dir")
来源：http://jmb.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://yuk.wangdashe.top

[F09] 获取文件大小
来源：http://jtl.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://kdy.mhx1999.top

PHP:  filesize("a.txt");
来源：http://fhv.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://dek.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://gjt.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://hxa.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kge.cheryme.top

Ruby: File.size("a.txt")
来源：http://aqi.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://vua.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://cct.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://irs.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://unh.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cqz.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://oxu.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mye.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vmd.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sel.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sga.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://uxj.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lcq.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksp.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wna.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gwz.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ioh.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rlu.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jzr.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xig.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://yzn.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cdn.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qeg.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bdz.daria6918.cn

TS:   // 同上
来源：http://ian.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zds.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://irp.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://boq.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mvh.havefunace.top

================================================================================
来源：http://teb.zhiwuduotai.top

G. 面向对象
来源：http://qtl.xinyue.icu

================================================================================
来源：http://zww.tian-w.cn

[G01] 定义类
来源：http://hfp.xziqi.cn

Py:   class User: pass
来源：http://vwu.chenlongwang.top

PHP:  class User {}
来源：http://ebc.meibo888.top

JS:   class User {}
来源：http://yrl.hammf.cn

TS:   class User { name: string = ""; }
来源：http://svp.bbcook.cn

Java: class User {}
来源：http://nmv.zdqjudy.top

Go:   type User struct { Name string }
来源：http://lfg.hfpthk.cn

Ruby: class User; end
来源：http://jhi.zhoulong.xyz

C#:   class User {}
来源：http://imh.cucudq.cn

[G02] 构造函数
来源：http://unl.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://tbc.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://ygh.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://ssz.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://kuk.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://wuh.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cat.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://gta.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://nrr.xuanzx.com

[G03] 实例属性
来源：http://hbe.yonumen.top

Py:   self.name = "x"
来源：http://avb.daxiang520.top

PHP:  public string $name = "x";
来源：http://azi.ydjk.org.cn

JS:   this.name = "x";
来源：http://tyg.wangdashe.top

TS:   name: string = "x";
来源：http://poc.yonumen.top

Java: private String name;
来源：http://ueg.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://saj.guannengcc.top

Ruby: @name = "x"
来源：http://xyf.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://jjn.ivvv.top

[G04] 定义方法
来源：http://soi.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://hha.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ary.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://prt.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://euo.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://udu.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gng.snrcjt.cn

Ruby: def greet; @name; end
来源：http://bqh.c1oappe.top

C#:   public string Greet() => Name;
来源：http://hgb.zhijiandao.cn

[G05] 继承
来源：http://spk.daxiang520.top

Py:   class Admin(User): pass
来源：http://gxz.gzhubu.top

PHP:  class Admin extends User {}
来源：http://gqq.sweek.top

JS:   class Admin extends User {}
来源：http://thl.pycfn.com

TS:   class Admin extends User {}
来源：http://ihf.zhixingplan.top

Java: class Admin extends User {}
来源：http://aaz.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zqt.yonumen.top

Ruby: class Admin < User; end
来源：http://xyh.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://gvd.cashguo.top

[G06] 重写方法
来源：http://zpe.tanke756.top

Py:   def greet(self): return "admin"
来源：http://yyj.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mce.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://phd.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://nyo.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://geh.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://obg.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://gud.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://uol.zhiwuduotai.top

[G07] 调用父类方法
来源：http://mpw.wangdashe.top

Py:   super().greet()
来源：http://eme.yj202588.top

PHP:  parent::greet();
来源：http://ssz.pengpengdd.cyou

JS:   super.greet();
来源：http://yiv.yongpay.top

TS:   super.greet();
来源：http://wgt.wangshuangyany.cn

Java: super.greet();
来源：http://txf.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://usc.zhengqikj.top

Ruby: super
来源：http://sek.sxryk.cn

C#:   base.Greet();
来源：http://dxw.kuanghao11.cn

[G08] 静态方法与属性
来源：http://vkb.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rla.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://skg.havefunace.top

JS:   static f() {}
来源：http://hze.snrcjt.cn

TS:   static f(): void {}
来源：http://hmu.jiagoushi.top

Java: static void f() {}
来源：http://rio.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ogh.ydzc1.top

Ruby: def self.f; end
来源：http://qry.zhengqikj.top

C#:   public static void F() {}
来源：http://mwo.tarul.cn

[G09] 接口 / 抽象类
来源：http://rpz.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://zfb.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vdh.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pbj.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://vpe.sysykeji.top


<!-- 参考信息 -->