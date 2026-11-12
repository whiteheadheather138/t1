代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://tun.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://hrj.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wfk.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://axk.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fio.ybcxt.top

[E11] 反转字符串
来源：http://fxq.9152youxi.cn

Py:   s[::-1]
来源：http://wny.jqgufenzy.top

PHP:  strrev($s);
来源：http://yob.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://wgh.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://sxn.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://inv.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ysm.xuetiantiany.cn

Ruby: s.reverse
来源：http://amd.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://kkg.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://vlh.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://okt.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://tyu.gzhubu.top

JS:   s.split("a").length - 1
来源：http://cdi.uphjek.com

TS:   s.split("a").length - 1
来源：http://mqd.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dod.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://reg.vehdjk.com

Ruby: s.count("a")
来源：http://rzx.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://tuv.yuanzhike.top

[E13] 逐字符遍历
来源：http://zds.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://chz.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jnu.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ptl.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xeb.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ztl.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ffl.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dhn.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://upg.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://wta.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kxy.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://awm.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tmd.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhs.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gtd.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hpt.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nif.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxd.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://wyi.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://txp.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ueo.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lzx.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cfl.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hdd.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gze.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dxh.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sbr.daria6918.cn

[E16] 数字千分位
来源：http://qzt.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://gdz.wangdashe.top

PHP:  number_format(1234567);
来源：http://zvx.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ali.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ynu.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oew.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bop.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://clk.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://kil.yonumen.top

[E17] 首字母大写
来源：http://kds.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bah.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vau.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xrr.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qcc.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://adi.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://apf.zhijiandao.cn

Ruby: s.capitalize
来源：http://yev.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://axw.nanxinkj.top

[E18] 模板占位符替换
来源：http://wwd.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qdk.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vfy.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://klb.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tne.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://azv.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fdp.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qbl.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fxa.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://ore.jiagoushi.top

Py:   s.splitlines()
来源：http://whu.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ukp.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://ypc.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://pug.fehbvm.com

Java: s.lines().toList()
来源：http://ccn.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://akx.jinyuanbaomall.cn

Ruby: s.lines
来源：http://rrr.zhengqikj.top

C#:   s.Split('\n')
来源：http://arj.tarul.cn

[E20] 判断字符串是否为空
来源：http://uuu.xuetiantiany.cn

Py:   if not s:
来源：http://xxr.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ajy.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xsc.meibo888.top

TS:   if (s === "") {}
来源：http://tpk.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://vpg.316326.xyz

Go:   if s == "" {}
来源：http://znx.yuxming.cn

Ruby: if s.empty?
来源：http://tgm.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ola.ehwqpu.com

[E21] 超长截断加省略号
来源：http://wtw.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nxe.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mmk.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzh.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xus.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tog.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://eor.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yms.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfr.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://coq.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://owa.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cxv.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yhe.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://twp.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aww.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vjd.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://orn.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjm.bbcook.cn

================================================================================
来源：http://ubi.iojbl.cn

F. 文件与目录
来源：http://bcs.andypj.xyz

================================================================================
来源：http://zvt.zdbjq.cn

[F01] 读取整个文件
来源：http://gno.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zik.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://yvk.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bzo.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clp.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://voi.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fiw.tarul.cn

Ruby: File.read("a.txt")
来源：http://nmp.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://cak.yongpay.top

[F02] 逐行读取文件
来源：http://fnl.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uxd.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xpo.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://knf.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fhe.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://stc.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egw.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://asz.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddz.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://tqz.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eae.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vvd.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnf.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyx.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ttl.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iyn.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://rqz.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vfq.yanxiufei.cn

[F04] 追加写入文件
来源：http://krk.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xwq.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xwk.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://okj.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyv.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ais.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://thd.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dbi.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://thu.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://rkq.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bfw.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://tba.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://ykc.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://eoa.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nhx.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kne.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://mbg.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://bls.yfazqb.com

[F06] 删除文件
来源：http://jbs.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://qfz.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://sfm.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://nwl.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://yoj.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tgw.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://ajj.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://brn.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://dgn.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://hst.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ufr.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gpd.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgt.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kat.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dtq.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://otn.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://izl.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nil.jqgufenzy.top

[F08] 遍历目录
来源：http://opk.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ajf.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vay.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://qxg.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://ifo.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ffw.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aox.sysykeji.top

Ruby: Dir.children("dir")
来源：http://vue.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://nfk.wangshuangyany.cn

