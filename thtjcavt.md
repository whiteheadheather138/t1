代发 wailian999

JS:   [...s].reverse().join("")
来源：http://owb.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://beq.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://rau.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qll.pengpengdd.cyou

Ruby: s.reverse
来源：http://zyr.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://eip.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://jmd.epnwcf.com

Py:   s.count("a")
来源：http://irq.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://cxk.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://fju.guannengcc.top

TS:   s.split("a").length - 1
来源：http://fre.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eal.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://hzr.sweek.top

Ruby: s.count("a")
来源：http://pjd.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://ebe.pycfn.com

[E13] 逐字符遍历
来源：http://jie.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://ywp.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iqz.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mro.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gre.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fmg.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ejc.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cjg.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tlz.bjfxy.top

[E14] URL 编码与 Base64
来源：http://smb.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zgl.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sby.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ejf.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mly.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://urf.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://omm.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fez.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wwp.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://tmn.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ktz.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ruz.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dcp.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rjx.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://axp.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uce.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://leg.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hnh.gaohongyu789.top

[E16] 数字千分位
来源：http://nya.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://vgk.yj202588.top

PHP:  number_format(1234567);
来源：http://nob.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mqi.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bij.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dpi.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gzi.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qsb.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://irm.chenjidiqi.icu

[E17] 首字母大写
来源：http://urb.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cuu.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mde.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xrn.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyj.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iae.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xwq.guannengcc.top

Ruby: s.capitalize
来源：http://lbe.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyd.cqqwz.cn

[E18] 模板占位符替换
来源：http://smy.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xis.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://swo.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sml.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jws.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cus.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxd.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mnt.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyg.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://xmz.yuxming.cn

Py:   s.splitlines()
来源：http://lzj.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://crs.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://kbo.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://zvb.xuetiantiany.cn

Java: s.lines().toList()
来源：http://uez.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://amj.ywan-chungtsiang.top

Ruby: s.lines
来源：http://ryu.zycfv.cn

C#:   s.Split('\n')
来源：http://lgx.fengsongda.top

[E20] 判断字符串是否为空
来源：http://qfu.shanyushiyangtech.top

Py:   if not s:
来源：http://tqb.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xlk.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qce.ivvv.top

TS:   if (s === "") {}
来源：http://kfw.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://vkv.snrcjt.cn

Go:   if s == "" {}
来源：http://bov.hcnkem.com

Ruby: if s.empty?
来源：http://ztj.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sji.xylfe.cn

[E21] 超长截断加省略号
来源：http://kag.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fts.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wuj.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tea.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqr.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kcs.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://muf.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bzs.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cro.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://muc.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://khm.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxq.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aoi.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tdf.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://trt.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nza.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://eph.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kin.gzhubu.top

================================================================================
来源：http://xdc.zdbjq.cn

F. 文件与目录
来源：http://xtu.fktsv.cn

================================================================================
来源：http://qen.hcnkem.com

[F01] 读取整个文件
来源：http://jgo.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://for.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://sls.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzn.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ilh.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ufw.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://msh.cashguo.top

Ruby: File.read("a.txt")
来源：http://new.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://mfq.meibo888.top

[F02] 逐行读取文件
来源：http://cgt.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uog.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gph.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iuh.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpv.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://umb.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dse.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hvb.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xyv.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://emt.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rzc.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vif.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://slt.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smj.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xfg.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ndz.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://vme.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://idj.dianchejie.cn

[F04] 追加写入文件
来源：http://hxx.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gzh.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uvr.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hwj.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gbd.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bbq.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bwl.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://poo.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jke.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://kqr.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyo.ivvv.top

PHP:  file_exists("a.txt");
来源：http://ajj.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://yte.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://uuj.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zup.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pub.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://xgn.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://kcz.jlsjyb.cn

[F06] 删除文件
来源：http://hqr.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://zwb.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://qnr.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://mjo.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://jcq.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tgh.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://tvg.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://kzv.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://que.havefunace.top

[F07] 创建目录（含多级）
来源：http://nmr.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://afs.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pkp.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xad.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjh.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://szg.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lkw.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nsh.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jkm.xylfe.cn

[F08] 遍历目录
来源：http://hde.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mgm.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zht.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://hcu.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://kle.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mtw.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dqa.yj20258888.top

Ruby: Dir.children("dir")
来源：http://isl.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://zho.yvedp.cn

[F09] 获取文件大小
来源：http://ztv.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://nof.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://qsi.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://yee.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://img.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://jig.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hqe.wangdashe.top

