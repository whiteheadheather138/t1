代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://xnz.redwolf501.top

Java: String.format("%03d", 7)
来源：http://cgi.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xfq.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://npa.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vlj.cqqwz.cn

[E11] 反转字符串
来源：http://pmp.mhx1999.top

Py:   s[::-1]
来源：http://xad.quarkkingdee.top

PHP:  strrev($s);
来源：http://nfk.havefunace.top

JS:   [...s].reverse().join("")
来源：http://rtd.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://nok.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qxx.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rcx.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://iil.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vao.tian-w.cn

[E12] 统计某字符出现次数
来源：http://iyt.gotoacloud.top

Py:   s.count("a")
来源：http://mvc.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://pmy.xziqi.cn

JS:   s.split("a").length - 1
来源：http://ctk.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://ely.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fyn.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://ndj.redwolf501.top

Ruby: s.count("a")
来源：http://fak.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://wae.ehwqpu.com

[E13] 逐字符遍历
来源：http://rsq.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://hre.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wlz.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zhm.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://clz.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zke.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://grp.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kbe.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ohv.c1oappe.top

[E14] URL 编码与 Base64
来源：http://dtz.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://emd.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://idr.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vlv.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://buc.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ycq.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ska.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zrv.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ktc.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://izm.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hms.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yqr.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rft.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hfq.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://abk.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gwr.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hcg.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cfs.fehbvm.com

[E16] 数字千分位
来源：http://col.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://ras.shzxlz.cn

PHP:  number_format(1234567);
来源：http://chi.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rpa.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dra.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ola.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ams.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sei.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://lkd.pengpengdd.cyou

[E17] 首字母大写
来源：http://pae.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tuh.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://eou.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vci.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vrc.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nzs.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mik.zhixingplan.top

Ruby: s.capitalize
来源：http://pyd.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hez.pycfn.com

[E18] 模板占位符替换
来源：http://xcn.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lil.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cqm.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vtn.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jva.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwf.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://njx.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fhh.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mzd.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://hot.yfazqb.com

Py:   s.splitlines()
来源：http://dnl.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cmi.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://let.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://njp.birdmap.top

Java: s.lines().toList()
来源：http://niw.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://att.tarul.cn

Ruby: s.lines
来源：http://klu.yonumen.top

C#:   s.Split('\n')
来源：http://ebo.c1oappe.top

[E20] 判断字符串是否为空
来源：http://pei.jinqigufen.top

Py:   if not s:
来源：http://cyx.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyo.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://brk.mhx1999.top

TS:   if (s === "") {}
来源：http://kid.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://ccg.yuanzhike.top

Go:   if s == "" {}
来源：http://kgp.zdbjq.cn

Ruby: if s.empty?
来源：http://ylc.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rtg.c1oappe.top

[E21] 超长截断加省略号
来源：http://dqq.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://can.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fqc.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jnw.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcx.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vcx.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://tzr.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lsp.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ceq.fzhhl.top

[E22] 字节长度与字符长度
来源：http://jfb.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://arc.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dvn.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qjq.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://scx.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qgv.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eco.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://ruh.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ybf.shanyushiyangtech.top

================================================================================
来源：http://zur.316326.xyz

F. 文件与目录
来源：http://sug.yuanzhike.top

================================================================================
来源：http://hmt.jiagoushi.top

[F01] 读取整个文件
来源：http://gvx.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oug.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://nwg.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://owi.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ijc.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wer.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://luc.hammf.cn

Ruby: File.read("a.txt")
来源：http://bha.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://moe.cqqwz.cn

[F02] 逐行读取文件
来源：http://llg.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ngi.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kyi.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bwu.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eiw.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mai.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uwl.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xae.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xmj.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://iuu.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://msa.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kaj.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ynt.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhj.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fxm.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ssc.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://jqc.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tmf.jqgufenzy.top

[F04] 追加写入文件
来源：http://qsk.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qca.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zfy.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://joy.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ovg.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://orb.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iqx.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gdc.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pzq.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://eps.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://guf.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://fpf.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://yor.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://sfk.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lec.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vnc.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://umd.sweek.top

C#:   File.Exists("a.txt")
来源：http://ptf.andypj.xyz

[F06] 删除文件
来源：http://yge.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://wdr.tanke756.top

PHP:  unlink("a.txt");
来源：http://kkr.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wnm.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://udz.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fhu.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://yxi.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://ouj.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://jxp.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://xgq.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bhu.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://the.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hni.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pyn.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlx.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xcb.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xqi.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lch.zdbjq.cn

