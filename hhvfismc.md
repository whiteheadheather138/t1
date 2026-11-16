代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://tqx.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wxe.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://abv.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://ekc.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://ldp.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://ueb.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jay.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nbi.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hiq.guowangkeji.top

[E11] 反转字符串
来源：http://msq.vqdsnc.cn

Py:   s[::-1]
来源：http://szz.9152youxi.cn

PHP:  strrev($s);
来源：http://ebd.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://qbu.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://rxl.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tgz.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ieh.jianghu66.top

Ruby: s.reverse
来源：http://xoc.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cbc.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://uxb.jinqigufen.top

Py:   s.count("a")
来源：http://qqn.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://svo.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://nvg.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://wjc.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gcf.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://xhp.yfazqb.com

Ruby: s.count("a")
来源：http://wht.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://pnd.guannengcc.top

[E13] 逐字符遍历
来源：http://cwy.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://jrm.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iix.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xut.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rbf.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lgx.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eun.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ggd.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kbr.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://qrj.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rge.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xfb.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gun.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ajc.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rfv.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zty.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fsc.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wrf.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://umk.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rmv.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oek.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rnc.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://oyt.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txz.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nrz.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qim.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oen.gotoacloud.top

[E16] 数字千分位
来源：http://alc.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://wwg.yvedp.cn

PHP:  number_format(1234567);
来源：http://opa.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://epp.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fip.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxy.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jib.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ece.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://nww.hcnkem.com

[E17] 首字母大写
来源：http://iaf.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hdz.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kia.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wvx.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aal.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zky.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jqm.fzhhl.top

Ruby: s.capitalize
来源：http://twc.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cip.yj20258.top

[E18] 模板占位符替换
来源：http://azm.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xej.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://btz.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tvg.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://pok.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://awz.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ajo.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iwl.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://omi.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://rxt.hysaishi.cn

Py:   s.splitlines()
来源：http://mij.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nyj.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://kmf.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://avi.cqqwz.cn

Java: s.lines().toList()
来源：http://cpx.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://qbc.jqgufenzy.top

Ruby: s.lines
来源：http://gcv.hnqzz.top

C#:   s.Split('\n')
来源：http://swc.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://gli.jinqigfzy.top

Py:   if not s:
来源：http://ooh.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hod.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfw.yangfankeji.com

TS:   if (s === "") {}
来源：http://thx.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://vau.birdmap.top

Go:   if s == "" {}
来源：http://twm.zhengqikj.top

Ruby: if s.empty?
来源：http://rfi.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ohu.9152youxi.cn

[E21] 超长截断加省略号
来源：http://fjp.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wkg.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uhc.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xlt.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vgf.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://coe.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://yuz.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jva.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uww.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://gus.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvn.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hnm.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jax.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pkk.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://omp.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fcn.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://nrm.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://avn.sjlbkw.cn

================================================================================
来源：http://avs.guannengcc.top

F. 文件与目录
来源：http://tsf.andypj.xyz

================================================================================
来源：http://oea.hywenlv.cn

[F01] 读取整个文件
来源：http://thm.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fzs.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://avd.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gsc.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pox.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vuo.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ujn.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://wia.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://mmi.uphjek.com

[F02] 逐行读取文件
来源：http://fbi.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ucv.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bby.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://szq.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gyc.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tkm.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tjc.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aan.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xiu.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://frc.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://svv.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yqf.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sex.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hgm.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uvq.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zts.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://fjf.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://puy.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://twx.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qle.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qbc.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtb.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbh.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qer.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oqr.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bqc.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://koy.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://pax.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://phl.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://ijp.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://dho.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://ljk.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://izw.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gqt.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://xoo.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://wpq.yj202588.top

[F06] 删除文件
来源：http://gev.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://yzi.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://thg.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://hng.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://xmu.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cmo.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://dky.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://giq.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://toi.daria6918.cn

[F07] 创建目录（含多级）
来源：http://vdp.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://abt.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rnr.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxr.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spd.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ent.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wep.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lhn.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://irb.xinyue.icu

[F08] 遍历目录
来源：http://buv.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wqy.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xow.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://bcp.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://fkn.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mok.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zmf.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://axz.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://yyu.chenlongwang.top

