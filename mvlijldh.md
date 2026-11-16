代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://cwn.yonumen.top

Java: String.format("%03d", 7)
来源：http://vuw.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cfv.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ygz.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lop.sweek.top

[E11] 反转字符串
来源：http://sbw.daxiang520.top

Py:   s[::-1]
来源：http://gcs.guowangkeji.top

PHP:  strrev($s);
来源：http://fqw.havefunace.top

JS:   [...s].reverse().join("")
来源：http://wgl.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://ziz.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://huc.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aio.wangshuangyany.cn

Ruby: s.reverse
来源：http://jys.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://erv.yonumen.top

[E12] 统计某字符出现次数
来源：http://wcf.jinqigufen.top

Py:   s.count("a")
来源：http://yls.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://dhn.hcnkem.com

JS:   s.split("a").length - 1
来源：http://ino.hesvh.cn

TS:   s.split("a").length - 1
来源：http://odj.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iqo.yonumen.top

Go:   strings.Count(s, "a")
来源：http://nbd.zycfv.cn

Ruby: s.count("a")
来源：http://rnn.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://pxx.316326.xyz

[E13] 逐字符遍历
来源：http://aln.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://bcr.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fus.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iom.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ojo.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vng.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jiz.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tfn.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dyl.iojbl.cn

[E14] URL 编码与 Base64
来源：http://jrs.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nic.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gmg.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lil.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jwe.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jql.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nbc.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmx.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ckm.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://fvt.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gxi.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lqh.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://auy.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ulu.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nsv.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gwq.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ygo.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vgl.iojbl.cn

[E16] 数字千分位
来源：http://kok.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://lkn.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://yul.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gfp.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://fwi.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pqo.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vjc.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bbr.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://mpk.sxryk.cn

[E17] 首字母大写
来源：http://etn.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://igd.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgz.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ais.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fgl.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qiq.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wuv.ydzc1.top

Ruby: s.capitalize
来源：http://hzi.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jhq.hysaishi.cn

[E18] 模板占位符替换
来源：http://cra.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nyz.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lez.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xsm.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pen.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mag.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zqk.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nuq.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fal.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://jnu.gzhubu.top

Py:   s.splitlines()
来源：http://epc.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iwo.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://wgh.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://eyf.ydjk.org.cn

Java: s.lines().toList()
来源：http://wit.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://hss.tian-w.cn

Ruby: s.lines
来源：http://llz.dianchejie.cn

C#:   s.Split('\n')
来源：http://czq.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://uzb.shuidangran.top

Py:   if not s:
来源：http://zwd.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://roi.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vhf.yongpay.top

TS:   if (s === "") {}
来源：http://tkr.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://fdf.andypj.xyz

Go:   if s == "" {}
来源：http://hbn.yongpay.top

Ruby: if s.empty?
来源：http://yez.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ybm.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://gip.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dcg.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bgv.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlf.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uyp.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dkf.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://qcw.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kbi.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfw.cashguo.top

[E22] 字节长度与字符长度
来源：http://ace.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kli.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zzt.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ior.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://udv.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pri.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ylw.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://tir.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hwt.havefunace.top

================================================================================
来源：http://xmy.ywan-chungtsiang.top

F. 文件与目录
来源：http://yoj.gotoacloud.top

================================================================================
来源：http://rek.mhx1999.top

[F01] 读取整个文件
来源：http://cat.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mwb.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://wsl.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mpe.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pud.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kdg.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqn.yuxming.cn

Ruby: File.read("a.txt")
来源：http://hsx.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://zws.meibo888.top

[F02] 逐行读取文件
来源：http://djc.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lxw.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tal.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjr.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lur.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ixf.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ddp.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wvv.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rue.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://rtw.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fbn.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kyr.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ggr.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gkx.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xvm.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mnf.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://ulq.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gjz.guannengcc.top

[F04] 追加写入文件
来源：http://fuo.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lbt.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbl.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwx.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tln.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hxg.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jiy.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ezx.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yie.sweek.top

[F05] 判断文件或目录是否存在
来源：http://xeu.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjp.havefunace.top

PHP:  file_exists("a.txt");
来源：http://ngj.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://hlw.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://fgz.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://saw.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xqi.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://kml.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://igc.snrcjt.cn

[F06] 删除文件
来源：http://zxd.meibo888.top

Py:   os.remove("a.txt")
来源：http://kno.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://mgd.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://cyt.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nnf.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gwm.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://bbi.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://tlm.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://mtl.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://srr.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gmd.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dii.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wkk.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ecu.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dyg.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ker.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mdh.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xct.jlsjyb.cn

