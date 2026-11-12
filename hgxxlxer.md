代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghq.xuanzx.com

[E11] 反转字符串
来源：http://mbg.jinqigfzy.top

Py:   s[::-1]
来源：http://gld.gzhubu.top

PHP:  strrev($s);
来源：http://lop.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://xha.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://rrc.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vcw.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ycp.andypj.xyz

Ruby: s.reverse
来源：http://ssm.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://mjl.tian-w.cn

[E12] 统计某字符出现次数
来源：http://rte.andypj.xyz

Py:   s.count("a")
来源：http://brr.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://mbg.sysykeji.top

JS:   s.split("a").length - 1
来源：http://ibs.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://mow.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zky.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://vjn.gotoacloud.top

Ruby: s.count("a")
来源：http://ssd.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://ddp.havefunace.top

[E13] 逐字符遍历
来源：http://zts.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://gba.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mdh.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kjj.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wzn.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxw.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://orm.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://scd.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xqv.ivvv.top

[E14] URL 编码与 Base64
来源：http://vdi.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fna.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://uqh.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ocn.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dek.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wxw.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://amq.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://csc.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ytz.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://zuw.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://meh.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jlt.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://knv.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lnv.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vnf.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dbg.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ywj.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uiv.hesvh.cn

[E16] 数字千分位
来源：http://tnm.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://yiq.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://pcw.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ygr.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vqq.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rwt.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iov.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uoc.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://tcd.sjlbkw.cn

[E17] 首字母大写
来源：http://lhk.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nmz.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xfz.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lgn.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fav.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bek.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nrb.daria6918.cn

Ruby: s.capitalize
来源：http://wfu.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrt.birdmap.top

[E18] 模板占位符替换
来源：http://duw.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://stk.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uqw.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ece.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://avd.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mkd.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jva.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xdr.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ktp.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://gwm.tian-w.cn

Py:   s.splitlines()
来源：http://vuc.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zde.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://jqq.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://git.gotoacloud.top

Java: s.lines().toList()
来源：http://lyn.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://vse.aizwys.cn

Ruby: s.lines
来源：http://dur.shzxlz.cn

C#:   s.Split('\n')
来源：http://dwu.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://hjb.yj202588.top

Py:   if not s:
来源：http://zkv.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yyk.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cty.guowangkeji.top

TS:   if (s === "") {}
来源：http://juv.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://slz.zhixingplan.top

Go:   if s == "" {}
来源：http://xmq.hnxiangtu.top

Ruby: if s.empty?
来源：http://vvl.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ndd.sysykeji.top

[E21] 超长截断加省略号
来源：http://crk.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://anw.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://phx.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://shv.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ifb.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dii.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://ngk.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uww.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://frm.daxiang520.top

[E22] 字节长度与字符长度
来源：http://jna.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rtj.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrl.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsb.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rre.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hlb.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hgc.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://ohr.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dnq.vehdjk.com

================================================================================
来源：http://onh.xuanzx.com

F. 文件与目录
来源：http://iia.xinyue.icu

================================================================================
来源：http://zse.gaohongyu789.top

[F01] 读取整个文件
来源：http://gba.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vfz.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://mfx.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://txn.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wcw.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zre.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xch.c1oappe.top

Ruby: File.read("a.txt")
来源：http://pnl.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://gom.guannengcc.top

[F02] 逐行读取文件
来源：http://bqa.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mcc.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bjq.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bzg.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://inj.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbd.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yra.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gtu.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lbw.hammf.cn

[F03] 写入文件（覆盖）
来源：http://jup.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lxg.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dke.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nsb.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abl.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kpc.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lnx.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://pga.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pys.wangdashe.top

[F04] 追加写入文件
来源：http://cja.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kme.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fus.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zis.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zlk.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gpv.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hyh.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lyr.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://axu.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://yfj.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://etu.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://tvi.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://rlt.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://bas.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fon.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vil.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://tpk.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://xcb.nwbrower.top

[F06] 删除文件
来源：http://hhl.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://yoh.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://vgf.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://wgt.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://hls.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kqc.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://pdy.ivvv.top

Ruby: File.delete("a.txt")
来源：http://czh.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://lxp.zycfv.cn

[F07] 创建目录（含多级）
来源：http://snv.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hmh.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jdl.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxz.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itf.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iex.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tyq.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://owq.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlr.dianchejie.cn

[F08] 遍历目录
来源：http://uhy.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fgj.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://juc.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://rci.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://kmv.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://azp.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://dqo.smart0.xyz