[F08] 遍历目录
来源：http://uam.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qjp.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fkc.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://qfs.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://gnn.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://htj.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tjz.aizwys.cn

Ruby: Dir.children("dir")
来源：http://atp.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://qdw.yangfankeji.com

[F09] 获取文件大小
来源：http://clt.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://tic.yj20258.top

PHP:  filesize("a.txt");
来源：http://gbq.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://knd.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://bts.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://god.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bvy.fzhhl.top

Ruby: File.size("a.txt")
来源：http://ptf.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://cgv.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://pcn.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wpa.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wli.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xpx.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://kbk.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kax.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://myx.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fox.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjy.0kj1m.cn

[F11] 复制与移动文件
来源：http://ddg.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nre.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xfx.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ztq.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fpv.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uca.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ttx.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rvs.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mzt.cheryme.top

[F12] CSV 读写
来源：http://prb.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hgj.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jff.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wnf.ydzc1.top

TS:   // 同上
来源：http://ohx.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://day.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qmz.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cra.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hbj.hfpthk.cn

================================================================================
来源：http://yxs.ywan-chungtsiang.top

G. 面向对象
来源：http://frj.daxiang520.top

================================================================================
来源：http://bqb.iojbl.cn

[G01] 定义类
来源：http://pof.andypj.xyz

Py:   class User: pass
来源：http://zlq.shanyushiyangtech.top

PHP:  class User {}
来源：http://ixv.nanxuanxn.top

JS:   class User {}
来源：http://rzn.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://tpx.sxryk.cn

Java: class User {}
来源：http://aww.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://knb.0kj1m.cn

Ruby: class User; end
来源：http://oba.sufxvd.cn

C#:   class User {}
来源：http://yew.zycfv.cn

[G02] 构造函数
来源：http://uhp.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://dqq.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://lzp.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://ecm.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://oai.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://nye.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyf.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://hyv.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://xvh.yj202588.top

[G03] 实例属性
来源：http://rtl.gogol.net.cn

Py:   self.name = "x"
来源：http://hjn.c1oappe.top

PHP:  public string $name = "x";
来源：http://xgd.svipenyu.cn

JS:   this.name = "x";
来源：http://nol.sysykeji.top

TS:   name: string = "x";
来源：http://iza.fktsv.cn

Java: private String name;
来源：http://lua.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nya.yuxming.cn

Ruby: @name = "x"
来源：http://lrx.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://sgt.chenzaomai.com

[G04] 定义方法
来源：http://xuv.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://mhr.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ayv.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://xar.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://arb.ivvv.top

Java: String greet() { return name; }
来源：http://wzl.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ysl.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://hgt.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://vpg.nwbrower.top

[G05] 继承
来源：http://wtj.guowangkeji.top

Py:   class Admin(User): pass
来源：http://yeu.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://srp.shuidangran.top

JS:   class Admin extends User {}
来源：http://jwm.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://ydw.kuanghao11.cn

Java: class Admin extends User {}
来源：http://jui.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vsj.cashguo.top

Ruby: class Admin < User; end
来源：http://hbs.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://hop.guowangkeji.top

[G06] 重写方法
来源：http://tik.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://rgc.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mlv.yj20258.top

JS:   greet() { return "admin"; }
来源：http://lls.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://wsf.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://atl.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tim.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://ivc.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://euk.dianchejie.cn

[G07] 调用父类方法
来源：http://cem.tanke756.top

Py:   super().greet()
来源：http://nqo.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://ktn.yj20258.top

JS:   super.greet();
来源：http://trz.andypj.xyz

TS:   super.greet();
来源：http://jlj.nanxuanxn.top

Java: super.greet();
来源：http://ouw.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gqy.yongpay.top

Ruby: super
来源：http://hpq.jianghu66.top

C#:   base.Greet();
来源：http://dbr.jiagoushi.top

[G08] 静态方法与属性
来源：http://dpt.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gub.zhongyouzk.top

PHP:  public static function f() {}
来源：http://luo.yfazqb.com

JS:   static f() {}
来源：http://orx.shangyingyoupin.top

TS:   static f(): void {}
来源：http://bwp.fanxiaobao.xyz

Java: static void f() {}
来源：http://nbj.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tiv.hammf.cn

Ruby: def self.f; end
来源：http://hcd.aibaodan.cn

C#:   public static void F() {}
来源：http://vhp.wangdashe.top

[G09] 接口 / 抽象类
来源：http://pnn.wangdashe.top


<!-- 参考信息 -->