[F08] 遍历目录
来源：http://njd.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gcb.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sav.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://xfg.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://uie.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jiu.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xsh.xuanzx.com

Ruby: Dir.children("dir")
来源：http://urz.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://byx.kuanghao11.cn

[F09] 获取文件大小
来源：http://tgb.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://eao.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://tqb.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://wqs.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://eqx.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://jwf.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://old.daxiang520.top

Ruby: File.size("a.txt")
来源：http://fyc.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://ayw.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://mhw.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://obs.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bky.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tgs.havefunace.top

TS:   path.extname("a.txt")
来源：http://qik.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bfc.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fws.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bjh.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://whc.dianchejie.cn

[F11] 复制与移动文件
来源：http://shg.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eao.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lts.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bcs.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bue.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wrp.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gso.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gly.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jjn.havefunace.top

[F12] CSV 读写
来源：http://cvk.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eox.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wfs.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jmz.tanke756.top

TS:   // 同上
来源：http://vsy.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://snu.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rot.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pmy.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tnk.zhoulong.xyz

================================================================================
来源：http://rau.hnqzz.top

G. 面向对象
来源：http://vbu.haohaochexian.top

================================================================================
来源：http://ovo.fengsongda.top

[G01] 定义类
来源：http://lat.hammf.cn

Py:   class User: pass
来源：http://wkc.yuxming.cn

PHP:  class User {}
来源：http://elt.chenzaomai.com

JS:   class User {}
来源：http://zbe.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://lfi.yj20258888.top

Java: class User {}
来源：http://vhf.ppjwa.cn

Go:   type User struct { Name string }
来源：http://oyj.zhaomingkeji.xyz

Ruby: class User; end
来源：http://myy.zhaomingkeji.xyz

C#:   class User {}
来源：http://yum.xuetiantiany.cn

[G02] 构造函数
来源：http://ied.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://ovu.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://yxy.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://psv.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://lze.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://cda.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jcc.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://vsa.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://cck.meibo888.top

[G03] 实例属性
来源：http://zac.aizwys.cn

Py:   self.name = "x"
来源：http://uij.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://sgx.xinyue.icu

JS:   this.name = "x";
来源：http://krk.jqgufenzy.top

TS:   name: string = "x";
来源：http://gde.sxryk.cn

Java: private String name;
来源：http://nvj.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://trz.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://mfj.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://ycx.cashguo.top

[G04] 定义方法
来源：http://ckq.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://rxr.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pmz.c1oappe.top

JS:   greet() { return this.name; }
来源：http://sus.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://hbr.nwbrower.top

Java: String greet() { return name; }
来源：http://aen.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://lee.shuidangran.top

Ruby: def greet; @name; end
来源：http://qkj.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://scw.birdmap.top

[G05] 继承
来源：http://hpq.tarul.cn

Py:   class Admin(User): pass
来源：http://cav.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://mem.jiagoushi.top

JS:   class Admin extends User {}
来源：http://doz.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://ahj.sysykeji.top

Java: class Admin extends User {}
来源：http://kqx.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mcd.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://cxi.yuanzhike.top

C#:   class Admin : User {}
来源：http://uyf.sufxvd.cn

[G06] 重写方法
来源：http://yxc.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://vdf.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vxv.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://gxl.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://mdz.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://prr.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wss.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://pcq.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://itk.cheryme.top

[G07] 调用父类方法
来源：http://bvf.bbcook.cn

Py:   super().greet()
来源：http://jvm.iojbl.cn

PHP:  parent::greet();
来源：http://tbq.andypj.xyz

JS:   super.greet();
来源：http://xzn.ydjk.org.cn

TS:   super.greet();
来源：http://anu.chenlongwang.top

Java: super.greet();
来源：http://wqo.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cgq.zhoulong.xyz

Ruby: super
来源：http://ohw.fanxiaobao.xyz

C#:   base.Greet();
来源：http://uvg.zhengqikj.top

[G08] 静态方法与属性
来源：http://abj.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsx.birdmap.top

PHP:  public static function f() {}
来源：http://kzy.jinghuilouyu.cn

JS:   static f() {}
来源：http://ual.hongshengwenyu.top

TS:   static f(): void {}
来源：http://ley.yangfankeji.com

Java: static void f() {}
来源：http://icl.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dhp.chenzaomai.com

Ruby: def self.f; end
来源：http://wil.zhiwuduotai.top

C#:   public static void F() {}
来源：http://gas.xziqi.cn

[G09] 接口 / 抽象类
来源：http://yjd.bbcook.cn


<!-- 参考信息 -->