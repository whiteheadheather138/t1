代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://xyr.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wsh.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwv.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://vse.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://nsa.c1oappe.top

Java: String.format("%03d", 7)
来源：http://xmp.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pwa.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lez.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://irs.cdnleiting.top

[E11] 反转字符串
来源：http://ecq.daria6918.cn

Py:   s[::-1]
来源：http://jly.guowangkeji.top

PHP:  strrev($s);
来源：http://pho.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://tuw.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://afc.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jla.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wqv.pycfn.com

Ruby: s.reverse
来源：http://tnp.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qui.fzhhl.top

[E12] 统计某字符出现次数
来源：http://tgc.havefunace.top

Py:   s.count("a")
来源：http://lft.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://syo.yueranfly.top

JS:   s.split("a").length - 1
来源：http://erq.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://kec.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tpo.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://csh.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://uoo.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://jtj.ivvv.top

[E13] 逐字符遍历
来源：http://fjk.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://srw.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hsm.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://dhz.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vbs.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://unk.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gue.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zwp.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://snf.xylfe.cn

[E14] URL 编码与 Base64
来源：http://ovk.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://chv.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yug.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lha.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cak.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://umg.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dcd.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://loi.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dou.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://lcz.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://xlf.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://std.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pvn.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cjd.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjp.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xoh.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://epb.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mth.xinyue.icu

[E16] 数字千分位
来源：http://phj.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://dom.0kj1m.cn

PHP:  number_format(1234567);
来源：http://wbw.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://awh.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lzo.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nfa.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rnk.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wtj.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://dot.316326.xyz

[E17] 首字母大写
来源：http://vko.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rog.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrb.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lpe.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lgi.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kyj.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://smb.yj20258888.top

Ruby: s.capitalize
来源：http://ybm.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://juy.fehbvm.com

[E18] 模板占位符替换
来源：http://trp.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xcp.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vxt.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://hkb.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wfu.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hll.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wva.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vdu.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aws.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://lyd.ppjwa.cn

Py:   s.splitlines()
来源：http://xlm.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pwa.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://mki.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://mtz.haohaochexian.top

Java: s.lines().toList()
来源：http://ihu.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://okm.shanyushiyangtech.top

Ruby: s.lines
来源：http://vjk.0kj1m.cn

C#:   s.Split('\n')
来源：http://hca.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://xul.jqgfzy.top

Py:   if not s:
来源：http://hjr.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://scn.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aez.andypj.xyz

TS:   if (s === "") {}
来源：http://hha.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://dft.ctjpmb.com

Go:   if s == "" {}
来源：http://biw.shzxlz.cn

Ruby: if s.empty?
来源：http://hcs.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zxi.wangdashe.top

[E21] 超长截断加省略号
来源：http://ivq.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kkj.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhb.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nwh.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yth.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://itw.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://ttd.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bnv.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://khi.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://sex.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vtv.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ema.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hju.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyv.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cxj.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhe.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://gdj.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oct.tarul.cn

================================================================================
来源：http://qiu.nanxinkj.top

F. 文件与目录
来源：http://vrg.cdnleiting.top

================================================================================
来源：http://ant.jqgufenzy.top

[F01] 读取整个文件
来源：http://tnh.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zcn.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://cxi.xziqi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://des.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjr.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lcn.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://unk.xziqi.cn

Ruby: File.read("a.txt")
来源：http://puo.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://jqd.ppjwa.cn

[F02] 逐行读取文件
来源：http://sjx.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://obz.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bdu.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wzd.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfu.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mog.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oay.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybx.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fub.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://vpj.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://agm.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://khe.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voi.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnf.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rxl.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kle.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://xrm.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://glc.xziqi.cn

[F04] 追加写入文件
来源：http://vsz.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://koe.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nvm.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igd.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zet.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iro.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uiw.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jqf.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxr.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://eyg.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mvh.birdmap.top

PHP:  file_exists("a.txt");
来源：http://qzo.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://ydu.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://znb.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://joe.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjq.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://woh.yj202588.top

C#:   File.Exists("a.txt")
来源：http://jyt.sxryk.cn

[F06] 删除文件
来源：http://olr.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://nmq.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://lpn.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ouw.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oyp.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yue.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://azp.yj20258.top

