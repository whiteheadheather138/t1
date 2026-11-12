代发 wailian999

Ruby: s.reverse
来源：http://nrk.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://nxp.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://avk.redwolf501.top

Py:   s.count("a")
来源：http://xgz.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://key.vehdjk.com

JS:   s.split("a").length - 1
来源：http://gei.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://klm.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bel.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://lyo.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://ykl.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://qka.zhijiandao.cn

[E13] 逐字符遍历
来源：http://hzg.tanke756.top

Py:   for ch in s: print(ch)
来源：http://fdf.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpa.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ztm.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jdm.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vbs.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eem.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mey.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ygj.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://yiy.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xab.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://was.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mdo.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bjx.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bnb.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://svh.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yvh.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xgj.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://vrg.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lvh.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://njh.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hum.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fzr.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vzu.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sak.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ltz.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://otr.yvedp.cn

[E16] 数字千分位
来源：http://fqs.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://qxq.wangdashe.top

PHP:  number_format(1234567);
来源：http://vrr.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ley.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vss.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrt.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dgb.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnl.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://mbd.nanxinkj.top

[E17] 首字母大写
来源：http://syt.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wob.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://zje.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zca.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuc.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ywb.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qfc.epnwcf.com

Ruby: s.capitalize
来源：http://mfy.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kjd.0kj1m.cn

[E18] 模板占位符替换
来源：http://arc.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pkg.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cig.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tyt.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zvk.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iou.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://izk.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eal.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oky.hnqzz.top

[E19] 多行文本按行拆分
来源：http://ugk.c1oappe.top

Py:   s.splitlines()
来源：http://lie.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hmz.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://liy.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://fvc.hysaishi.cn

Java: s.lines().toList()
来源：http://xqt.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://obx.xziqi.cn

Ruby: s.lines
来源：http://gpd.yj202588.top

C#:   s.Split('\n')
来源：http://equ.vehdjk.com

[E20] 判断字符串是否为空
来源：http://tuf.cdnleiting.top

Py:   if not s:
来源：http://vop.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zlr.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tiq.hywenlv.cn

TS:   if (s === "") {}
来源：http://rhm.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://jeq.guowangkeji.top

Go:   if s == "" {}
来源：http://uam.dashuyun.cn

Ruby: if s.empty?
来源：http://fni.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gxx.meibo888.top

[E21] 超长截断加省略号
来源：http://ytx.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://odq.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yfj.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oms.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezf.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ekf.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zzx.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cbt.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://irt.sxryk.cn

[E22] 字节长度与字符长度
来源：http://gpj.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sgl.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kpu.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mee.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://izd.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qsq.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ewj.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://ozn.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://omh.ppjwa.cn

================================================================================
来源：http://ujm.redwolf501.top

F. 文件与目录
来源：http://wwt.ehwqpu.com

================================================================================
来源：http://kvr.yangfankeji.com

[F01] 读取整个文件
来源：http://zzm.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://txc.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://cbe.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fre.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://olz.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://luv.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ewx.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://gec.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://lur.uphjek.com

[F02] 逐行读取文件
来源：http://ivp.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://azw.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dcd.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilj.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://odp.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cns.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kdh.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ieb.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwy.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://djo.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cex.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://llc.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jyl.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cny.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ojv.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vdp.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://cqd.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wuz.ydjk.org.cn

[F04] 追加写入文件
来源：http://slz.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ddo.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zqr.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uhh.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hgj.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bhd.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kaw.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xuz.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ydn.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://qvr.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dxj.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://upm.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://ynh.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://hfh.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://xfg.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uwk.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://izn.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://rkt.cqqwz.cn

[F06] 删除文件
来源：http://ubj.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://fqf.havefunace.top

PHP:  unlink("a.txt");
来源：http://ymt.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://afa.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qlz.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ddu.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://was.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://uof.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://ntc.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://wuq.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lgh.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://swb.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngn.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxv.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lgu.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pab.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hor.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://one.xylfe.cn

[F08] 遍历目录
来源：http://wxo.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nxu.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vee.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://nkv.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://ygg.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qjk.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bvk.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://lby.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://vzy.cucudq.cn

[F09] 获取文件大小
来源：http://wsd.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://yyb.yj202588.top

PHP:  filesize("a.txt");
来源：http://kew.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://tkh.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://rep.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://ida.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ssx.mhx1999.top

