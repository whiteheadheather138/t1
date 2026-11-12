代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://puj.yj20258.top

Java: String.format("%03d", 7)
来源：http://dcq.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xpn.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjv.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ujf.sweek.top

[E11] 反转字符串
来源：http://zqg.yuanzhike.top

Py:   s[::-1]
来源：http://hkg.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://ooq.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://pix.cheryme.top

TS:   [...s].reverse().join("")
来源：http://wiz.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://svh.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vur.shuidangran.top

Ruby: s.reverse
来源：http://yes.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://pmo.vehdjk.com

[E12] 统计某字符出现次数
来源：http://bgp.316326.xyz

Py:   s.count("a")
来源：http://meu.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://ipk.yuxming.cn

JS:   s.split("a").length - 1
来源：http://jcp.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://cxm.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dqn.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://lyi.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://cuc.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://rdu.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://ixl.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://udf.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://boe.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lsv.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://feq.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ihp.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pvk.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sqy.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vit.pycfn.com

[E14] URL 编码与 Base64
来源：http://fis.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://icn.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://erw.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tea.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://euo.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wux.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gyq.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fxc.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ull.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://zuv.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yfj.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mzb.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kyw.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ote.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ulx.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://itc.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ypu.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zlx.316326.xyz

[E16] 数字千分位
来源：http://ret.sweek.top

Py:   f"{1234567:,}"
来源：http://zgp.hammf.cn

PHP:  number_format(1234567);
来源：http://ajw.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nry.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qzg.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqx.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ljg.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gml.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://mxn.gogol.net.cn

[E17] 首字母大写
来源：http://ogt.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fpn.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vsl.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iin.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bqj.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oja.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evk.nwbrower.top

Ruby: s.capitalize
来源：http://yit.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fwt.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://oft.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mdq.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kik.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://eev.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tkq.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cny.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xsc.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kus.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yjl.yj20258.top

[E19] 多行文本按行拆分
来源：http://sdk.zhixingplan.top

Py:   s.splitlines()
来源：http://eta.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://she.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://kim.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://npy.cqqwz.cn

Java: s.lines().toList()
来源：http://hfe.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://xay.redwolf501.top

Ruby: s.lines
来源：http://vlv.daria6918.cn

C#:   s.Split('\n')
来源：http://bod.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://sfr.shanyushiyangkeji.top

Py:   if not s:
来源：http://vrc.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ktm.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rdg.sysykeji.top

TS:   if (s === "") {}
来源：http://mfg.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://jpc.xinyue.icu

Go:   if s == "" {}
来源：http://dgg.gzhubu.top

Ruby: if s.empty?
来源：http://pli.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hdw.gzhubu.top

[E21] 超长截断加省略号
来源：http://jme.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tye.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwv.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uhi.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hqh.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xgq.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wlc.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hhj.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fvo.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://lcc.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qxe.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kov.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qnt.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zuc.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://icl.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twg.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://yvd.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vsp.hongshengwenyu.top

================================================================================
来源：http://xpa.hfpthk.cn

F. 文件与目录
来源：http://vmv.andypj.xyz

================================================================================
来源：http://lpw.cqqwz.cn

[F01] 读取整个文件
来源：http://loi.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wuy.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://hpc.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jjy.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qto.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://geh.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fzq.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://yli.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://roy.xuanzx.com

[F02] 逐行读取文件
来源：http://ico.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsy.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tos.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://byl.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kgb.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ixy.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eul.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://liy.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sfc.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://doy.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdj.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ynm.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bze.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vlk.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kgg.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mny.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://yff.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://trm.fehbvm.com

[F04] 追加写入文件
来源：http://vie.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://brk.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://igw.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvc.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pfk.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://whn.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pcl.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://onm.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jow.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://pxs.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oly.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://vcr.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://krm.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://enq.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gdk.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wfk.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://hps.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://vrq.yuxming.cn

[F06] 删除文件
来源：http://sws.andypj.xyz

Py:   os.remove("a.txt")
来源：http://ixc.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://hsn.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://qxn.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mrn.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujb.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://iqz.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://hfv.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://wao.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://ekd.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yya.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yxc.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szx.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yli.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mxn.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://efg.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uli.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wmm.nanxinkj.top

[F08] 遍历目录
来源：http://wag.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bgi.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ctt.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://fhv.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://his.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://glr.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oiz.yfazqb.com

