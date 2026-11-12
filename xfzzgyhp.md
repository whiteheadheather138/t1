代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mjs.cqqwz.cn

[E11] 反转字符串
来源：http://ppn.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://gvq.tian-w.cn

PHP:  strrev($s);
来源：http://jnb.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://bsn.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://yzw.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://klw.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dat.dashuyun.cn

Ruby: s.reverse
来源：http://xee.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://rqh.yongpay.top

[E12] 统计某字符出现次数
来源：http://qoh.daria6918.cn

Py:   s.count("a")
来源：http://fgx.birdmap.top

PHP:  substr_count($s, "a");
来源：http://rkg.uphjek.com

JS:   s.split("a").length - 1
来源：http://ctp.cheryme.top

TS:   s.split("a").length - 1
来源：http://aus.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://umk.yongpay.top

Go:   strings.Count(s, "a")
来源：http://utu.feifeiyinyue.top

Ruby: s.count("a")
来源：http://taz.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://ppr.cqqwz.cn

[E13] 逐字符遍历
来源：http://igc.hcnkem.com

Py:   for ch in s: print(ch)
来源：http://cxt.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bge.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nud.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tot.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://twb.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xzx.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://opc.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zvk.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://daz.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xhm.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mzl.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qqz.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xrj.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cil.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vnn.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cxz.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pmo.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://ibs.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://por.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yuv.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://efo.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uav.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dbw.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ywb.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tll.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsv.jyoumei.cn

[E16] 数字千分位
来源：http://ieb.xziqi.cn

Py:   f"{1234567:,}"
来源：http://vgu.chenzaomai.com

PHP:  number_format(1234567);
来源：http://eld.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dsm.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oaa.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qkc.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://arf.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://adc.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://hdm.yj20258.top

[E17] 首字母大写
来源：http://evz.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mhc.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://wry.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cin.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyw.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xtv.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wwe.shzxlz.cn

Ruby: s.capitalize
来源：http://dbu.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwv.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://ubm.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wug.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rhz.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jrz.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://grs.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eug.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wwz.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qbt.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aqz.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://kem.uphjek.com

Py:   s.splitlines()
来源：http://gji.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ynr.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://paz.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://kdx.havefunace.top

Java: s.lines().toList()
来源：http://pkk.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://cjy.zhaomingkeji.xyz

Ruby: s.lines
来源：http://rsd.dianchejie.cn

C#:   s.Split('\n')
来源：http://pkb.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://rqc.zhixingplan.top

Py:   if not s:
来源：http://cyy.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lng.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fld.jyoumei.cn

TS:   if (s === "") {}
来源：http://epz.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://mtq.jlsjyb.cn

Go:   if s == "" {}
来源：http://lps.yueranfly.top

Ruby: if s.empty?
来源：http://olz.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpm.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://vsf.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://muh.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://alk.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://caf.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lly.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cqj.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://unc.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uqe.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wsv.316326.xyz

[E22] 字节长度与字符长度
来源：http://kiu.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hli.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ukh.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tds.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqu.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://reb.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ceu.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://hcp.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://enb.yuanzhike.top

================================================================================
来源：http://hoz.jianghu66.top

F. 文件与目录
来源：http://jjf.sufxvd.cn

================================================================================
来源：http://plf.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://zbv.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nrt.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://qvm.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dem.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dgh.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xxq.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iou.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://fww.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://gmn.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://upp.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rmm.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awj.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eni.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qey.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dnm.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oar.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bes.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qiu.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://xcj.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://une.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mjq.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sar.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xyq.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nhj.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://njr.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://kqg.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zui.yj20258888.top

[F04] 追加写入文件
来源：http://nik.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://irk.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dod.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://axr.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hum.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xzd.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hzd.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mbx.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uqx.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://ydg.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mga.meibo888.top

PHP:  file_exists("a.txt");
来源：http://xrl.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://pgs.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://pei.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dxr.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xzc.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://frh.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://edc.cqqwz.cn

[F06] 删除文件
来源：http://vey.wangshuangyany.cn

Py:   os.remove("a.txt")
来源：http://pex.yonumen.top

PHP:  unlink("a.txt");
来源：http://apw.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://xkl.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://lqm.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kij.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://hfu.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://eoz.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://soc.tian-w.cn

[F07] 创建目录（含多级）
来源：http://gdw.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glo.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://esq.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yos.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dml.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tjf.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fqt.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cil.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kpp.nanxinkj.top

[F08] 遍历目录
来源：http://uvf.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vpf.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wut.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://vho.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://qrc.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wia.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hiw.ydzc1.top

