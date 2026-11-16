代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://vmp.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qju.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ewk.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://ssq.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://rnn.sxryk.cn

Java: String.format("%03d", 7)
来源：http://zsk.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vrr.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zbi.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ycx.fengsongda.top

[E11] 反转字符串
来源：http://vtg.fzhhl.top

Py:   s[::-1]
来源：http://hnf.cqqwz.cn

PHP:  strrev($s);
来源：http://vbo.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://pze.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://xpy.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gep.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sen.havefunace.top

Ruby: s.reverse
来源：http://lhb.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://bkv.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://pmq.yuanzhike.top

Py:   s.count("a")
来源：http://bgv.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://asz.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://mfj.fzhhl.top

TS:   s.split("a").length - 1
来源：http://djj.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hfe.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://hps.jianghu66.top

Ruby: s.count("a")
来源：http://uvw.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://vie.yangfankeji.com

[E13] 逐字符遍历
来源：http://eme.uphjek.com

Py:   for ch in s: print(ch)
来源：http://pzx.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nkh.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://drb.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://etu.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ixn.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uep.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kaf.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://slu.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://aes.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qwe.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bfz.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xiz.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fkb.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qqs.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://knv.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uol.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://txe.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://qei.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nmm.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://snc.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wjr.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vji.c1oappe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nzw.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://emx.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bbj.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oft.ctjpmb.com

[E16] 数字千分位
来源：http://fqj.sysykeji.top

Py:   f"{1234567:,}"
来源：http://rxr.guowangkeji.top

PHP:  number_format(1234567);
来源：http://bpe.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gxw.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://chh.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ojx.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gbu.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sho.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://rfq.jinghuilouyu.cn

[E17] 首字母大写
来源：http://uqb.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nuu.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ish.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vul.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://orp.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rys.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gna.birdmap.top

Ruby: s.capitalize
来源：http://zwx.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwo.tarul.cn

[E18] 模板占位符替换
来源：http://bro.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sxn.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tqo.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ymo.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dqr.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ljn.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tph.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wih.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dvj.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://kfj.jqgfzy.top

Py:   s.splitlines()
来源：http://poi.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jrn.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://rta.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://jrq.ctjpmb.com

Java: s.lines().toList()
来源：http://xwa.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://anc.fengsongda.top

Ruby: s.lines
来源：http://sne.zhijiandao.cn

C#:   s.Split('\n')
来源：http://qjm.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://lio.bbcook.cn

Py:   if not s:
来源：http://piu.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kvu.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nyf.uphjek.com

TS:   if (s === "") {}
来源：http://otq.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://ghb.tarul.cn

Go:   if s == "" {}
来源：http://rlm.xylfe.cn

Ruby: if s.empty?
来源：http://mjo.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aov.zhengqikj.top

[E21] 超长截断加省略号
来源：http://ymw.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vrr.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ens.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxc.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsu.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oop.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://igd.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pxh.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gmf.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://rqi.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hxn.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nio.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dtk.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://faf.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mps.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ava.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://eez.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xmx.redwolf501.top

================================================================================
来源：http://tkd.xingfuxueyuan.xyz

F. 文件与目录
来源：http://hak.guowangkeji.top

================================================================================
来源：http://ktx.xziqi.cn

[F01] 读取整个文件
来源：http://npe.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ynk.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://aat.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yyc.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pdn.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lhn.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gdx.guannengcc.top

Ruby: File.read("a.txt")
来源：http://beb.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://eim.ctjpmb.com

[F02] 逐行读取文件
来源：http://vmo.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tzj.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yii.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbi.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://joi.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hob.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://daf.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nqd.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://toy.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://dcp.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ilf.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jtn.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pwi.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jvy.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://urn.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iup.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://tff.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dvv.0kj1m.cn

[F04] 追加写入文件
来源：http://htk.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://epy.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpd.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvc.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ail.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ftc.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://crp.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvi.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://voq.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://xfs.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nhh.havefunace.top

PHP:  file_exists("a.txt");
来源：http://uoq.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://hkn.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://esq.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mqi.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qkh.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://jvc.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://aws.yj20258.top

[F06] 删除文件
来源：http://vgq.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://whw.fengsongda.top

PHP:  unlink("a.txt");
来源：http://ygn.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://qag.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://blq.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://quv.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://wez.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://srf.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://nvm.hammf.cn

[F07] 创建目录（含多级）
来源：http://rcc.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://grv.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cax.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zse.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrh.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uua.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://btw.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://udm.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ugs.hfpthk.cn