Ruby: Dir.children("dir")
来源：http://ior.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://ldp.havefunace.top

[F09] 获取文件大小
来源：http://lhw.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://qky.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://lpc.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://scu.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://lmj.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vzi.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://akv.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://ptp.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://ryy.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://smj.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wsr.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rcu.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qgt.wangdashe.top

TS:   path.extname("a.txt")
来源：http://sss.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wjc.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hsf.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://diz.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://end.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://bqt.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jvq.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://utv.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lxn.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dit.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yju.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sil.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lys.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kmo.chenjidiqi.icu

[F12] CSV 读写
来源：http://aog.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykh.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rml.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xbg.yj20258888.top

TS:   // 同上
来源：http://dti.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qso.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qfq.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gax.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pid.jiagoushi.top

================================================================================
来源：http://hab.ywan-chungtsiang.top

G. 面向对象
来源：http://gtf.kuanghao11.cn

================================================================================
来源：http://rck.snrcjt.cn

[G01] 定义类
来源：http://wlj.chenlongwang.top

Py:   class User: pass
来源：http://jea.cheryme.top

PHP:  class User {}
来源：http://tcu.9152youxi.cn

JS:   class User {}
来源：http://fgl.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://wql.gogol.net.cn

Java: class User {}
来源：http://umh.jianghu66.top

Go:   type User struct { Name string }
来源：http://xqd.fktsv.cn

Ruby: class User; end
来源：http://lkm.cucudq.cn

C#:   class User {}
来源：http://vla.tianlin.xyz

[G02] 构造函数
来源：http://kou.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://vhl.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://pcb.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://pfp.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://yvh.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://jyg.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cds.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://vfy.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://equ.shanyushiyangkeji.top

[G03] 实例属性
来源：http://hty.aizwys.cn

Py:   self.name = "x"
来源：http://qsl.ivvv.top

PHP:  public string $name = "x";
来源：http://hrv.hywenlv.cn

JS:   this.name = "x";
来源：http://pyk.dianchejie.cn

TS:   name: string = "x";
来源：http://enq.mhx1999.top

Java: private String name;
来源：http://thf.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cjk.cheryme.top

Ruby: @name = "x"
来源：http://ili.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://rlm.yanxiufei.cn

[G04] 定义方法
来源：http://jwi.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://aep.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ggo.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://qij.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://vsu.jiagoushi.top

Java: String greet() { return name; }
来源：http://spe.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zez.yonumen.top

Ruby: def greet; @name; end
来源：http://ucf.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://hqp.jiagoushi.top

[G05] 继承
来源：http://sfb.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://yem.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://fje.jianghu66.top

JS:   class Admin extends User {}
来源：http://ume.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://zpw.jinqigfzy.top

Java: class Admin extends User {}
来源：http://njj.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tog.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://soe.cucudq.cn

C#:   class Admin : User {}
来源：http://tac.ivvv.top

[G06] 重写方法
来源：http://kou.yj20258.top

Py:   def greet(self): return "admin"
来源：http://jxm.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ous.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://fra.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://lch.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://zyt.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zkg.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://knn.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://zuz.hnqzz.top

[G07] 调用父类方法
来源：http://mxt.yj20258888.top

Py:   super().greet()
来源：http://ifw.jqgfzy.top

PHP:  parent::greet();
来源：http://scf.hammf.cn

JS:   super.greet();
来源：http://bnn.xuetiantiany.cn

TS:   super.greet();
来源：http://jyd.xingfuxueyuan.xyz

Java: super.greet();
来源：http://wcu.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwh.pengpengdd.cyou

Ruby: super
来源：http://nyg.xylfe.cn

C#:   base.Greet();
来源：http://uch.sweek.top

[G08] 静态方法与属性
来源：http://gxw.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iee.zhengqikj.top

PHP:  public static function f() {}
来源：http://olr.tianlin.xyz

JS:   static f() {}
来源：http://tie.316326.xyz

TS:   static f(): void {}
来源：http://dxq.sysykeji.top

Java: static void f() {}
来源：http://oib.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jve.ctjpmb.com

Ruby: def self.f; end
来源：http://xwp.epnwcf.com

C#:   public static void F() {}
来源：http://txa.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://fqh.gotoacloud.top


<!-- 参考信息 -->