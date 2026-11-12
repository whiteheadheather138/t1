代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nro.wangdashe.top

[E11] 反转字符串
来源：http://aaf.jianghu66.top

Py:   s[::-1]
来源：http://npc.xziqi.cn

PHP:  strrev($s);
来源：http://jzv.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://cui.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://rdk.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://leq.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://reg.jinqigufen.top

Ruby: s.reverse
来源：http://eon.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://oxw.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://xwo.tianlin.xyz

Py:   s.count("a")
来源：http://sni.havefunace.top

PHP:  substr_count($s, "a");
来源：http://bwq.gzhubu.top

JS:   s.split("a").length - 1
来源：http://ygl.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://iuq.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wcr.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://lep.ctjpmb.com

Ruby: s.count("a")
来源：http://oci.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://myz.svipenyu.cn

[E13] 逐字符遍历
来源：http://jtd.cheryme.top

Py:   for ch in s: print(ch)
来源：http://pqx.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://epq.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nch.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vui.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qbl.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wub.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://moi.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xxh.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://aww.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ejr.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ubl.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mhg.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gjs.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pli.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cyd.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://inf.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gcm.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://rhg.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mcz.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vte.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epq.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lnx.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wgh.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bmh.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zsk.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://egy.yanxiufei.cn

[E16] 数字千分位
来源：http://ruf.wangdashe.top

Py:   f"{1234567:,}"
来源：http://nco.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://sst.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pub.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://czn.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xbd.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://prb.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bpa.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://ntd.shanyushiyangtech.top

[E17] 首字母大写
来源：http://dqx.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xjx.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eoz.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ldz.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rnw.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rky.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lwo.epnwcf.com

Ruby: s.capitalize
来源：http://sxx.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rue.fzhhl.top

[E18] 模板占位符替换
来源：http://wet.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qtz.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rkv.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ikt.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://avp.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hih.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rfp.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://foz.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ira.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://eil.feifeiyinyue.top

Py:   s.splitlines()
来源：http://hms.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fzj.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://ebw.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://opy.ivvv.top

Java: s.lines().toList()
来源：http://aae.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://veh.hywenlv.cn

Ruby: s.lines
来源：http://llv.tian-w.cn

C#:   s.Split('\n')
来源：http://hex.guannengcc.top

[E20] 判断字符串是否为空
来源：http://qfl.hnxiangtu.top

Py:   if not s:
来源：http://zhw.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wnj.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vin.hammf.cn

TS:   if (s === "") {}
来源：http://sji.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://cel.c1oappe.top

Go:   if s == "" {}
来源：http://hat.yj20258.top

Ruby: if s.empty?
来源：http://qzc.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rkl.fengsongda.top

[E21] 超长截断加省略号
来源：http://kly.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ozy.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wdv.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsm.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nte.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dby.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://kdi.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hpk.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://niv.fzhhl.top

[E22] 字节长度与字符长度
来源：http://ddd.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ocg.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kqw.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zzc.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyw.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dkn.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pxi.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://ipp.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbs.vqdsnc.cn

================================================================================
来源：http://zas.chenlongwang.top

F. 文件与目录
来源：http://boj.tanke756.top

================================================================================
来源：http://jcw.hfpthk.cn

[F01] 读取整个文件
来源：http://hkj.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hfy.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://hmg.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pja.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fmp.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://roy.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://roj.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://zcv.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://mem.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://jsz.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nvp.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dot.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sol.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ydk.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://unk.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxu.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ypf.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fsr.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://ion.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iyh.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fvl.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgx.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bue.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://upf.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lrf.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://iln.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wsm.yanxiufei.cn

[F04] 追加写入文件
来源：http://vje.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ikz.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uei.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdb.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjw.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://err.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lzb.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tvm.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://twm.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://yqd.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yki.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://ywr.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://gcv.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://qrv.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://utr.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sjx.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://bxd.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://lsx.sjlbkw.cn

[F06] 删除文件
来源：http://dns.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://zkm.gzhubu.top

PHP:  unlink("a.txt");
来源：http://nnu.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lzs.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://kbg.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvd.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://aph.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://yoz.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://ytf.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://rjo.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tmm.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fvh.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hla.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vwx.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mmg.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gtz.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gri.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sff.hongshengwenyu.top

[F08] 遍历目录
来源：http://kmu.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://den.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hag.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://tjb.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://jmw.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rxl.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://beb.yueranfly.top

Ruby: Dir.children("dir")
来源：http://kbu.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://yky.kuanghao11.cn

