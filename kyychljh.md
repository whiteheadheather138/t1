代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://brw.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbi.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xmp.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://otn.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://ole.fengsongda.top

Java: String.format("%03d", 7)
来源：http://mky.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qgn.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://axg.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfw.gotoacloud.top

[E11] 反转字符串
来源：http://oxu.guannengcc.top

Py:   s[::-1]
来源：http://wmk.andypj.xyz

PHP:  strrev($s);
来源：http://ndo.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://rgf.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://gex.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://vpn.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vtf.yangfankeji.com

Ruby: s.reverse
来源：http://cpu.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yzc.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://sfc.zhixingplan.top

Py:   s.count("a")
来源：http://enr.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://tdw.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://cyf.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://bze.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sll.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://wgk.yj202588.top

Ruby: s.count("a")
来源：http://wzp.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://dtv.hnqzz.top

[E13] 逐字符遍历
来源：http://xix.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://ewq.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ull.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lro.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://msv.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tac.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://geo.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wuq.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hwz.yvedp.cn

[E14] URL 编码与 Base64
来源：http://qrf.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://keq.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qpo.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tnr.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dwa.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nlp.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mov.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ete.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://msd.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://qfx.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bsm.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wvh.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jxw.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yqh.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fwi.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wei.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tvp.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zpb.ehwqpu.com

[E16] 数字千分位
来源：http://oyd.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://xcz.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://kux.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pjf.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dqu.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ihy.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mdd.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bgn.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://nou.pycfn.com

[E17] 首字母大写
来源：http://jzh.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gpp.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rvq.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygq.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmj.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fuc.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cbn.shzxlz.cn

Ruby: s.capitalize
来源：http://dvy.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gnk.hcnkem.com

[E18] 模板占位符替换
来源：http://dyh.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cjg.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lux.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ens.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qgz.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bdc.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rkc.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvw.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kuu.wangdashe.top

[E19] 多行文本按行拆分
来源：http://xre.ctjpmb.com

Py:   s.splitlines()
来源：http://awl.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://squ.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://xrl.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://rsh.snrcjt.cn

Java: s.lines().toList()
来源：http://uwk.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://tlr.dashuyun.cn

Ruby: s.lines
来源：http://vtx.yangfankeji.com

C#:   s.Split('\n')
来源：http://hav.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://owe.jlsjyb.cn

Py:   if not s:
来源：http://urq.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ejj.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://guk.guannengcc.top

TS:   if (s === "") {}
来源：http://ikt.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://kze.aizwys.cn

Go:   if s == "" {}
来源：http://tel.nanxuanxn.top

Ruby: if s.empty?
来源：http://hcp.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cpv.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://sky.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tkz.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wdo.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hms.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzp.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://apo.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://auo.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nhf.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ckt.yfazqb.com

[E22] 字节长度与字符长度
来源：http://kyq.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krk.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://met.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehm.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtb.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iay.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qim.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://zbd.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hpv.ydzc1.top

================================================================================
来源：http://vxl.andypj.xyz

F. 文件与目录
来源：http://mep.jqgfzy.top

================================================================================
来源：http://hyb.c1oappe.top

[F01] 读取整个文件
来源：http://cdn.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uuv.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://cpr.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://enn.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rka.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hai.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ubt.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://pfy.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://yyk.yvedp.cn

[F02] 逐行读取文件
来源：http://ipr.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jkl.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vlv.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xec.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zes.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bhm.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hps.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yqs.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bve.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://jkm.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pel.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wwn.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bho.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imx.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bqm.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cbf.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://mmi.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kmh.shzxlz.cn

[F04] 追加写入文件
来源：http://sta.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tup.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hte.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecz.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tev.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uxp.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cqk.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ibb.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ito.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://kzb.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bmq.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://nzv.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://ezu.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://eoe.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dcv.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fko.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://kwl.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://joq.zhengqikj.top

[F06] 删除文件
来源：http://oub.meibo888.top

Py:   os.remove("a.txt")
来源：http://jpc.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://uky.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bis.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://pyj.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dbf.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://ksz.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://utg.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://bnn.cheryme.top

[F07] 创建目录（含多级）
来源：http://uwq.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oet.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://flp.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ytl.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jgs.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sem.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://juf.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gxj.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oca.sxryk.cn

[F08] 遍历目录
来源：http://jym.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://obt.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fod.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://cuc.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://iii.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fjw.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nxg.cashguo.top