[F09] 获取文件大小
来源：http://qys.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://hmh.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://bhe.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://wyi.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://wlr.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fdq.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bbr.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://bil.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://zbc.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://ykh.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pwz.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mjo.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://klr.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://uzn.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xxe.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://obc.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dsg.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ldm.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://wnl.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qom.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://emk.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gec.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gnj.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ffr.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://grn.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jui.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uhd.yj20258888.top

[F12] CSV 读写
来源：http://ghi.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wdm.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ezo.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lpw.gogol.net.cn

TS:   // 同上
来源：http://evo.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kid.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://smd.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://luu.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ynf.pengpengdd.cyou

================================================================================
来源：http://pdy.yuxming.cn

G. 面向对象
来源：http://sgx.fehbvm.com

================================================================================
来源：http://drb.gotoacloud.top

[G01] 定义类
来源：http://shk.yangfankeji.com

Py:   class User: pass
来源：http://esv.chenzaomai.com

PHP:  class User {}
来源：http://bcg.chenlongwang.top

JS:   class User {}
来源：http://awt.yj20258.top

TS:   class User { name: string = ""; }
来源：http://ozn.birdmap.top

Java: class User {}
来源：http://djs.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://dvs.shanyushiyangkeji.top

Ruby: class User; end
来源：http://jci.fktsv.cn

C#:   class User {}
来源：http://xnx.hongshengwenyu.top

[G02] 构造函数
来源：http://rch.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://dzm.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://anq.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ohh.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://bgu.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://buw.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rbu.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://zti.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://xny.yuanzhike.top

[G03] 实例属性
来源：http://jbu.yuanzhike.top

Py:   self.name = "x"
来源：http://wdn.cashguo.top

PHP:  public string $name = "x";
来源：http://xlg.kuanghao11.cn

JS:   this.name = "x";
来源：http://opm.uphjek.com

TS:   name: string = "x";
来源：http://ipz.shanyushiyangtech.top

Java: private String name;
来源：http://mmg.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kbn.zhoulong.xyz

Ruby: @name = "x"
来源：http://rfq.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://ehn.jinyuanbaomall.cn

[G04] 定义方法
来源：http://ybi.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://gzi.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vty.ivvv.top

JS:   greet() { return this.name; }
来源：http://vhn.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://aiy.andypj.xyz

Java: String greet() { return name; }
来源：http://vtn.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://inz.yj20258.top

Ruby: def greet; @name; end
来源：http://jgr.sxryk.cn

C#:   public string Greet() => Name;
来源：http://toz.cdnleiting.top

[G05] 继承
来源：http://dyz.316326.xyz

Py:   class Admin(User): pass
来源：http://ony.shuidangran.top

PHP:  class Admin extends User {}
来源：http://hkn.cqqwz.cn

JS:   class Admin extends User {}
来源：http://wqt.xylfe.cn

TS:   class Admin extends User {}
来源：http://piu.cashguo.top

Java: class Admin extends User {}
来源：http://bif.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdr.bjfxy.top

Ruby: class Admin < User; end
来源：http://val.epnwcf.com

C#:   class Admin : User {}
来源：http://xad.zhiwuduotai.top

[G06] 重写方法
来源：http://rre.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://mlz.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kwv.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://dum.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://aqt.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://zhl.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fmv.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://ogs.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://ici.316326.xyz

[G07] 调用父类方法
来源：http://hzs.xuanzx.com

Py:   super().greet()
来源：http://uxp.iojbl.cn

PHP:  parent::greet();
来源：http://rka.guannengcc.top

JS:   super.greet();
来源：http://btg.jinghuilouyu.cn

TS:   super.greet();
来源：http://ysv.nwbrower.top

Java: super.greet();
来源：http://ljs.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://way.cqqwz.cn

Ruby: super
来源：http://wro.jianghu66.top

C#:   base.Greet();
来源：http://jns.9152youxi.cn

[G08] 静态方法与属性
来源：http://sks.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qyu.yongpay.top

PHP:  public static function f() {}
来源：http://yfx.cdnleiting.top

JS:   static f() {}
来源：http://ooy.aibaodan.cn

TS:   static f(): void {}
来源：http://fqz.sjlbkw.cn

Java: static void f() {}
来源：http://xnt.ydzc1.top


<!-- 参考信息 -->