[F09] 获取文件大小
来源：http://pbr.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://utj.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://xns.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://tss.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://dfe.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://cjg.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pud.gzhubu.top

Ruby: File.size("a.txt")
来源：http://hli.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://pyi.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://mwj.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wzz.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqh.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wqu.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://utu.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nsp.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jif.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tln.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rjo.sjlbkw.cn

[F11] 复制与移动文件
来源：http://fuz.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qbi.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gxy.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fhj.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxz.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dur.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yyq.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hkw.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yla.yueranfly.top

[F12] CSV 读写
来源：http://ezu.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://miu.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xkp.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ekt.cashguo.top

TS:   // 同上
来源：http://ddy.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kpl.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ywd.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ehc.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mfq.fktsv.cn

================================================================================
来源：http://wfq.9152youxi.cn

G. 面向对象
来源：http://ipz.meibo888.top

================================================================================
来源：http://pon.haohaochexian.top

[G01] 定义类
来源：http://ggd.quarkkingdee.top

Py:   class User: pass
来源：http://xkr.hfpthk.cn

PHP:  class User {}
来源：http://ghe.316326.xyz

JS:   class User {}
来源：http://cxz.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://mxe.jinqigfzy.top

Java: class User {}
来源：http://tpy.yongpay.top

Go:   type User struct { Name string }
来源：http://whx.shangyingyoupin.top

Ruby: class User; end
来源：http://vlb.hywenlv.cn

C#:   class User {}
来源：http://zxo.zhengqikj.top

[G02] 构造函数
来源：http://joc.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wlo.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://jmp.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://aqx.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://qcz.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://gpu.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myu.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://gej.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://zqt.xinyue.icu

[G03] 实例属性
来源：http://yzu.cdnleiting.top

Py:   self.name = "x"
来源：http://tlt.wangdashe.top

PHP:  public string $name = "x";
来源：http://vcu.jiagoushi.top

JS:   this.name = "x";
来源：http://hlg.gaohongyu789.top

TS:   name: string = "x";
来源：http://izq.chenlongwang.top

Java: private String name;
来源：http://nkp.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zdj.svipenyu.cn

Ruby: @name = "x"
来源：http://kmd.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://mjm.shuidangran.top

[G04] 定义方法
来源：http://psh.tarul.cn

Py:   def greet(self): return self.name
来源：http://fua.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://bqh.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://vqz.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://dfq.hnqzz.top

Java: String greet() { return name; }
来源：http://rhx.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pfd.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://pfo.cashguo.top

C#:   public string Greet() => Name;
来源：http://wgx.haohaochexian.top

[G05] 继承
来源：http://ncm.meibo888.top

Py:   class Admin(User): pass
来源：http://udc.yongpay.top

PHP:  class Admin extends User {}
来源：http://fti.birdmap.top

JS:   class Admin extends User {}
来源：http://vfn.cashguo.top

TS:   class Admin extends User {}
来源：http://zxr.gogol.net.cn

Java: class Admin extends User {}
来源：http://lfe.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rti.ppjwa.cn

Ruby: class Admin < User; end
来源：http://vql.hnxiangtu.top

C#:   class Admin : User {}
来源：http://ycb.ybcxt.top

[G06] 重写方法
来源：http://qbe.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://acm.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dvf.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://egi.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://mkv.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://lzf.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eyv.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://cac.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://tju.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://rch.daxiang520.top

Py:   super().greet()
来源：http://xkc.jqgfzy.top

PHP:  parent::greet();
来源：http://cvk.guannengcc.top

JS:   super.greet();
来源：http://nji.smart0.xyz

TS:   super.greet();
来源：http://dio.epnwcf.com

Java: super.greet();
来源：http://uoc.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eaz.jiagoushi.top

Ruby: super
来源：http://qet.bjfxy.top

C#:   base.Greet();
来源：http://kcl.c1oappe.top

[G08] 静态方法与属性
来源：http://qyd.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://twp.guowangkeji.top

PHP:  public static function f() {}
来源：http://gat.hcnkem.com

JS:   static f() {}
来源：http://cxt.yonumen.top

TS:   static f(): void {}
来源：http://ggu.havefunace.top

Java: static void f() {}
来源：http://lea.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fuj.gotoacloud.top

Ruby: def self.f; end
来源：http://njk.cashguo.top

C#:   public static void F() {}
来源：http://lqo.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://zen.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://wbv.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://dln.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mkm.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://jjq.epnwcf.com


<!-- 参考信息 -->