[F08] 遍历目录
来源：http://vsc.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zmz.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://etl.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://bai.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://ofg.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gzy.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://flh.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://lin.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://vqd.dianchejie.cn

[F09] 获取文件大小
来源：http://prd.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://hmw.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://hsk.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://ukn.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://yno.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://ygx.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pms.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://mlh.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://fso.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://gcu.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzf.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rac.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nhe.hnqzz.top

TS:   path.extname("a.txt")
来源：http://snj.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cqr.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qhg.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tym.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sux.c1oappe.top

[F11] 复制与移动文件
来源：http://fkd.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nbp.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://duo.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rrt.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rcx.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ygh.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kcc.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mrr.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mga.chenlongwang.top

[F12] CSV 读写
来源：http://kzn.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ftw.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjp.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgd.ydzc1.top

TS:   // 同上
来源：http://dfc.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://njb.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eld.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zww.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://afa.chenzaomai.com

================================================================================
来源：http://ydr.ehwqpu.com

G. 面向对象
来源：http://oyj.iojbl.cn

================================================================================
来源：http://piw.hnqzz.top

[G01] 定义类
来源：http://nwi.fengsongda.top

Py:   class User: pass
来源：http://qzs.yuanzhike.top

PHP:  class User {}
来源：http://nfh.jlsjyb.cn

JS:   class User {}
来源：http://ioi.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://lfq.c1oappe.top

Java: class User {}
来源：http://mzk.gogol.net.cn

Go:   type User struct { Name string }
来源：http://pwn.ywan-chungtsiang.top

Ruby: class User; end
来源：http://vzl.jqgfzy.top

C#:   class User {}
来源：http://rwe.yuxming.cn

[G02] 构造函数
来源：http://vpw.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://voj.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://mlz.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://fwz.birdmap.top

TS:   constructor(public name: string) {}
来源：http://kwp.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://ziw.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://esd.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://blu.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://fcg.xziqi.cn

[G03] 实例属性
来源：http://swk.chenjidiqi.icu

Py:   self.name = "x"
来源：http://pku.ybcxt.top

PHP:  public string $name = "x";
来源：http://mrk.jianghu66.top

JS:   this.name = "x";
来源：http://org.c1oappe.top

TS:   name: string = "x";
来源：http://tap.vqdsnc.cn

Java: private String name;
来源：http://sro.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lul.zhiwuduotai.top

Ruby: @name = "x"
来源：http://pap.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://nlw.snrcjt.cn

[G04] 定义方法
来源：http://cen.daxiang520.top

Py:   def greet(self): return self.name
来源：http://zdb.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cnp.yuxming.cn

JS:   greet() { return this.name; }
来源：http://ahj.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://fsl.yuxming.cn

Java: String greet() { return name; }
来源：http://jzr.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://bmx.mhx1999.top

Ruby: def greet; @name; end
来源：http://sak.xuanzx.com

C#:   public string Greet() => Name;
来源：http://fzy.snrcjt.cn

[G05] 继承
来源：http://nfq.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://swj.hammf.cn

PHP:  class Admin extends User {}
来源：http://abz.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://jbg.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://hkf.gotoacloud.top

Java: class Admin extends User {}
来源：http://wih.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://exk.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://xgk.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://kyu.fktsv.cn

[G06] 重写方法
来源：http://bfe.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://rhv.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://phq.316326.xyz

JS:   greet() { return "admin"; }
来源：http://kts.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://kob.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://wnr.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://maw.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://jsy.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://cpd.chenzaomai.com

[G07] 调用父类方法
来源：http://uxp.birdmap.top

Py:   super().greet()
来源：http://cic.zhijiandao.cn

PHP:  parent::greet();
来源：http://iej.xuetiantiany.cn

JS:   super.greet();
来源：http://dhi.fehbvm.com

TS:   super.greet();
来源：http://pel.jinqigfzy.top

Java: super.greet();
来源：http://krb.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iay.gotoacloud.top

Ruby: super
来源：http://rlw.sjlbkw.cn

C#:   base.Greet();
来源：http://kuf.cheryme.top

[G08] 静态方法与属性
来源：http://det.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lrj.cashguo.top

PHP:  public static function f() {}
来源：http://jiy.shangyingyoupin.top

JS:   static f() {}
来源：http://ycc.yonumen.top

TS:   static f(): void {}
来源：http://yls.tarul.cn

Java: static void f() {}
来源：http://dtz.nanxinkj.top


<!-- 参考信息 -->