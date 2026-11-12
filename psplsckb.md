代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://uwa.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://att.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsb.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://nkm.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://wto.52xcode.cn

Java: String.format("%03d", 7)
来源：http://gaa.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://enm.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nig.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pbj.xziqi.cn

[E11] 反转字符串
来源：http://drx.52xcode.cn

Py:   s[::-1]
来源：http://fdq.yueranfly.top

PHP:  strrev($s);
来源：http://lnf.yongpay.top

JS:   [...s].reverse().join("")
来源：http://efj.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://zwl.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mmd.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://jbn.xziqi.cn

Ruby: s.reverse
来源：http://nxt.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://wmo.daria6918.cn

[E12] 统计某字符出现次数
来源：http://bgq.redwolf501.top

Py:   s.count("a")
来源：http://zcm.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://oot.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://rwa.havefunace.top

TS:   s.split("a").length - 1
来源：http://zyt.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gvb.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://asj.guowangkeji.top

Ruby: s.count("a")
来源：http://xwi.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://ggc.gogol.net.cn

[E13] 逐字符遍历
来源：http://apl.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://oxp.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ryq.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mgs.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://flc.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rzv.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hbk.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wez.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyg.yj20258.top

[E14] URL 编码与 Base64
来源：http://oqo.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nap.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qlm.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://btb.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jgk.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ati.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lvr.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gjz.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zid.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://oss.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ffs.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mhm.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lsk.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://oni.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awa.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtt.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://adm.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pee.cdnleiting.top

[E16] 数字千分位
来源：http://qdc.nwbrower.top

Py:   f"{1234567:,}"
来源：http://pav.cashguo.top

PHP:  number_format(1234567);
来源：http://exm.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://bel.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mmc.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eoz.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gnc.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vpi.cashguo.top

C#:   1234567.ToString("N0")
来源：http://dhu.0kj1m.cn

[E17] 首字母大写
来源：http://xby.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mvz.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ehp.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ubv.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://glt.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fhq.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lpx.kuanghao11.cn

Ruby: s.capitalize
来源：http://zif.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qdr.nwbrower.top

[E18] 模板占位符替换
来源：http://wzh.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fib.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://swv.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ztr.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fkl.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://upm.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zwk.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rjs.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nqb.meibo888.top

[E19] 多行文本按行拆分
来源：http://uyr.vqdsnc.cn

Py:   s.splitlines()
来源：http://xuu.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hoz.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://ydo.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://ups.aibaodan.cn

Java: s.lines().toList()
来源：http://ybc.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://sxe.fktsv.cn

Ruby: s.lines
来源：http://ang.nwbrower.top

C#:   s.Split('\n')
来源：http://gzj.ybcxt.top

[E20] 判断字符串是否为空
来源：http://oip.jiagoushi.top

Py:   if not s:
来源：http://duf.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vmg.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://orj.zhoulong.xyz

TS:   if (s === "") {}
来源：http://kil.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://hgf.9152youxi.cn

Go:   if s == "" {}
来源：http://wjg.meibo888.top

Ruby: if s.empty?
来源：http://whl.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zdv.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://zyl.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqu.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ran.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mtx.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vft.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gqo.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://dfy.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rym.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxp.hnqzz.top

[E22] 字节长度与字符长度
来源：http://ttt.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://erm.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xap.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wed.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wyc.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rca.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://igu.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://hsk.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xdm.shuidangran.top

================================================================================
来源：http://goc.c1oappe.top

F. 文件与目录
来源：http://yea.fzhhl.top

================================================================================
来源：http://mhr.fehbvm.com

[F01] 读取整个文件
来源：http://nqr.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qva.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://gbl.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://phj.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bxr.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vgy.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jrf.yueranfly.top

Ruby: File.read("a.txt")
来源：http://szu.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://jlk.52xcode.cn

[F02] 逐行读取文件
来源：http://bcr.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csf.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wtc.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pbi.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oxe.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uxs.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rpk.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukr.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://veq.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://jne.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mfw.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ldx.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pnq.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfn.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wfz.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gjv.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://zdv.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gxu.zhixingplan.top

[F04] 追加写入文件
来源：http://qxw.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yka.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nev.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbz.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oid.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sqy.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cbn.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wrd.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gim.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://wqa.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sal.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://swz.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://vya.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://bgg.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sjz.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hoz.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://rad.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://rtc.9152youxi.cn

[F06] 删除文件
来源：http://jwm.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://mog.hesvh.cn

PHP:  unlink("a.txt");
来源：http://czs.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://usx.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fqg.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udv.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://ivc.meibo888.top

Ruby: File.delete("a.txt")
来源：http://mne.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://ygb.52xcode.cn