Ruby: File.size("a.txt")
来源：http://ctg.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://qhy.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://lva.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lnn.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qcm.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mqa.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://yqy.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yxg.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwk.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ono.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://egv.chenzaomai.com

[F11] 复制与移动文件
来源：http://xzm.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kdf.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ihi.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qoj.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wve.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gvr.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://plq.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dbc.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ytv.cucudq.cn

[F12] CSV 读写
来源：http://jam.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emu.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bzl.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sil.gzhubu.top

TS:   // 同上
来源：http://kox.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iyg.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nme.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zbc.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pxi.hongshengwenyu.top

================================================================================
来源：http://sxi.meibo888.top

G. 面向对象
来源：http://plj.jlsjyb.cn

================================================================================
来源：http://wqk.fehbvm.com

[G01] 定义类
来源：http://btz.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://kfe.hnxiangtu.top

PHP:  class User {}
来源：http://nkw.quarkkingdee.top

JS:   class User {}
来源：http://owe.ivvv.top

TS:   class User { name: string = ""; }
来源：http://cnc.jinyuanbaomall.cn

Java: class User {}
来源：http://ccz.cheryme.top

Go:   type User struct { Name string }
来源：http://aru.jqgfzy.top

Ruby: class User; end
来源：http://ftt.ivvv.top

C#:   class User {}
来源：http://usu.iojbl.cn

[G02] 构造函数
来源：http://spe.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://jvv.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://css.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://uby.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://obk.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://nhv.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kcp.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://kab.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://tdr.wangshuangyany.cn

[G03] 实例属性
来源：http://kvm.zhoulong.xyz

Py:   self.name = "x"
来源：http://ail.meibo888.top

PHP:  public string $name = "x";
来源：http://uck.chenlongwang.top

JS:   this.name = "x";
来源：http://qcf.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://qgy.vqdsnc.cn

Java: private String name;
来源：http://vud.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zvm.iojbl.cn

Ruby: @name = "x"
来源：http://uoh.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://mbe.cucudq.cn

[G04] 定义方法
来源：http://cff.ybcxt.top

Py:   def greet(self): return self.name
来源：http://ccq.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://som.tian-w.cn

JS:   greet() { return this.name; }
来源：http://dsq.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://qju.jyoumei.cn

Java: String greet() { return name; }
来源：http://adi.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://jxm.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://cpl.cheryme.top

C#:   public string Greet() => Name;
来源：http://phs.jqgufenzy.top

[G05] 继承
来源：http://ebg.dashuyun.cn

Py:   class Admin(User): pass
来源：http://drq.wangdashe.top

PHP:  class Admin extends User {}
来源：http://oog.9152youxi.cn

JS:   class Admin extends User {}
来源：http://zqn.hnqzz.top

TS:   class Admin extends User {}
来源：http://emq.xuanzx.com

Java: class Admin extends User {}
来源：http://djm.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wft.cashguo.top

Ruby: class Admin < User; end
来源：http://wdx.xziqi.cn

C#:   class Admin : User {}
来源：http://pqu.aizwys.cn

[G06] 重写方法
来源：http://tgd.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://izx.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sfs.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://cfs.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://wik.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://ttw.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wet.yj20258.top

Ruby: def greet; "admin"; end
来源：http://vym.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://kfc.cdnleiting.top

[G07] 调用父类方法
来源：http://bmp.nwbrower.top

Py:   super().greet()
来源：http://zzz.aizwys.cn

PHP:  parent::greet();
来源：http://oia.meibo888.top

JS:   super.greet();
来源：http://rqr.shangyingyoupin.top

TS:   super.greet();
来源：http://qpn.fehbvm.com

Java: super.greet();
来源：http://jlw.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hej.svipenyu.cn

Ruby: super
来源：http://eyz.jinghuilouyu.cn

C#:   base.Greet();
来源：http://jlc.guannengcc.top

[G08] 静态方法与属性
来源：http://xqa.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gne.tian-w.cn

PHP:  public static function f() {}
来源：http://jki.9152youxi.cn

JS:   static f() {}
来源：http://rlk.tarul.cn

TS:   static f(): void {}
来源：http://lgo.yj202588.top

Java: static void f() {}
来源：http://llg.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bec.cdnleiting.top

Ruby: def self.f; end
来源：http://uzz.dianchejie.cn

C#:   public static void F() {}
来源：http://hvb.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://wqh.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://axx.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://jgq.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://suo.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://pwt.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://tjh.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://bwd.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zxq.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://rhb.redwolf501.top


<!-- 参考信息 -->