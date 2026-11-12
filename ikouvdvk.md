代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://sgu.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://vpo.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://onl.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://odq.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rsc.xylfe.cn

[E11] 反转字符串
来源：http://fel.zhijiandao.cn

Py:   s[::-1]
来源：http://zgq.tanke756.top

PHP:  strrev($s);
来源：http://cev.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://lva.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://unb.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://njy.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wzb.zhiwuduotai.top

Ruby: s.reverse
来源：http://ush.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bym.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://ufa.wangshuangyany.cn

Py:   s.count("a")
来源：http://vya.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://znp.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://ejo.bbcook.cn

TS:   s.split("a").length - 1
来源：http://udr.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gov.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://pto.hesvh.cn

Ruby: s.count("a")
来源：http://ykx.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://apz.aizwys.cn

[E13] 逐字符遍历
来源：http://woz.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://ofk.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ahr.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wlw.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ova.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nkv.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvs.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vly.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rqj.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://nbb.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdu.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohy.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eoi.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lbz.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eya.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdq.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pys.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hol.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://bmw.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://afk.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://asn.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yla.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zue.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://phu.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qqh.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://smk.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rnr.yonumen.top

[E16] 数字千分位
来源：http://pzw.wangdashe.top

Py:   f"{1234567:,}"
来源：http://mqk.hysaishi.cn

PHP:  number_format(1234567);
来源：http://gox.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qfq.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qml.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tta.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hen.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iil.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://nvh.pycfn.com

[E17] 首字母大写
来源：http://plx.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mde.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jny.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ded.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsi.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://odc.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://meb.aibaodan.cn

Ruby: s.capitalize
来源：http://anu.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hzc.cdnleiting.top

[E18] 模板占位符替换
来源：http://xap.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zcr.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dad.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pfn.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ufz.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybf.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aom.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rsw.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://znk.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://omu.0kj1m.cn

Py:   s.splitlines()
来源：http://pwd.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vkd.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://vuk.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://pfo.gaohongyu789.top

Java: s.lines().toList()
来源：http://ess.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://wyy.vehdjk.com

Ruby: s.lines
来源：http://ycq.ybcxt.top

C#:   s.Split('\n')
来源：http://byg.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://raf.nwbrower.top

Py:   if not s:
来源：http://ywt.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvq.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vjz.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://jdr.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://zpq.yonumen.top

Go:   if s == "" {}
来源：http://ldh.andypj.xyz

Ruby: if s.empty?
来源：http://npf.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dph.tianlin.xyz

[E21] 超长截断加省略号
来源：http://myw.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wac.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qby.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyx.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jln.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rpp.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://meq.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://isk.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://esr.fzhhl.top

[E22] 字节长度与字符长度
来源：http://hpy.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ztq.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vam.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mtk.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhn.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hey.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gxu.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://zkn.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cpb.jianghu66.top

================================================================================
来源：http://nri.shanyushiyangkeji.top

F. 文件与目录
来源：http://xga.aibaodan.cn

================================================================================
来源：http://hww.hongshengwenyu.top

[F01] 读取整个文件
来源：http://uxj.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ivi.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://nzv.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gmo.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tfs.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://wyc.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kcn.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://fra.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://snq.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://wdj.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rcs.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mee.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vdu.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxn.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kzf.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mpm.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ehx.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tua.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://txb.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pbw.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbm.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izf.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uks.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eyu.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qaj.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://kyk.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ldt.daria6918.cn

[F04] 追加写入文件
来源：http://kwk.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xgm.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ure.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpc.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sej.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vij.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wjn.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://imr.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kvs.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://xpv.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tdp.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://owu.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://yfy.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://lus.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uiq.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yit.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://clc.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://crk.epnwcf.com

[F06] 删除文件
来源：http://hql.52xcode.cn

Py:   os.remove("a.txt")
来源：http://omq.wangdashe.top

PHP:  unlink("a.txt");
来源：http://ymg.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hku.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vtz.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yqx.yonumen.top

Go:   os.Remove("a.txt")
来源：http://euk.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://oby.316326.xyz

C#:   File.Delete("a.txt");
来源：http://gjt.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://jus.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cuj.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vix.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nxa.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twz.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dpw.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://krs.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rpv.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ekf.hywenlv.cn

[F08] 遍历目录
来源：http://rpr.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://epa.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dgy.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://xnt.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://chd.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ztx.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yul.xziqi.cn

Ruby: Dir.children("dir")
来源：http://eph.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://kcq.sufxvd.cn