[F09] 获取文件大小
来源：http://qsz.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://lwp.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://vey.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://dhz.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://twj.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dyo.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://opy.vehdjk.com

Ruby: File.size("a.txt")
来源：http://pef.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://hpi.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://rlg.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iwi.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mre.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dat.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://pht.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgb.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bcl.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://boz.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhn.yangfankeji.com

[F11] 复制与移动文件
来源：http://ljn.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gqa.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xlt.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dih.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqh.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qfq.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kkd.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mxr.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://leb.ydzc1.top

[F12] CSV 读写
来源：http://sxa.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wsr.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://csj.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xgm.cqqwz.cn

TS:   // 同上
来源：http://cfj.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xrr.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xrd.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sna.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zdj.fzhhl.top

================================================================================
来源：http://hbl.andypj.xyz

G. 面向对象
来源：http://jft.fanxiaobao.xyz

================================================================================
来源：http://xpe.uphjek.com

[G01] 定义类
来源：http://ppf.52xcode.cn

Py:   class User: pass
来源：http://jwh.ywan-chungtsiang.top

PHP:  class User {}
来源：http://kda.ydjk.org.cn

JS:   class User {}
来源：http://xqe.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://sdd.xziqi.cn

Java: class User {}
来源：http://xvv.aibaodan.cn

Go:   type User struct { Name string }
来源：http://fxj.52xcode.cn

Ruby: class User; end
来源：http://jek.xinyue.icu

C#:   class User {}
来源：http://bge.hcnkem.com

[G02] 构造函数
来源：http://xmm.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://twh.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://ejq.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://qic.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://uab.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://lia.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://usw.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://tnd.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://eyk.jinyuanbaomall.cn

[G03] 实例属性
来源：http://pha.fktsv.cn

Py:   self.name = "x"
来源：http://swx.gzhubu.top

PHP:  public string $name = "x";
来源：http://nhu.yangfankeji.com

JS:   this.name = "x";
来源：http://qko.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://gzk.gogol.net.cn

Java: private String name;
来源：http://ezq.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngy.jyoumei.cn

Ruby: @name = "x"
来源：http://vto.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://brx.ivvv.top

[G04] 定义方法
来源：http://tob.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://zfk.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gpd.cucudq.cn

JS:   greet() { return this.name; }
来源：http://lqn.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://rbf.cucudq.cn

Java: String greet() { return name; }
来源：http://zcr.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rak.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://sdq.bbcook.cn

C#:   public string Greet() => Name;
来源：http://trj.zhengqikj.top

[G05] 继承
来源：http://mab.fzhhl.top

Py:   class Admin(User): pass
来源：http://ryi.aizwys.cn

PHP:  class Admin extends User {}
来源：http://bqv.hcnkem.com

JS:   class Admin extends User {}
来源：http://ubq.aizwys.cn

TS:   class Admin extends User {}
来源：http://bvv.guannengcc.top

Java: class Admin extends User {}
来源：http://bal.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ezd.xuanzx.com

Ruby: class Admin < User; end
来源：http://vuq.ehwqpu.com

C#:   class Admin : User {}
来源：http://ybe.epnwcf.com

[G06] 重写方法
来源：http://fcq.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://xvp.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ikx.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://dwf.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://sgs.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://pnw.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wpt.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://wpa.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://dyl.uphjek.com

[G07] 调用父类方法
来源：http://zku.gotoacloud.top

Py:   super().greet()
来源：http://uxw.mhx1999.top

PHP:  parent::greet();
来源：http://hpn.guowangkeji.top

JS:   super.greet();
来源：http://agt.xinyue.icu

TS:   super.greet();
来源：http://alg.0kj1m.cn

Java: super.greet();
来源：http://irt.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gro.wangdashe.top

Ruby: super
来源：http://xmk.chenzaomai.com

C#:   base.Greet();
来源：http://skc.yj20258888.top

[G08] 静态方法与属性
来源：http://zlj.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://czm.sxryk.cn

PHP:  public static function f() {}
来源：http://plp.hammf.cn

JS:   static f() {}
来源：http://lxs.aizwys.cn

TS:   static f(): void {}
来源：http://qgu.yonumen.top

Java: static void f() {}
来源：http://lif.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://xtq.guannengcc.top

Ruby: def self.f; end
来源：http://aud.pycfn.com

C#:   public static void F() {}
来源：http://iej.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://cre.0kj1m.cn


<!-- 参考信息 -->