Ruby: File.size("a.txt")
来源：http://vlk.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://sex.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://bcd.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fbu.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gfk.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://otv.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://doa.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ejt.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xeg.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zfs.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sri.nanxuanxn.top

[F11] 复制与移动文件
来源：http://nyy.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vir.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sdk.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://czl.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyx.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://opw.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pwl.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vcu.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vug.yangfankeji.com

[F12] CSV 读写
来源：http://chf.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jky.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hxd.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gto.xylfe.cn

TS:   // 同上
来源：http://tkb.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xhh.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://phk.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xkl.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gid.aibaodan.cn

================================================================================
来源：http://jng.tian-w.cn

G. 面向对象
来源：http://hww.jyoumei.cn

================================================================================
来源：http://bfl.gzhubu.top

[G01] 定义类
来源：http://kdr.daria6918.cn

Py:   class User: pass
来源：http://erj.hysaishi.cn

PHP:  class User {}
来源：http://pdv.gotoacloud.top

JS:   class User {}
来源：http://mtn.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://oku.jinghuilouyu.cn

Java: class User {}
来源：http://hma.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://lgl.yangfankeji.com

Ruby: class User; end
来源：http://adx.nwbrower.top

C#:   class User {}
来源：http://ita.jiagoushi.top

[G02] 构造函数
来源：http://wzt.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://uhm.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://jrx.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://tvz.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://ugw.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://fev.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wyc.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://syc.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://rku.redwolf501.top

[G03] 实例属性
来源：http://xhj.zdqjudy.top

Py:   self.name = "x"
来源：http://acx.yj202588.top

PHP:  public string $name = "x";
来源：http://sta.yonumen.top

JS:   this.name = "x";
来源：http://uqm.316326.xyz

TS:   name: string = "x";
来源：http://pfw.bjfxy.top

Java: private String name;
来源：http://bpj.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zao.bjfxy.top

Ruby: @name = "x"
来源：http://avg.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://slr.birdmap.top

[G04] 定义方法
来源：http://zyx.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://skv.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mka.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://tzy.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://kdo.gogol.net.cn

Java: String greet() { return name; }
来源：http://ikb.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ugd.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://uut.xinyue.icu

C#:   public string Greet() => Name;
来源：http://ign.tianlin.xyz

[G05] 继承
来源：http://pqn.c1oappe.top

Py:   class Admin(User): pass
来源：http://asw.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://uvc.tarul.cn

JS:   class Admin extends User {}
来源：http://mcj.yangfankeji.com

TS:   class Admin extends User {}
来源：http://mfy.yonumen.top

Java: class Admin extends User {}
来源：http://fhw.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yjj.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://wso.fengsongda.top

C#:   class Admin : User {}
来源：http://vek.zhaomingkeji.xyz

[G06] 重写方法
来源：http://nje.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://huq.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tdo.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://gum.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://ers.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://hhx.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rnx.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://oec.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://cmz.guowangkeji.top

[G07] 调用父类方法
来源：http://guy.cashguo.top

Py:   super().greet()
来源：http://gpt.zhixingplan.top

PHP:  parent::greet();
来源：http://vhj.sysykeji.top

JS:   super.greet();
来源：http://gbj.xuetiantiany.cn

TS:   super.greet();
来源：http://xoa.tian-w.cn

Java: super.greet();
来源：http://hdg.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qcg.aizwys.cn

Ruby: super
来源：http://bee.jianghu66.top

C#:   base.Greet();
来源：http://dld.ehwqpu.com

[G08] 静态方法与属性
来源：http://zpd.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xix.hammf.cn

PHP:  public static function f() {}
来源：http://caz.jlsjyb.cn

JS:   static f() {}
来源：http://kuz.dashuyun.cn

TS:   static f(): void {}
来源：http://nvj.redwolf501.top

Java: static void f() {}
来源：http://vhy.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qia.cheryme.top

Ruby: def self.f; end
来源：http://wdn.chenzaomai.com

C#:   public static void F() {}
来源：http://twq.pycfn.com

[G09] 接口 / 抽象类
来源：http://whh.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://wsp.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://tqf.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pfw.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://mkq.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://sfp.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://utt.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yeo.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://wvy.fzhhl.top

[G10] 访问控制
来源：http://pcf.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dxx.gzhubu.top

PHP:  public / protected / private
来源：http://czp.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://wdr.bjfxy.top


<!-- 参考信息 -->