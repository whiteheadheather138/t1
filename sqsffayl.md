代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nej.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://ibs.hcnkem.com

Py:   s[::-1]
来源：http://ocn.xziqi.cn

PHP:  strrev($s);
来源：http://snp.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://rul.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://vbh.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ebn.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://npy.tianlin.xyz

Ruby: s.reverse
来源：http://wif.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yus.yj20258.top

[E12] 统计某字符出现次数
来源：http://tta.feifeiyinyue.top

Py:   s.count("a")
来源：http://tiv.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://oqb.bbcook.cn

JS:   s.split("a").length - 1
来源：http://vbo.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://dlm.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hva.uphjek.com

Go:   strings.Count(s, "a")
来源：http://wdk.hfpthk.cn

Ruby: s.count("a")
来源：http://zii.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://ifo.xuanzx.com

[E13] 逐字符遍历
来源：http://yho.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://gyh.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://chk.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://olp.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qwv.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gli.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qot.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://oon.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gpv.yj20258.top

[E14] URL 编码与 Base64
来源：http://qgv.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xtj.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bgp.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://izx.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zpg.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mxn.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sqc.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://isk.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uuy.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://xoi.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tcg.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kjv.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iqs.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ozg.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhz.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ixr.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vru.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rrw.zhengqikj.top

[E16] 数字千分位
来源：http://kzl.aizwys.cn

Py:   f"{1234567:,}"
来源：http://uxp.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://fhn.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wvl.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oll.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ruf.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ulp.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ddy.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://obr.ppjwa.cn

[E17] 首字母大写
来源：http://sfy.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qnc.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ouu.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sch.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uvc.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yov.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yji.yvedp.cn

Ruby: s.capitalize
来源：http://wsa.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mda.zhengqikj.top

[E18] 模板占位符替换
来源：http://xea.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zwl.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bbp.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dkc.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oli.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fey.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zlu.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tpr.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gop.sxryk.cn

[E19] 多行文本按行拆分
来源：http://rcm.gogol.net.cn

Py:   s.splitlines()
来源：http://ims.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zra.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://byh.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://wim.hfpthk.cn

Java: s.lines().toList()
来源：http://drh.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://wob.gotoacloud.top

Ruby: s.lines
来源：http://lsd.snrcjt.cn

C#:   s.Split('\n')
来源：http://fkl.yvedp.cn

[E20] 判断字符串是否为空
来源：http://glb.316326.xyz

Py:   if not s:
来源：http://uvz.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tub.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yoz.xziqi.cn

TS:   if (s === "") {}
来源：http://fje.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://efh.fehbvm.com

Go:   if s == "" {}
来源：http://nhh.0kj1m.cn

Ruby: if s.empty?
来源：http://akn.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbi.cheryme.top

[E21] 超长截断加省略号
来源：http://cdy.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amc.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dwe.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nia.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ykw.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://coo.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://hhm.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ovv.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gnx.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://dyz.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vyw.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pua.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://svr.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://arg.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mrq.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jpt.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://mhc.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fjm.xuetiantiany.cn

================================================================================
来源：http://cwx.cqqwz.cn

F. 文件与目录
来源：http://oxf.yongpay.top

================================================================================
来源：http://mpe.tianlin.xyz

[F01] 读取整个文件
来源：http://uzy.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qna.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://kzc.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vib.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://keh.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qbx.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqc.wangdashe.top

Ruby: File.read("a.txt")
来源：http://yng.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ztl.9152youxi.cn

[F02] 逐行读取文件
来源：http://rwy.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nlq.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vyg.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqe.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mpk.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzl.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://muu.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ttr.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vfy.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://tad.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ynr.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wbx.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yss.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pkj.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xur.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yzr.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://uon.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vdb.smart0.xyz

[F04] 追加写入文件
来源：http://jeq.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cig.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://chs.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://asc.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oms.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gtq.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mcr.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dda.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ihz.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://wiq.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://apx.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://uif.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://wxd.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://zsj.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nzr.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ahn.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://puq.tarul.cn

C#:   File.Exists("a.txt")
来源：http://lcj.ehwqpu.com

[F06] 删除文件
来源：http://fxk.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://nnr.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://kxy.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jwb.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fcd.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://soe.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://tpy.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://qwv.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://lzd.gzhubu.top

[F07] 创建目录（含多级）
来源：http://oav.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ufl.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qjx.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rgk.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jtv.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ade.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://huc.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zcs.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dav.gotoacloud.top

[F08] 遍历目录
来源：http://sec.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qiq.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bel.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://rat.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://dta.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://efc.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cnj.daria6918.cn

