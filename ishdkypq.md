代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://fdd.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://onx.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvm.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://ljw.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://sea.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://wnt.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yjn.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llc.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yja.jyoumei.cn

[E11] 反转字符串
来源：http://jir.fzhhl.top

Py:   s[::-1]
来源：http://yen.sxryk.cn

PHP:  strrev($s);
来源：http://tiz.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://ahj.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://djg.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bqw.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eml.tian-w.cn

Ruby: s.reverse
来源：http://ihq.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://kja.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://isp.jinqigfzy.top

Py:   s.count("a")
来源：http://jzr.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://xxn.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://lbj.redwolf501.top

TS:   s.split("a").length - 1
来源：http://pfk.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mlj.cheryme.top

Go:   strings.Count(s, "a")
来源：http://ixh.52xcode.cn

Ruby: s.count("a")
来源：http://dqi.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://xiz.sweek.top

[E13] 逐字符遍历
来源：http://cbg.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://czl.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xsk.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hdf.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gzn.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wuy.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ais.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ipw.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://psy.birdmap.top

[E14] URL 编码与 Base64
来源：http://usm.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://utb.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzi.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rcl.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yio.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pvg.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xmd.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uvu.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ifa.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://kdg.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wxj.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ogr.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nru.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fdc.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://znd.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qpc.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ugg.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.tianlin.xyz

[E16] 数字千分位
来源：http://fiz.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://vfz.fktsv.cn

PHP:  number_format(1234567);
来源：http://ywo.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fkp.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wvz.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wpv.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sts.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ozo.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://pyr.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://oct.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://azd.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://afc.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nhi.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sru.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wds.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kyf.vqdsnc.cn

Ruby: s.capitalize
来源：http://ldw.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rfu.ydjk.org.cn

[E18] 模板占位符替换
来源：http://dqo.hnqzz.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pjh.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://esg.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jog.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xik.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cvw.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tvi.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kjj.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujx.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://lzn.sweek.top

Py:   s.splitlines()
来源：http://kxs.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tsr.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://xel.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://dvu.nanxuanxn.top

Java: s.lines().toList()
来源：http://rzi.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://oxf.zhixingplan.top

Ruby: s.lines
来源：http://roz.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://kbr.yj20258888.top

[E20] 判断字符串是否为空
来源：http://unj.fktsv.cn

Py:   if not s:
来源：http://wmw.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yla.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhd.zhongyouzk.top

TS:   if (s === "") {}
来源：http://duv.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://jlu.yvedp.cn

Go:   if s == "" {}
来源：http://fvn.guowangkeji.top

Ruby: if s.empty?
来源：http://gir.sysykeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://acu.epnwcf.com

[E21] 超长截断加省略号
来源：http://eya.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itc.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lkh.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ems.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbn.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fjq.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://sdm.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vob.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ocl.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://fdn.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://shs.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://muv.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://igg.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fky.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ajh.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://spm.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://hde.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rko.cashguo.top

================================================================================
来源：http://aqd.gotoacloud.top

F. 文件与目录
来源：http://jbr.yueranfly.top

================================================================================
来源：http://zbi.sjlbkw.cn

[F01] 读取整个文件
来源：http://xcw.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ote.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://rny.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mha.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zyk.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sjg.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://trq.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://qvu.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://jjc.yj20258.top

[F02] 逐行读取文件
来源：http://oqu.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zpm.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pms.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imx.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sdk.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://inz.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tjv.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://adh.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lju.havefunace.top

[F03] 写入文件（覆盖）
来源：http://pmp.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ish.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kyv.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcr.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jcc.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ntc.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bsb.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://sek.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wtn.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://qkr.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbq.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zyt.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndy.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imi.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rbl.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ned.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xjd.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://agf.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://nyd.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gun.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://vpu.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://sjz.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://ukl.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://voe.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://elf.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://umr.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://dda.ehwqpu.com

[F06] 删除文件
来源：http://nqg.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://irw.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://tnq.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://wqi.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://noq.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kbg.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://hzd.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://azk.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://nci.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://hmj.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xop.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rdf.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypb.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ajo.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nma.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wbg.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rwi.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yaw.zhoulong.xyz

