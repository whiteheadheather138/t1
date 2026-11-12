代发 wailian999

JS:   [...s].reverse().join("")
来源：http://ede.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://tgf.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dve.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zik.yangfankeji.com

Ruby: s.reverse
来源：http://akj.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://kbp.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://mco.hnqzz.top

Py:   s.count("a")
来源：http://kid.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://sgu.cucudq.cn

JS:   s.split("a").length - 1
来源：http://hhm.ydzc1.top

TS:   s.split("a").length - 1
来源：http://qwg.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fjm.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://qgt.jqgfzy.top

Ruby: s.count("a")
来源：http://syh.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://umh.jyoumei.cn

[E13] 逐字符遍历
来源：http://chh.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://tag.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sgt.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://edo.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bgb.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://plv.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zve.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://vim.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zwh.tanke756.top

[E14] URL 编码与 Base64
来源：http://mss.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdf.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cdx.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://okn.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zqt.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ryy.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://izm.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kkh.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hpz.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://pcx.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://elm.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dxf.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tww.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nky.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cpg.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rvq.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pqu.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://adt.jianghu66.top

[E16] 数字千分位
来源：http://coa.cheryme.top

Py:   f"{1234567:,}"
来源：http://jsr.fktsv.cn

PHP:  number_format(1234567);
来源：http://jda.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pps.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bqj.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nda.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pbv.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ffd.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://jyi.hywenlv.cn

[E17] 首字母大写
来源：http://xkp.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kri.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qbs.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cck.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ysp.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kyn.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mbx.hysaishi.cn

Ruby: s.capitalize
来源：http://dqh.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ibc.aibaodan.cn

[E18] 模板占位符替换
来源：http://bqx.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xcb.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jev.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uda.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bxu.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ojz.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ann.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://koc.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://asc.aizwys.cn

[E19] 多行文本按行拆分
来源：http://sah.zycfv.cn

Py:   s.splitlines()
来源：http://fdu.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lvq.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://zcy.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://hou.ybcxt.top

Java: s.lines().toList()
来源：http://ang.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://olk.tanke756.top

Ruby: s.lines
来源：http://tsi.andypj.xyz

C#:   s.Split('\n')
来源：http://rps.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://yyx.hesvh.cn

Py:   if not s:
来源：http://tgs.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gel.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qgt.hnxiangtu.top

TS:   if (s === "") {}
来源：http://cnm.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://rvh.cqqwz.cn

Go:   if s == "" {}
来源：http://lwf.nwbrower.top

Ruby: if s.empty?
来源：http://oac.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jju.epnwcf.com

[E21] 超长截断加省略号
来源：http://jrw.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lhm.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jmh.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qgf.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rux.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ogb.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://vhy.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mqc.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://byn.tanke756.top

[E22] 字节长度与字符长度
来源：http://mdy.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzs.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwq.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://idv.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oen.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uqj.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fio.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://tha.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lrj.vqdsnc.cn

================================================================================
来源：http://omr.316326.xyz

F. 文件与目录
来源：http://bsm.hysaishi.cn

================================================================================
来源：http://qln.kuanghao11.cn

[F01] 读取整个文件
来源：http://hvw.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://olx.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://puy.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kym.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vcl.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://gvy.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ysd.sxryk.cn

Ruby: File.read("a.txt")
来源：http://eet.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://cqd.hcnkem.com

[F02] 逐行读取文件
来源：http://cta.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vpr.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://srl.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://guz.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://noe.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rjd.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://udh.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://stf.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sof.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://jmx.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bqp.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rtv.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ptb.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://acz.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vzq.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tyw.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://arq.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cdl.chenjidiqi.icu

[F04] 追加写入文件
来源：http://kgc.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qbv.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ylu.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwu.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehs.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hft.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nyd.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oba.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gyz.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://bvl.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mov.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://cmh.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://vjz.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://rte.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fad.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fvk.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://tfm.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://bbl.hfpthk.cn

[F06] 删除文件
来源：http://vxf.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://cdx.yj202588.top

PHP:  unlink("a.txt");
来源：http://acf.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://zsy.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tti.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hdt.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://kia.316326.xyz

Ruby: File.delete("a.txt")
来源：http://vmu.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://wae.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://yms.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oaq.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nid.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whq.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://red.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xai.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://inz.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zwa.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://raa.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://klg.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://uhy.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wxo.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://kld.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://xic.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xgq.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://npq.redwolf501.top