Ruby: Dir.children("dir")
来源：http://ymi.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://tng.hywenlv.cn

[F09] 获取文件大小
来源：http://qhf.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://cyd.xylfe.cn

PHP:  filesize("a.txt");
来源：http://unt.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://bno.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://eir.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ler.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ebi.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://mrt.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://qbf.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ouk.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uhm.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dls.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nsg.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://cqh.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzq.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rlj.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tbs.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iik.jyoumei.cn

[F11] 复制与移动文件
来源：http://xkh.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eml.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aax.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rur.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hcq.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bvf.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rfx.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xrh.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xbf.yonumen.top

[F12] CSV 读写
来源：http://bsk.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jng.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jbv.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dyf.shanyushiyangtech.top

TS:   // 同上
来源：http://xgd.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://umc.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfh.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ijk.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ytw.tarul.cn

================================================================================
来源：http://gke.zhengqikj.top

G. 面向对象
来源：http://cua.xziqi.cn

================================================================================
来源：http://asr.tian-w.cn

[G01] 定义类
来源：http://bio.ybcxt.top

Py:   class User: pass
来源：http://abe.jiagoushi.top

PHP:  class User {}
来源：http://ryq.hnxiangtu.top

JS:   class User {}
来源：http://pop.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://kqx.yonumen.top

Java: class User {}
来源：http://zrn.pycfn.com

Go:   type User struct { Name string }
来源：http://ith.bbcook.cn

Ruby: class User; end
来源：http://xqi.jinghuilouyu.cn

C#:   class User {}
来源：http://iku.xziqi.cn

[G02] 构造函数
来源：http://xiw.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://wgb.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://ess.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://olk.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://jdu.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://fgj.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ate.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://ufq.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://lcg.guowangkeji.top

[G03] 实例属性
来源：http://smg.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://blx.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://lbr.fengsongda.top

JS:   this.name = "x";
来源：http://gea.kuanghao11.cn

TS:   name: string = "x";
来源：http://xry.hywenlv.cn

Java: private String name;
来源：http://yvt.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsi.nwbrower.top

Ruby: @name = "x"
来源：http://wla.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://lsp.c1oappe.top

[G04] 定义方法
来源：http://ujn.xziqi.cn

Py:   def greet(self): return self.name
来源：http://lcm.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dhm.ivvv.top

JS:   greet() { return this.name; }
来源：http://lrz.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://ohi.nwbrower.top

Java: String greet() { return name; }
来源：http://vce.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lmf.tian-w.cn

Ruby: def greet; @name; end
来源：http://rgk.nwbrower.top

C#:   public string Greet() => Name;
来源：http://tau.316326.xyz

[G05] 继承
来源：http://mwy.smart0.xyz

Py:   class Admin(User): pass
来源：http://vgn.aizwys.cn

PHP:  class Admin extends User {}
来源：http://tax.xuanzx.com

JS:   class Admin extends User {}
来源：http://xqq.epnwcf.com

TS:   class Admin extends User {}
来源：http://bnd.hnqzz.top

Java: class Admin extends User {}
来源：http://caf.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yke.bjfxy.top

Ruby: class Admin < User; end
来源：http://ipe.fengsongda.top

C#:   class Admin : User {}
来源：http://cbh.shzxlz.cn

[G06] 重写方法
来源：http://ldr.uphjek.com

Py:   def greet(self): return "admin"
来源：http://zlo.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://svt.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://vda.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://jqz.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://prd.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dvo.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://hdc.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://khv.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://ykb.shuidangran.top

Py:   super().greet()
来源：http://lta.ybcxt.top

PHP:  parent::greet();
来源：http://amt.chenjidiqi.icu

JS:   super.greet();
来源：http://lbl.0kj1m.cn

TS:   super.greet();
来源：http://vxh.ppjwa.cn

Java: super.greet();
来源：http://byo.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sax.jyoumei.cn

Ruby: super
来源：http://fus.tian-w.cn

C#:   base.Greet();
来源：http://pcz.sufxvd.cn

[G08] 静态方法与属性
来源：http://jwz.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pay.jqgfzy.top

PHP:  public static function f() {}
来源：http://hho.jianghu66.top

JS:   static f() {}
来源：http://ipi.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://ckt.hysaishi.cn

Java: static void f() {}
来源：http://tea.gzhubu.top


<!-- 参考信息 -->