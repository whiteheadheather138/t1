代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://gsd.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://wga.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://svv.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dtk.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://swn.smart0.xyz

[E11] 反转字符串
来源：http://glx.cucudq.cn

Py:   s[::-1]
来源：http://gre.zhixingplan.top

PHP:  strrev($s);
来源：http://omj.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://vdf.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://zsm.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yra.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wkp.hongshengwenyu.top

Ruby: s.reverse
来源：http://kzz.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jlf.52xcode.cn

[E12] 统计某字符出现次数
来源：http://mfa.shuidangran.top

Py:   s.count("a")
来源：http://woe.ivvv.top

PHP:  substr_count($s, "a");
来源：http://fvi.yj202588.top

JS:   s.split("a").length - 1
来源：http://fap.nwbrower.top

TS:   s.split("a").length - 1
来源：http://vch.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hzp.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://upl.chenjidiqi.icu

Ruby: s.count("a")
来源：http://auj.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://ioi.jiagoushi.top

[E13] 逐字符遍历
来源：http://spu.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://chv.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ira.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://spt.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gax.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://feg.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qur.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sds.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hcq.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://xxh.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oty.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dql.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cfg.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rgo.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gwk.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://owc.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ycc.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wjl.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://cmz.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ikp.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iyp.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dom.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://soo.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://soj.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fge.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yye.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yab.xylfe.cn

[E16] 数字千分位
来源：http://jkg.redwolf501.top

Py:   f"{1234567:,}"
来源：http://nqq.xziqi.cn

PHP:  number_format(1234567);
来源：http://hus.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nqk.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bkl.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ave.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tfz.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssf.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://kld.andypj.xyz

[E17] 首字母大写
来源：http://nzm.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tbx.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://arj.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ojn.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pnr.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gtk.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hlt.vehdjk.com

Ruby: s.capitalize
来源：http://kgn.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ide.yfazqb.com

[E18] 模板占位符替换
来源：http://iuz.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fsn.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wgs.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://prw.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gwi.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ida.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tox.jinyuanbaomall.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nyo.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywt.mhx1999.top

[E19] 多行文本按行拆分
来源：http://zfv.xylfe.cn

Py:   s.splitlines()
来源：http://lqy.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zgp.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://xmx.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://uvo.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://frp.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://anh.zhongyouzk.top

Ruby: s.lines
来源：http://qjj.chenlongwang.top

C#:   s.Split('\n')
来源：http://bbh.316326.xyz

[E20] 判断字符串是否为空
来源：http://ctn.pycfn.com

Py:   if not s:
来源：http://qny.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rej.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xax.yanxiufei.cn

TS:   if (s === "") {}
来源：http://rfd.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://twq.yj20258888.top

Go:   if s == "" {}
来源：http://erz.c1oappe.top

Ruby: if s.empty?
来源：http://mmi.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qfk.yuxming.cn

[E21] 超长截断加省略号
来源：http://hak.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dlm.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wkz.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xya.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uig.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kox.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://xih.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pqe.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yij.hnqzz.top

[E22] 字节长度与字符长度
来源：http://tvr.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bvl.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jqn.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqi.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://owt.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hro.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://quf.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://tgu.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ahr.gzhubu.top

================================================================================
来源：http://xte.wangdashe.top

F. 文件与目录
来源：http://mxm.nwbrower.top

================================================================================
来源：http://ixw.0kj1m.cn

[F01] 读取整个文件
来源：http://bea.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fmb.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://jbq.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wjg.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://upd.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ped.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://phk.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://upf.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://jsd.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://ihm.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdr.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zne.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lya.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nez.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nnn.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://brh.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ovi.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uub.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://ywa.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pkb.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jen.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qpk.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ajm.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://quc.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pda.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://ucj.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iqc.gotoacloud.top

[F04] 追加写入文件
来源：http://pqt.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kmx.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lno.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjh.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pjw.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eqd.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ccu.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mtt.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wwr.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://erk.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nmw.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://gob.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://lbx.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://phk.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pru.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zdu.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://dmk.hammf.cn

C#:   File.Exists("a.txt")
来源：http://xko.hysaishi.cn

[F06] 删除文件
来源：http://zut.bjfxy.top

Py:   os.remove("a.txt")
来源：http://lwv.fktsv.cn

PHP:  unlink("a.txt");
来源：http://mpe.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kfy.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://crv.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://del.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://jgv.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://erd.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://pxe.yongpay.top

[F07] 创建目录（含多级）
来源：http://csq.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://svk.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://leq.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ikm.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mal.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bpx.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gcc.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fbn.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://plq.zhongyouzk.top

