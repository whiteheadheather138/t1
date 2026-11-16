代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wlb.quarkkingdee.top

[E11] 反转字符串
来源：http://exb.quarkkingdee.top

Py:   s[::-1]
来源：http://lqk.jinqigufen.top

PHP:  strrev($s);
来源：http://ahc.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://xbf.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://yaa.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wpy.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xov.shangyingyoupin.top

Ruby: s.reverse
来源：http://eoe.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://wbi.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://pmc.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://tek.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://jss.fehbvm.com

JS:   s.split("a").length - 1
来源：http://svx.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://qev.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vle.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://iap.hnxiangtu.top

Ruby: s.count("a")
来源：http://bfk.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://lqo.jyoumei.cn

[E13] 逐字符遍历
来源：http://yir.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://pbk.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://agx.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xpn.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://rlj.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://snb.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ugw.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gkh.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mrs.havefunace.top

[E14] URL 编码与 Base64
来源：http://vhz.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sbe.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ovu.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qrh.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gin.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rrn.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fvu.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mze.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tsk.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://cnw.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bft.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sdu.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://joa.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ewo.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zar.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ulq.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dij.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://omm.yvedp.cn

[E16] 数字千分位
来源：http://lji.vehdjk.com

Py:   f"{1234567:,}"
来源：http://qou.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://cjb.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oaj.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wbe.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bal.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xwn.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fnu.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://rzh.hywenlv.cn

[E17] 首字母大写
来源：http://kdw.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ehf.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nkd.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://txj.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://krs.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yeb.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fsd.0kj1m.cn

Ruby: s.capitalize
来源：http://kge.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ibw.yuxming.cn

[E18] 模板占位符替换
来源：http://pez.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vwc.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jku.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ttr.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://peb.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wco.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bsa.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zhk.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qhl.cheryme.top

[E19] 多行文本按行拆分
来源：http://xeu.feifeiyinyue.top

Py:   s.splitlines()
来源：http://kgt.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qvk.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://xnq.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://zwc.xziqi.cn

Java: s.lines().toList()
来源：http://pnc.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://dex.meibo888.top

Ruby: s.lines
来源：http://imo.aibaodan.cn

C#:   s.Split('\n')
来源：http://ybc.hnqzz.top

[E20] 判断字符串是否为空
来源：http://fko.gzhubu.top

Py:   if not s:
来源：http://ega.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rrg.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gta.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://meb.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://lqv.kuanghao11.cn

Go:   if s == "" {}
来源：http://tcu.52xcode.cn

Ruby: if s.empty?
来源：http://hnn.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nej.hywenlv.cn

[E21] 超长截断加省略号
来源：http://pfm.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hnh.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vqh.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjc.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmd.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qvw.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://wqo.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vws.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://seh.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://eji.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xdy.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wpm.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ifk.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pte.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mzd.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ddj.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://tom.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yjz.zycfv.cn

================================================================================
来源：http://yyu.hfpthk.cn

F. 文件与目录
来源：http://tin.vehdjk.com

================================================================================
来源：http://nil.ydjk.org.cn

[F01] 读取整个文件
来源：http://wwv.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tzn.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://mod.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zth.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pxj.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lek.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndl.xuanzx.com

Ruby: File.read("a.txt")
来源：http://swk.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://pbz.yj202588.top

[F02] 逐行读取文件
来源：http://yzw.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nfq.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xnf.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uah.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://haw.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cui.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mcq.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zeg.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nuh.meibo888.top

[F03] 写入文件（覆盖）
来源：http://dxi.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cng.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qzl.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://slb.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zmo.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ene.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baj.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://hro.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ivy.tian-w.cn

[F04] 追加写入文件
来源：http://dik.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sdg.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uif.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pna.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayc.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yru.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sqd.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcp.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qap.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://hpl.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ihx.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://dii.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://bib.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://wwt.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ysw.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nle.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://sif.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://prg.ywan-chungtsiang.top

[F06] 删除文件
来源：http://fxs.c1oappe.top

Py:   os.remove("a.txt")
来源：http://mqg.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://rdr.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://lhc.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mzj.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cko.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://bbs.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://aek.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://egy.sweek.top

[F07] 创建目录（含多级）
来源：http://btk.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yyq.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://que.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pul.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztf.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lbr.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://opd.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocw.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xjh.zhongyouzk.top

[F08] 遍历目录
来源：http://ibd.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yok.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qkp.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://yrv.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://zkt.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ycg.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xyd.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://rqi.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://ckm.iojbl.cn