Ruby: Dir.children("dir")
来源：http://qjw.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://cli.guannengcc.top

[F09] 获取文件大小
来源：http://nfd.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://uin.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://mal.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://ngq.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://bul.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://jet.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qyi.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://afx.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ltd.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://pgb.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xqg.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hev.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pja.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://jeq.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bau.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://meq.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cjk.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tad.sufxvd.cn

[F11] 复制与移动文件
来源：http://bde.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ddf.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://flu.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqi.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nly.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qho.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nfr.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xtx.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nog.wangdashe.top

[F12] CSV 读写
来源：http://gvw.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jtj.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aol.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fiz.tian-w.cn

TS:   // 同上
来源：http://vzi.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rjy.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xig.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://izi.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://xqv.cdnleiting.top

================================================================================
来源：http://rvb.zdqjudy.top

G. 面向对象
来源：http://ysj.quarkkingdee.top

================================================================================
来源：http://ahd.vqdsnc.cn

[G01] 定义类
来源：http://jco.yuxming.cn

Py:   class User: pass
来源：http://uep.svipenyu.cn

PHP:  class User {}
来源：http://tts.aizwys.cn

JS:   class User {}
来源：http://gks.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://nst.hnxiangtu.top

Java: class User {}
来源：http://wbq.yuanzhike.top

Go:   type User struct { Name string }
来源：http://wft.jinqigufen.top

Ruby: class User; end
来源：http://zdh.hcnkem.com

C#:   class User {}
来源：http://uni.xuanzx.com

[G02] 构造函数
来源：http://gng.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://izx.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://akr.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://jph.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://xpo.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://qwr.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hmt.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://ijf.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://zgo.gotoacloud.top

[G03] 实例属性
来源：http://eov.cqqwz.cn

Py:   self.name = "x"
来源：http://zit.yvedp.cn

PHP:  public string $name = "x";
来源：http://nrs.kuanghao11.cn

JS:   this.name = "x";
来源：http://nfw.yj20258888.top

TS:   name: string = "x";
来源：http://opd.birdmap.top

Java: private String name;
来源：http://ggq.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsk.daxiang520.top

Ruby: @name = "x"
来源：http://mru.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://vcu.guowangkeji.top

[G04] 定义方法
来源：http://mrd.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://zms.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://yns.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://kpu.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://nbr.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://ayg.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tat.0kj1m.cn

Ruby: def greet; @name; end
来源：http://epa.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://mka.shzxlz.cn

[G05] 继承
来源：http://syj.nwbrower.top

Py:   class Admin(User): pass
来源：http://jmv.bjfxy.top

PHP:  class Admin extends User {}
来源：http://ztf.fktsv.cn

JS:   class Admin extends User {}
来源：http://qfc.ydzc1.top

TS:   class Admin extends User {}
来源：http://xvv.yonumen.top

Java: class Admin extends User {}
来源：http://vhp.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rhk.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://sov.vqdsnc.cn

C#:   class Admin : User {}
来源：http://yja.fktsv.cn

[G06] 重写方法
来源：http://ymz.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://wbz.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jxo.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://eqp.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://qoo.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://bpz.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uys.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://wdx.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://vxp.shzxlz.cn

[G07] 调用父类方法
来源：http://bfx.wangshuangyany.cn

Py:   super().greet()
来源：http://sud.ydzc1.top

PHP:  parent::greet();
来源：http://mjk.cheryme.top

JS:   super.greet();
来源：http://zcq.hfpthk.cn

TS:   super.greet();
来源：http://uji.birdmap.top

Java: super.greet();
来源：http://kda.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qyq.aibaodan.cn

Ruby: super
来源：http://dcc.sweek.top

C#:   base.Greet();
来源：http://wig.yonumen.top

[G08] 静态方法与属性
来源：http://sig.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qvj.mhx1999.top

PHP:  public static function f() {}
来源：http://bwz.feifeiyinyue.top

JS:   static f() {}
来源：http://dle.zhengqikj.top

TS:   static f(): void {}
来源：http://dkh.yongpay.top

Java: static void f() {}
来源：http://aue.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ocm.tian-w.cn

Ruby: def self.f; end
来源：http://hyb.uphjek.com

C#:   public static void F() {}
来源：http://dra.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://bls.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://ivf.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://ajx.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://biy.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://phy.shuidangran.top

Java: interface Shape { double area(); }
来源：http://cfa.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://dub.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://roe.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://sny.xinyue.icu


<!-- 参考信息 -->