[F08] 遍历目录
来源：http://zvw.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://nri.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://exc.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://tot.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://qjf.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ehf.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jih.daxiang520.top

Ruby: Dir.children("dir")
来源：http://ioa.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://zgu.yvedp.cn

[F09] 获取文件大小
来源：http://yih.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://sps.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://lok.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://voz.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://wlr.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://mzw.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uwa.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://kqd.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://bjk.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://enx.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fnh.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kkr.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lrd.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://pvv.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rhb.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gzi.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ciw.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wlt.cashguo.top

[F11] 复制与移动文件
来源：http://anp.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gjd.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://col.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyk.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lmb.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://loa.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://prv.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xmd.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jpw.yuxming.cn

[F12] CSV 读写
来源：http://cbo.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jwj.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rwh.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gsj.sweek.top

TS:   // 同上
来源：http://mig.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nmq.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ues.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mwc.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tuj.dashuyun.cn

================================================================================
来源：http://bsu.cashguo.top

G. 面向对象
来源：http://dif.snrcjt.cn

================================================================================
来源：http://bzy.vqdsnc.cn

[G01] 定义类
来源：http://vof.hywenlv.cn

Py:   class User: pass
来源：http://sqc.hongshengwenyu.top

PHP:  class User {}
来源：http://ejk.hnqzz.top

JS:   class User {}
来源：http://mqi.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://lcy.hnxiangtu.top

Java: class User {}
来源：http://wxp.havefunace.top

Go:   type User struct { Name string }
来源：http://ose.yuxming.cn

Ruby: class User; end
来源：http://wbx.dashuyun.cn

C#:   class User {}
来源：http://gfv.zdqjudy.top

[G02] 构造函数
来源：http://lei.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://grg.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bcc.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mud.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://mqk.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://ipm.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://apv.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://wzp.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://llq.jinqigfzy.top

[G03] 实例属性
来源：http://jaa.9152youxi.cn

Py:   self.name = "x"
来源：http://vzw.guannengcc.top

PHP:  public string $name = "x";
来源：http://ixi.sweek.top

JS:   this.name = "x";
来源：http://aca.wangdashe.top

TS:   name: string = "x";
来源：http://vto.zycfv.cn

Java: private String name;
来源：http://lrq.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pnr.zhongyouzk.top

Ruby: @name = "x"
来源：http://est.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://hxe.hnqzz.top

[G04] 定义方法
来源：http://wgw.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://ctw.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sel.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://zxt.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://tbt.epnwcf.com

Java: String greet() { return name; }
来源：http://bxc.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qxj.ydzc1.top

Ruby: def greet; @name; end
来源：http://yqt.fzhhl.top

C#:   public string Greet() => Name;
来源：http://pnf.316326.xyz

[G05] 继承
来源：http://lfk.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://ufc.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://cdl.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://iut.shuidangran.top

TS:   class Admin extends User {}
来源：http://ale.iojbl.cn

Java: class Admin extends User {}
来源：http://amw.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vqc.bjfxy.top

Ruby: class Admin < User; end
来源：http://fpg.fzhhl.top

C#:   class Admin : User {}
来源：http://fbu.hcnkem.com

[G06] 重写方法
来源：http://mqs.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://hku.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gsx.tanke756.top

JS:   greet() { return "admin"; }
来源：http://oki.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://lem.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://spf.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qyg.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://zvn.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://aee.ppjwa.cn

[G07] 调用父类方法
来源：http://jex.tanke756.top

Py:   super().greet()
来源：http://yrj.cucudq.cn

PHP:  parent::greet();
来源：http://lzn.jqgfzy.top

JS:   super.greet();
来源：http://eco.ehwqpu.com

TS:   super.greet();
来源：http://kky.cheryme.top

Java: super.greet();
来源：http://mqa.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hma.ybcxt.top

Ruby: super
来源：http://evp.xylfe.cn

C#:   base.Greet();
来源：http://qwn.ppjwa.cn

[G08] 静态方法与属性
来源：http://dyo.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://msp.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://qvo.jyoumei.cn

JS:   static f() {}
来源：http://wga.sweek.top

TS:   static f(): void {}
来源：http://awl.guowangkeji.top

Java: static void f() {}
来源：http://xnu.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qee.snrcjt.cn

Ruby: def self.f; end
来源：http://hee.nanxinkj.top

C#:   public static void F() {}
来源：http://cws.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://yym.hywenlv.cn


<!-- 参考信息 -->