[F08] 遍历目录
来源：http://ogl.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qpz.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fbj.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://vbu.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://upn.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mfc.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ixq.cucudq.cn

Ruby: Dir.children("dir")
来源：http://yvd.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://vmp.ydzc1.top

[F09] 获取文件大小
来源：http://quv.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://jzq.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://acb.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://rnc.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://awv.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ktw.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fka.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://alh.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://fcq.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://plp.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ehh.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kya.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://txd.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://gus.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uul.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bld.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nfl.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://spo.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://ofp.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bhy.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zwr.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uid.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://poc.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsn.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lon.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oto.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mml.yonumen.top

[F12] CSV 读写
来源：http://aho.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rkd.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ozo.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wci.ivvv.top

TS:   // 同上
来源：http://qzl.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://upq.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qxn.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://grc.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ieh.feifeiyinyue.top

================================================================================
来源：http://osm.xuetiantiany.cn

G. 面向对象
来源：http://ejo.zhijiandao.cn

================================================================================
来源：http://tie.shangyingyoupin.top

[G01] 定义类
来源：http://nrk.epnwcf.com

Py:   class User: pass
来源：http://lfb.xuetiantiany.cn

PHP:  class User {}
来源：http://myn.tarul.cn

JS:   class User {}
来源：http://hfj.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://akm.hongshengwenyu.top

Java: class User {}
来源：http://cjp.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://ych.iojbl.cn

Ruby: class User; end
来源：http://wwn.ppjwa.cn

C#:   class User {}
来源：http://mwt.gogol.net.cn

[G02] 构造函数
来源：http://pod.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://iuo.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://psx.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://drh.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://qpo.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://bmu.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cvj.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://sid.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://lpm.aibaodan.cn

[G03] 实例属性
来源：http://deu.ctjpmb.com

Py:   self.name = "x"
来源：http://bqe.dashuyun.cn

PHP:  public string $name = "x";
来源：http://afo.chenlongwang.top

JS:   this.name = "x";
来源：http://qsz.fehbvm.com

TS:   name: string = "x";
来源：http://iih.gaohongyu789.top

Java: private String name;
来源：http://ruz.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ugs.zhongyouzk.top

Ruby: @name = "x"
来源：http://xgo.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ajw.shuidangran.top

[G04] 定义方法
来源：http://dnr.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://gxu.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fjt.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://zlp.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://upa.aizwys.cn

Java: String greet() { return name; }
来源：http://gmz.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jun.cucudq.cn

Ruby: def greet; @name; end
来源：http://dgf.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://xls.iojbl.cn

[G05] 继承
来源：http://nuk.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://whi.mhx1999.top

PHP:  class Admin extends User {}
来源：http://khx.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://moy.nanxinkj.top

TS:   class Admin extends User {}
来源：http://xff.vqdsnc.cn

Java: class Admin extends User {}
来源：http://khj.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nju.jyoumei.cn

Ruby: class Admin < User; end
来源：http://ltq.zhijiandao.cn

C#:   class Admin : User {}
来源：http://ckm.hnxiangtu.top

[G06] 重写方法
来源：http://bpe.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://nat.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yex.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://vkd.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://esr.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://prr.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyx.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://svd.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://avu.aibaodan.cn

[G07] 调用父类方法
来源：http://adn.zhengqikj.top

Py:   super().greet()
来源：http://ikd.mhx1999.top

PHP:  parent::greet();
来源：http://myl.sxryk.cn

JS:   super.greet();
来源：http://ysi.sysykeji.top

TS:   super.greet();
来源：http://rse.hcnkem.com

Java: super.greet();
来源：http://neb.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jrv.zdbjq.cn

Ruby: super
来源：http://ztz.smart0.xyz

C#:   base.Greet();
来源：http://dlr.ivvv.top

[G08] 静态方法与属性
来源：http://hop.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qxb.yvedp.cn

PHP:  public static function f() {}
来源：http://old.xuetiantiany.cn

JS:   static f() {}
来源：http://dim.jyoumei.cn

TS:   static f(): void {}
来源：http://wja.fzhhl.top

Java: static void f() {}
来源：http://aeg.hfpthk.cn


<!-- 参考信息 -->