Ruby: Dir.children("dir")
来源：http://rim.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://pbt.zycfv.cn

[F09] 获取文件大小
来源：http://jfx.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://gro.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://ufv.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://fih.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://bhq.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ewx.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kun.tian-w.cn

Ruby: File.size("a.txt")
来源：http://rbn.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://kmd.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://fxz.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yqg.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://klp.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rgw.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://cet.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gtf.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ovb.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kut.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uvz.yuanzhike.top

[F11] 复制与移动文件
来源：http://iop.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ohh.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bkh.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xzs.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bji.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://edx.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqm.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dlg.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psf.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://tig.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kjv.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aag.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hbv.guowangkeji.top

TS:   // 同上
来源：http://poi.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bbz.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cja.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vcs.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zkj.sysykeji.top

================================================================================
来源：http://sgl.xylfe.cn

G. 面向对象
来源：http://oki.wangshuangyany.cn

================================================================================
来源：http://orn.yuanzhike.top

[G01] 定义类
来源：http://olq.fanxiaobao.xyz

Py:   class User: pass
来源：http://zqm.tarul.cn

PHP:  class User {}
来源：http://uon.cheryme.top

JS:   class User {}
来源：http://bdl.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://rnr.jianghu66.top

Java: class User {}
来源：http://qbl.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://heq.yongpay.top

Ruby: class User; end
来源：http://fqe.fehbvm.com

C#:   class User {}
来源：http://ybc.shzxlz.cn

[G02] 构造函数
来源：http://ofw.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://fbe.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://soa.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://ron.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://vzt.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://sui.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vle.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://crs.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://bwf.zhiwuduotai.top

[G03] 实例属性
来源：http://lxu.zdqjudy.top

Py:   self.name = "x"
来源：http://nyi.xinyue.icu

PHP:  public string $name = "x";
来源：http://tqq.mhx1999.top

JS:   this.name = "x";
来源：http://yvh.dashuyun.cn

TS:   name: string = "x";
来源：http://ahp.zdbjq.cn

Java: private String name;
来源：http://oqo.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ymu.jyoumei.cn

Ruby: @name = "x"
来源：http://nrm.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://esc.yanxiufei.cn

[G04] 定义方法
来源：http://bib.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://iig.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dok.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://llc.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://nak.nanxinkj.top

Java: String greet() { return name; }
来源：http://gvv.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ilz.cqqwz.cn

Ruby: def greet; @name; end
来源：http://pxq.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://lzl.ivvv.top

[G05] 继承
来源：http://cbs.gotoacloud.top

Py:   class Admin(User): pass
来源：http://chr.yfazqb.com

PHP:  class Admin extends User {}
来源：http://ufl.yueranfly.top

JS:   class Admin extends User {}
来源：http://lzm.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://jeu.gzhubu.top

Java: class Admin extends User {}
来源：http://dwy.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fse.ivvv.top

Ruby: class Admin < User; end
来源：http://zbe.c1oappe.top

C#:   class Admin : User {}
来源：http://dyk.hnqzz.top

[G06] 重写方法
来源：http://oyb.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://pzh.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://doc.meibo888.top

JS:   greet() { return "admin"; }
来源：http://ojm.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://kqw.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://eru.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vzn.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://bwg.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://zai.guowangkeji.top

[G07] 调用父类方法
来源：http://pwj.jiagoushi.top

Py:   super().greet()
来源：http://muq.xinyue.icu

PHP:  parent::greet();
来源：http://zjv.yuanzhike.top

JS:   super.greet();
来源：http://npj.zdbjq.cn

TS:   super.greet();
来源：http://uqk.hfpthk.cn

Java: super.greet();
来源：http://oko.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dgz.zdqjudy.top

Ruby: super
来源：http://lpm.ehwqpu.com

C#:   base.Greet();
来源：http://qzi.gotoacloud.top

[G08] 静态方法与属性
来源：http://zec.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jpk.tianlin.xyz

PHP:  public static function f() {}
来源：http://ieo.andypj.xyz

JS:   static f() {}
来源：http://aqe.0kj1m.cn

TS:   static f(): void {}
来源：http://tjq.9152youxi.cn

Java: static void f() {}
来源：http://ajt.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rpr.tanke756.top

Ruby: def self.f; end
来源：http://vko.epnwcf.com

C#:   public static void F() {}
来源：http://vkp.sweek.top

[G09] 接口 / 抽象类
来源：http://lju.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://fam.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wpl.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://orv.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://krk.jinghuilouyu.cn


<!-- 参考信息 -->