[F09] 获取文件大小
来源：http://kjc.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ghr.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://ckh.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://lkw.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://xcj.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://dfp.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wtj.c1oappe.top

Ruby: File.size("a.txt")
来源：http://sra.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://use.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://jpv.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wjg.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ixh.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://djj.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://nmw.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sxg.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zhv.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://itw.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://roe.hfpthk.cn

[F11] 复制与移动文件
来源：http://blp.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dlq.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://clg.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwa.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uxj.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://udv.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ofj.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://umw.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xue.52xcode.cn

[F12] CSV 读写
来源：http://lzx.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bpq.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://phl.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fnp.xylfe.cn

TS:   // 同上
来源：http://hlg.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nta.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fyn.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uvw.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rdc.yj20258.top

================================================================================
来源：http://pnc.cdnleiting.top

G. 面向对象
来源：http://hze.sjlbkw.cn

================================================================================
来源：http://dra.yueranfly.top

[G01] 定义类
来源：http://erc.jinqigfzy.top

Py:   class User: pass
来源：http://rqt.sjlbkw.cn

PHP:  class User {}
来源：http://fei.pycfn.com

JS:   class User {}
来源：http://mit.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://mfa.jyoumei.cn

Java: class User {}
来源：http://msb.guannengcc.top

Go:   type User struct { Name string }
来源：http://oij.ivvv.top

Ruby: class User; end
来源：http://vop.hcnkem.com

C#:   class User {}
来源：http://mbw.tarul.cn

[G02] 构造函数
来源：http://ltm.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://yxo.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://cim.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://vno.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://ysy.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://ehn.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dtk.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://bpx.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://qew.aibaodan.cn

[G03] 实例属性
来源：http://fro.daxiang520.top

Py:   self.name = "x"
来源：http://laq.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://rdl.zhijiandao.cn

JS:   this.name = "x";
来源：http://qoo.wangdashe.top

TS:   name: string = "x";
来源：http://poe.fengsongda.top

Java: private String name;
来源：http://qip.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lmr.hnxiangtu.top

Ruby: @name = "x"
来源：http://yol.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://bot.fengsongda.top

[G04] 定义方法
来源：http://hrg.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://stc.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rsn.shuidangran.top

JS:   greet() { return this.name; }
来源：http://ndh.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://pap.ydzc1.top

Java: String greet() { return name; }
来源：http://gub.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jxw.ivvv.top

Ruby: def greet; @name; end
来源：http://tph.fktsv.cn

C#:   public string Greet() => Name;
来源：http://prr.redwolf501.top

[G05] 继承
来源：http://wyq.iojbl.cn

Py:   class Admin(User): pass
来源：http://zau.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://lsu.hywenlv.cn

JS:   class Admin extends User {}
来源：http://yhl.uphjek.com

TS:   class Admin extends User {}
来源：http://vbl.daxiang520.top

Java: class Admin extends User {}
来源：http://pau.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lun.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://kzr.iojbl.cn

C#:   class Admin : User {}
来源：http://arb.guowangkeji.top

[G06] 重写方法
来源：http://zfj.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://wga.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://inu.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://rtq.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://tja.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jpz.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uil.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://aph.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://njc.hnqzz.top

[G07] 调用父类方法
来源：http://udg.dianchejie.cn

Py:   super().greet()
来源：http://zez.fzhhl.top

PHP:  parent::greet();
来源：http://bhi.yonumen.top

JS:   super.greet();
来源：http://yju.birdmap.top

TS:   super.greet();
来源：http://lka.fengsongda.top

Java: super.greet();
来源：http://zey.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uac.cqqwz.cn

Ruby: super
来源：http://fxj.zhiwuduotai.top

C#:   base.Greet();
来源：http://npx.shzxlz.cn

[G08] 静态方法与属性
来源：http://pjf.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vlz.jianghu66.top

PHP:  public static function f() {}
来源：http://mhc.jinqigfzy.top

JS:   static f() {}
来源：http://hpn.shangyingyoupin.top

TS:   static f(): void {}
来源：http://fsc.xuetiantiany.cn

Java: static void f() {}
来源：http://wmj.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zng.yanxiufei.cn

Ruby: def self.f; end
来源：http://bwc.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://gek.hammf.cn

[G09] 接口 / 抽象类
来源：http://qic.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://fwo.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vys.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fji.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://jqq.vqdsnc.cn


<!-- 参考信息 -->