[F07] 创建目录（含多级）
来源：http://aum.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kxg.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cvv.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bpn.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ywr.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://azy.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bhl.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oss.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xlo.xinyue.icu

[F08] 遍历目录
来源：http://uev.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dlm.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xmx.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://kar.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://bmj.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ebb.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lzq.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://ooo.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://qte.ybcxt.top

[F09] 获取文件大小
来源：http://wcj.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://xnx.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://wkv.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://gex.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://ivp.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://lly.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nns.52xcode.cn

Ruby: File.size("a.txt")
来源：http://zpm.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://mmb.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ofu.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nbx.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dbx.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qqc.nwbrower.top

TS:   path.extname("a.txt")
来源：http://yog.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jdu.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xit.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sol.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gny.ppjwa.cn

[F11] 复制与移动文件
来源：http://ckt.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wex.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xgt.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbl.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqx.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://msq.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pqm.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rwh.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gxd.pengpengdd.cyou

[F12] CSV 读写
来源：http://rja.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://omi.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pwl.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vyg.yueranfly.top

TS:   // 同上
来源：http://tef.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkb.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhz.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lvk.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bvv.jinqigufen.top

================================================================================
来源：http://rdc.yueranfly.top

G. 面向对象
来源：http://oxp.hnqzz.top

================================================================================
来源：http://fvh.zhaomingkeji.xyz

[G01] 定义类
来源：http://eca.yj202588.top

Py:   class User: pass
来源：http://mkp.ehwqpu.com

PHP:  class User {}
来源：http://ioy.316326.xyz

JS:   class User {}
来源：http://wuv.cashguo.top

TS:   class User { name: string = ""; }
来源：http://ejp.ydzc1.top

Java: class User {}
来源：http://gbw.zdbjq.cn

Go:   type User struct { Name string }
来源：http://vgj.kuanghao11.cn

Ruby: class User; end
来源：http://gvs.feifeiyinyue.top

C#:   class User {}
来源：http://eeg.andypj.xyz

[G02] 构造函数
来源：http://byv.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://wnr.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://fqj.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://qyn.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://uty.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://mnq.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://upq.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://owf.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://amp.fzhhl.top

[G03] 实例属性
来源：http://rkl.bbcook.cn

Py:   self.name = "x"
来源：http://nqf.zhixingplan.top

PHP:  public string $name = "x";
来源：http://cti.zhengqikj.top

JS:   this.name = "x";
来源：http://fmw.xziqi.cn

TS:   name: string = "x";
来源：http://zda.cheryme.top

Java: private String name;
来源：http://zxl.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yfv.ybcxt.top

Ruby: @name = "x"
来源：http://hkr.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://fwx.haohaochexian.top

[G04] 定义方法
来源：http://fsa.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://aig.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://euz.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://nma.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://ynw.jqgfzy.top

Java: String greet() { return name; }
来源：http://zae.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gtr.redwolf501.top

Ruby: def greet; @name; end
来源：http://lmh.sysykeji.top

C#:   public string Greet() => Name;
来源：http://oxc.dashuyun.cn

[G05] 继承
来源：http://hap.redwolf501.top

Py:   class Admin(User): pass
来源：http://ujd.havefunace.top

PHP:  class Admin extends User {}
来源：http://zit.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://jop.hcnkem.com

TS:   class Admin extends User {}
来源：http://zpt.dianchejie.cn

Java: class Admin extends User {}
来源：http://onr.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mkh.guowangkeji.top

Ruby: class Admin < User; end
来源：http://olr.gaohongyu789.top

C#:   class Admin : User {}
来源：http://dhw.jinyuanbaomall.cn

[G06] 重写方法
来源：http://ffb.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://tzt.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gir.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://suw.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://qpd.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://tag.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bbx.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://jeq.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://tkn.hesvh.cn

[G07] 调用父类方法
来源：http://iuq.daria6918.cn

Py:   super().greet()
来源：http://mpk.yj20258888.top

PHP:  parent::greet();
来源：http://enr.fengsongda.top

JS:   super.greet();
来源：http://amq.fengsongda.top

TS:   super.greet();
来源：http://ukx.zdbjq.cn

Java: super.greet();
来源：http://yqt.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://usb.yueranfly.top

Ruby: super
来源：http://iie.jlsjyb.cn

C#:   base.Greet();
来源：http://cwb.ybcxt.top

[G08] 静态方法与属性
来源：http://bth.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fqy.zhongyouzk.top

PHP:  public static function f() {}
来源：http://kku.yangfankeji.com

JS:   static f() {}
来源：http://bni.hcnkem.com

TS:   static f(): void {}
来源：http://ghv.hnqzz.top

Java: static void f() {}
来源：http://xcd.nwbrower.top


<!-- 参考信息 -->