[F09] 获取文件大小
来源：http://nyx.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://tvx.havefunace.top

PHP:  filesize("a.txt");
来源：http://ezv.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://qes.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://lmb.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://gpv.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbv.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://lyz.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://eck.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://hbx.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mdd.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xxl.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://voe.smart0.xyz

TS:   path.extname("a.txt")
来源：http://dpj.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ihh.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://swn.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kbc.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lnf.nanxuanxn.top

[F11] 复制与移动文件
来源：http://qks.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xvx.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://erf.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://otc.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gof.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zkp.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jsp.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ybx.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pkz.c1oappe.top

[F12] CSV 读写
来源：http://sjr.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kcc.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wqb.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivx.aizwys.cn

TS:   // 同上
来源：http://wze.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://psc.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pcj.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dtv.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lee.xylfe.cn

================================================================================
来源：http://flh.dashuyun.cn

G. 面向对象
来源：http://zfl.zdqjudy.top

================================================================================
来源：http://rqh.zhaomingkeji.xyz

[G01] 定义类
来源：http://kqb.zhiwuduotai.top

Py:   class User: pass
来源：http://jcg.xuanzx.com

PHP:  class User {}
来源：http://lfp.dianchejie.cn

JS:   class User {}
来源：http://xin.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://iom.yj202588.top

Java: class User {}
来源：http://vvl.guannengcc.top

Go:   type User struct { Name string }
来源：http://cqp.feifeiyinyue.top

Ruby: class User; end
来源：http://rjk.hfpthk.cn

C#:   class User {}
来源：http://scd.guannengcc.top

[G02] 构造函数
来源：http://rfh.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://xiz.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://grp.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://bdm.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://pki.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://fdk.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tno.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://xod.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://mxf.tianlin.xyz

[G03] 实例属性
来源：http://zgb.aibaodan.cn

Py:   self.name = "x"
来源：http://dpb.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://xxz.ppjwa.cn

JS:   this.name = "x";
来源：http://cdo.sjlbkw.cn

TS:   name: string = "x";
来源：http://fwm.tian-w.cn

Java: private String name;
来源：http://wgf.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jph.yj202588.top

Ruby: @name = "x"
来源：http://hbq.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://vns.svipenyu.cn

[G04] 定义方法
来源：http://fhs.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://qsv.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jcq.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://kif.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://mfz.yj202588.top

Java: String greet() { return name; }
来源：http://uib.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xvn.guannengcc.top

Ruby: def greet; @name; end
来源：http://hij.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://bbi.ehwqpu.com

[G05] 继承
来源：http://qkn.guowangkeji.top

Py:   class Admin(User): pass
来源：http://ypo.hesvh.cn

PHP:  class Admin extends User {}
来源：http://bcw.gzhubu.top

JS:   class Admin extends User {}
来源：http://wmz.redwolf501.top

TS:   class Admin extends User {}
来源：http://orr.yuxming.cn

Java: class Admin extends User {}
来源：http://nrp.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wbi.ctjpmb.com

Ruby: class Admin < User; end
来源：http://arw.chenlongwang.top

C#:   class Admin : User {}
来源：http://dxr.vqdsnc.cn

[G06] 重写方法
来源：http://obs.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://ksr.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ynk.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://cuj.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://ucv.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://gyr.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xxk.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://fqo.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://hvo.zhengqikj.top

[G07] 调用父类方法
来源：http://osd.0kj1m.cn

Py:   super().greet()
来源：http://iks.smart0.xyz

PHP:  parent::greet();
来源：http://vyx.zhiwuduotai.top

JS:   super.greet();
来源：http://wxk.pengpengdd.cyou

TS:   super.greet();
来源：http://ojl.mhx1999.top

Java: super.greet();
来源：http://iyd.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rra.cheryme.top

Ruby: super
来源：http://mpb.tarul.cn

C#:   base.Greet();
来源：http://qsk.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://xnv.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jvx.0kj1m.cn

PHP:  public static function f() {}
来源：http://wrc.hnxiangtu.top

JS:   static f() {}
来源：http://goj.cdnleiting.top

TS:   static f(): void {}
来源：http://kin.zhixingplan.top

Java: static void f() {}
来源：http://cyd.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hiz.nanxuanxn.top

Ruby: def self.f; end
来源：http://jtl.fengsongda.top

C#:   public static void F() {}
来源：http://wcr.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://fpa.smart0.xyz


<!-- 参考信息 -->