Ruby: Dir.children("dir")
来源：http://rua.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://kpp.zhijiandao.cn

[F09] 获取文件大小
来源：http://zqh.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://tmu.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://qop.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://qbi.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://utq.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kzc.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://exc.316326.xyz

Ruby: File.size("a.txt")
来源：http://unh.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://jws.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://ylr.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zah.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wfv.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://urw.ivvv.top

TS:   path.extname("a.txt")
来源：http://hff.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tsz.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sei.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://umk.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eli.nanxuanxn.top

[F11] 复制与移动文件
来源：http://hvu.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://isw.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ifk.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdz.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbx.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://swy.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tiu.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qke.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://njt.ppjwa.cn

[F12] CSV 读写
来源：http://hry.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://viu.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kcv.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zvm.feifeiyinyue.top

TS:   // 同上
来源：http://rjj.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ona.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mzx.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jon.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://csz.guowangkeji.top

================================================================================
来源：http://rts.shanyushiyangkeji.top

G. 面向对象
来源：http://lqf.haohaochexian.top

================================================================================
来源：http://pjs.hesvh.cn

[G01] 定义类
来源：http://yxc.tarul.cn

Py:   class User: pass
来源：http://dwk.fengsongda.top

PHP:  class User {}
来源：http://psn.gaohongyu789.top

JS:   class User {}
来源：http://ldr.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://fsn.bbcook.cn

Java: class User {}
来源：http://tqt.meibo888.top

Go:   type User struct { Name string }
来源：http://giz.xinyue.icu

Ruby: class User; end
来源：http://uxd.zdqjudy.top

C#:   class User {}
来源：http://cwt.tanke756.top

[G02] 构造函数
来源：http://gkx.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://fvd.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://shu.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://tab.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://fsi.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://svb.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://apb.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://ymu.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://foz.dashuyun.cn

[G03] 实例属性
来源：http://yvj.jiagoushi.top

Py:   self.name = "x"
来源：http://mdo.ppjwa.cn

PHP:  public string $name = "x";
来源：http://wis.snrcjt.cn

JS:   this.name = "x";
来源：http://lgh.snrcjt.cn

TS:   name: string = "x";
来源：http://nzp.jianghu66.top

Java: private String name;
来源：http://qgu.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://unl.jqgfzy.top

Ruby: @name = "x"
来源：http://wnd.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://pya.zdbjq.cn

[G04] 定义方法
来源：http://pmy.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://aqy.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wok.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://odz.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://vfm.daxiang520.top

Java: String greet() { return name; }
来源：http://zhp.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qdg.bbcook.cn

Ruby: def greet; @name; end
来源：http://ffs.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://swe.iojbl.cn

[G05] 继承
来源：http://vvy.tarul.cn

Py:   class Admin(User): pass
来源：http://mxd.wangdashe.top

PHP:  class Admin extends User {}
来源：http://zjn.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://dsk.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://nht.chenzaomai.com

Java: class Admin extends User {}
来源：http://and.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yui.wangdashe.top

Ruby: class Admin < User; end
来源：http://pqk.jqgufenzy.top

C#:   class Admin : User {}
来源：http://sme.vqdsnc.cn

[G06] 重写方法
来源：http://tfa.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://pts.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jly.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://zal.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://jao.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://gee.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lau.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://exe.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://xke.cheryme.top

[G07] 调用父类方法
来源：http://zqd.jinghuilouyu.cn

Py:   super().greet()
来源：http://bqa.yj20258888.top

PHP:  parent::greet();
来源：http://lxi.svipenyu.cn

JS:   super.greet();
来源：http://cgs.zhaomingkeji.xyz

TS:   super.greet();
来源：http://qsx.smart0.xyz

Java: super.greet();
来源：http://hei.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ovx.yongpay.top

Ruby: super
来源：http://kbm.52xcode.cn

C#:   base.Greet();
来源：http://atl.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://ihu.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://agu.yuanzhike.top

PHP:  public static function f() {}
来源：http://xzi.iojbl.cn

JS:   static f() {}
来源：http://dxm.hcnkem.com

TS:   static f(): void {}
来源：http://jfx.aibaodan.cn

Java: static void f() {}
来源：http://ltz.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dlu.bbcook.cn

Ruby: def self.f; end
来源：http://qxb.zycfv.cn

C#:   public static void F() {}
来源：http://zvj.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://daw.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://vrj.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://vjz.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ybm.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://tda.zhongyouzk.top


<!-- 参考信息 -->