Ruby: File.delete("a.txt")
来源：http://zhx.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://pdn.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://mhf.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pyk.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bgc.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzg.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wkl.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qqm.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lag.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yya.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zml.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://pwo.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mkv.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hjz.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://pcn.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://dqp.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://frm.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://utl.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://beu.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://icu.bbcook.cn

[F09] 获取文件大小
来源：http://ctx.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://vxw.ivvv.top

PHP:  filesize("a.txt");
来源：http://erq.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://nem.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://vji.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://vjr.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bov.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://kin.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://crr.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://qem.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ivg.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zxo.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ioq.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://abc.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://shr.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kzc.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xmp.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://frh.tarul.cn

[F11] 复制与移动文件
来源：http://ydo.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pvl.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zou.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iyh.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rpm.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://unb.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pca.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lir.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qnt.zhijiandao.cn

[F12] CSV 读写
来源：http://clv.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmp.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uwv.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wfn.bbcook.cn

TS:   // 同上
来源：http://nqs.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tnp.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bff.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lvu.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://krz.chenlongwang.top

================================================================================
来源：http://bwg.tian-w.cn

G. 面向对象
来源：http://kek.xziqi.cn

================================================================================
来源：http://idi.tarul.cn

[G01] 定义类
来源：http://uyb.zhijiandao.cn

Py:   class User: pass
来源：http://jal.nwbrower.top

PHP:  class User {}
来源：http://hje.gotoacloud.top

JS:   class User {}
来源：http://gyi.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://vld.xylfe.cn

Java: class User {}
来源：http://zdd.zhengqikj.top

Go:   type User struct { Name string }
来源：http://cwo.ybcxt.top

Ruby: class User; end
来源：http://lfm.pycfn.com

C#:   class User {}
来源：http://zbe.zhixingplan.top

[G02] 构造函数
来源：http://dyh.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://qxh.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://gmm.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://rry.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://imx.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://rpw.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://noa.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://kec.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://zsi.bbcook.cn

[G03] 实例属性
来源：http://jxj.uphjek.com

Py:   self.name = "x"
来源：http://kwr.nwbrower.top

PHP:  public string $name = "x";
来源：http://cvd.aizwys.cn

JS:   this.name = "x";
来源：http://nky.havefunace.top

TS:   name: string = "x";
来源：http://szp.sufxvd.cn

Java: private String name;
来源：http://anr.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ybs.316326.xyz

Ruby: @name = "x"
来源：http://sxz.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://azs.hcnkem.com

[G04] 定义方法
来源：http://cld.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://lcg.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kst.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://xno.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://ydn.sjlbkw.cn

Java: String greet() { return name; }
来源：http://ixa.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://art.tianlin.xyz

Ruby: def greet; @name; end
来源：http://hkr.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://ayp.aibaodan.cn

[G05] 继承
来源：http://kce.9152youxi.cn

Py:   class Admin(User): pass
来源：http://jik.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://jgr.shzxlz.cn

JS:   class Admin extends User {}
来源：http://cza.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://bxv.sweek.top

Java: class Admin extends User {}
来源：http://gzu.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rbc.zdqjudy.top

Ruby: class Admin < User; end
来源：http://lgs.quarkkingdee.top

C#:   class Admin : User {}
来源：http://pft.tanke756.top

[G06] 重写方法
来源：http://ddf.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://loh.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://vvz.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://qyy.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://gja.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://hei.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yco.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://jxx.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://whf.ivvv.top

[G07] 调用父类方法
来源：http://gxt.xuetiantiany.cn

Py:   super().greet()
来源：http://akm.quarkkingdee.top

PHP:  parent::greet();
来源：http://sbs.fzhhl.top

JS:   super.greet();
来源：http://whm.svipenyu.cn

TS:   super.greet();
来源：http://sww.ydjk.org.cn

Java: super.greet();
来源：http://duy.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lma.yonumen.top

Ruby: super
来源：http://lnh.mhx1999.top

C#:   base.Greet();
来源：http://lgp.sufxvd.cn

[G08] 静态方法与属性
来源：http://hmc.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rll.tanke756.top

PHP:  public static function f() {}
来源：http://uve.sjlbkw.cn

JS:   static f() {}
来源：http://okk.tanke756.top

TS:   static f(): void {}
来源：http://snd.chenjidiqi.icu

Java: static void f() {}
来源：http://otb.zhijiandao.cn


<!-- 参考信息 -->