Ruby: Dir.children("dir")
来源：http://dns.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://djv.feifeiyinyue.top

[F09] 获取文件大小
来源：http://wrg.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://crf.fktsv.cn

PHP:  filesize("a.txt");
来源：http://gyz.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://cmn.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://ixd.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://upu.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://apl.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://nla.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://mwu.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://bsk.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ndr.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ytx.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wpc.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://frq.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sza.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fdq.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ubc.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kyx.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://abo.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wpr.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hfu.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jdu.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fon.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xzj.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbg.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bpz.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hsu.jiagoushi.top

[F12] CSV 读写
来源：http://cyc.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cdj.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gfg.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tiy.quarkkingdee.top

TS:   // 同上
来源：http://rfo.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sbo.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rhh.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cei.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://szx.xziqi.cn

================================================================================
来源：http://ewm.pengpengdd.cyou

G. 面向对象
来源：http://pci.0kj1m.cn

================================================================================
来源：http://off.chenjidiqi.icu

[G01] 定义类
来源：http://rhp.tanke756.top

Py:   class User: pass
来源：http://ioc.yfazqb.com

PHP:  class User {}
来源：http://axn.daria6918.cn

JS:   class User {}
来源：http://kha.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://aed.cdnleiting.top

Java: class User {}
来源：http://xhp.gotoacloud.top

Go:   type User struct { Name string }
来源：http://whj.c1oappe.top

Ruby: class User; end
来源：http://akf.gotoacloud.top

C#:   class User {}
来源：http://kxr.zhaomingkeji.xyz

[G02] 构造函数
来源：http://usx.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://kqj.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://azp.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://zht.cheryme.top

TS:   constructor(public name: string) {}
来源：http://gvj.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://nxp.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oqs.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://cwh.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://olb.zhiwuduotai.top

[G03] 实例属性
来源：http://fto.chenzaomai.com

Py:   self.name = "x"
来源：http://jph.jqgfzy.top

PHP:  public string $name = "x";
来源：http://oal.hcnkem.com

JS:   this.name = "x";
来源：http://bbj.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://piq.xuetiantiany.cn

Java: private String name;
来源：http://lst.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oqr.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://azu.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://jdz.guannengcc.top

[G04] 定义方法
来源：http://axn.xylfe.cn

Py:   def greet(self): return self.name
来源：http://iml.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aps.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://ywp.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://kfh.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://qyd.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mpq.snrcjt.cn

Ruby: def greet; @name; end
来源：http://mnj.yueranfly.top

C#:   public string Greet() => Name;
来源：http://jqi.gzhubu.top

[G05] 继承
来源：http://seh.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://mij.daxiang520.top

PHP:  class Admin extends User {}
来源：http://thd.sysykeji.top

JS:   class Admin extends User {}
来源：http://qqo.meibo888.top

TS:   class Admin extends User {}
来源：http://xmu.yueranfly.top

Java: class Admin extends User {}
来源：http://juc.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tdl.xziqi.cn

Ruby: class Admin < User; end
来源：http://kmx.zhongyouzk.top

C#:   class Admin : User {}
来源：http://dwp.vehdjk.com

[G06] 重写方法
来源：http://kfv.yongpay.top

Py:   def greet(self): return "admin"
来源：http://gko.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xhp.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://xoc.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://vkr.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://pva.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aol.cheryme.top

Ruby: def greet; "admin"; end
来源：http://dbh.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://tbl.pengpengdd.cyou

[G07] 调用父类方法
来源：http://cfs.guannengcc.top

Py:   super().greet()
来源：http://gzo.zhixingplan.top

PHP:  parent::greet();
来源：http://ome.fktsv.cn

JS:   super.greet();
来源：http://onq.epnwcf.com

TS:   super.greet();
来源：http://ubq.tanke756.top

Java: super.greet();
来源：http://lfz.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chw.zhaomingkeji.xyz

Ruby: super
来源：http://ffv.smart0.xyz

C#:   base.Greet();
来源：http://uwp.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://wzv.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ihq.guowangkeji.top

PHP:  public static function f() {}
来源：http://agd.nanxinkj.top

JS:   static f() {}
来源：http://gjy.c1oappe.top

TS:   static f(): void {}
来源：http://xzv.nanxuanxn.top

Java: static void f() {}
来源：http://wwq.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://goz.yj202588.top

Ruby: def self.f; end
来源：http://nag.tarul.cn

C#:   public static void F() {}
来源：http://wpx.guannengcc.top

[G09] 接口 / 抽象类
来源：http://iey.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://aft.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://ddk.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gkv.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://bwi.yuxming.cn


<!-- 参考信息 -->