代发 wailian999

Ruby: s.reverse
来源：http://ahi.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://edw.zycfv.cn

[E12] 统计某字符出现次数
来源：http://dxq.daria6918.cn

Py:   s.count("a")
来源：http://lff.yj202588.top

PHP:  substr_count($s, "a");
来源：http://ysr.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://vwq.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://ekn.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tuz.tanke756.top

Go:   strings.Count(s, "a")
来源：http://bik.yj202588.top

Ruby: s.count("a")
来源：http://qve.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://iqh.sweek.top

[E13] 逐字符遍历
来源：http://lwf.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://tfj.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zcy.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jrt.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://oyt.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oga.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqw.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mvx.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yyz.52xcode.cn

[E14] URL 编码与 Base64
来源：http://yem.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://odd.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qte.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zgq.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bmk.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vku.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wte.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nxf.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zvm.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://ibj.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://czs.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://scr.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uqh.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sfj.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ehu.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vri.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://egn.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vqw.jqgfzy.top

[E16] 数字千分位
来源：http://knb.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://esi.xziqi.cn

PHP:  number_format(1234567);
来源：http://dsa.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pmu.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://osv.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ogb.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ixk.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wxf.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://upl.chenlongwang.top

[E17] 首字母大写
来源：http://xgo.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://khr.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tpp.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jce.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qyi.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asd.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nto.uphjek.com

Ruby: s.capitalize
来源：http://xxp.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kjo.jqgfzy.top

[E18] 模板占位符替换
来源：http://ydf.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcy.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fte.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rgg.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qff.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pab.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uqw.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlk.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hoq.yuxming.cn

[E19] 多行文本按行拆分
来源：http://nly.c1oappe.top

Py:   s.splitlines()
来源：http://pgu.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hkb.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://mpa.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://ydl.bjfxy.top

Java: s.lines().toList()
来源：http://uog.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://uda.tarul.cn

Ruby: s.lines
来源：http://cis.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://poe.yvedp.cn

[E20] 判断字符串是否为空
来源：http://kuf.chenzaomai.com

Py:   if not s:
来源：http://ljn.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fyj.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ilu.sufxvd.cn

TS:   if (s === "") {}
来源：http://oel.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://qsg.andypj.xyz

Go:   if s == "" {}
来源：http://heo.cqqwz.cn

Ruby: if s.empty?
来源：http://lgz.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xfu.cashguo.top

[E21] 超长截断加省略号
来源：http://jmv.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nus.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rnu.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qhu.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dts.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cul.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://rch.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qsj.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jdl.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://wli.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://efa.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ubn.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vqz.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://abr.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sas.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://emn.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://lbs.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://paa.hcnkem.com

================================================================================
来源：http://xwr.guannengcc.top

F. 文件与目录
来源：http://mke.jinqigfzy.top

================================================================================
来源：http://ewr.vqdsnc.cn

[F01] 读取整个文件
来源：http://hsv.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vcr.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://fpt.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://itl.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ryz.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iij.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ghl.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://ktn.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://epy.gotoacloud.top

[F02] 逐行读取文件
来源：http://uzf.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gha.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ypz.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jjl.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ujv.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svk.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bgb.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pmi.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hcn.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://lwy.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bvd.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vcv.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nku.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fww.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rdu.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://grd.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://wnj.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jkq.yj20258888.top

[F04] 追加写入文件
来源：http://ypo.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://doj.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mlv.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://plh.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baj.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://voa.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iep.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eyg.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cwd.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://wwl.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://czn.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://lrv.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://pag.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://lnz.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wqp.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ttg.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://dqp.yongpay.top

C#:   File.Exists("a.txt")
来源：http://nwj.yongpay.top

[F06] 删除文件
来源：http://qyk.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://ucm.birdmap.top

PHP:  unlink("a.txt");
来源：http://yaa.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bux.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://woe.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://twk.hammf.cn

Go:   os.Remove("a.txt")
来源：http://fif.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://zlj.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://gpa.guannengcc.top

[F07] 创建目录（含多级）
来源：http://izv.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nyj.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ntk.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gcf.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rov.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qrz.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cne.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wzy.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sxu.hnqzz.top

[F08] 遍历目录
来源：http://jvd.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pkg.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ihl.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://smi.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://umu.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fiz.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oar.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://bpv.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://cwr.jiagoushi.top

[F09] 获取文件大小
来源：http://alh.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://wja.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://azq.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://jib.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://ajf.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://uiw.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ogx.xylfe.cn

Ruby: File.size("a.txt")
来源：http://tyf.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://exb.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wbm.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mbg.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://brl.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tpd.cashguo.top

TS:   path.extname("a.txt")
来源：http://uhw.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bsl.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yhy.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fot.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pha.zhengqikj.top

[F11] 复制与移动文件
来源：http://sxy.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ark.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hku.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjl.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzm.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zkr.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nex.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ccd.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bhh.yj20258.top

[F12] CSV 读写
来源：http://pkk.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hik.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yxg.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://csp.zdqjudy.top

TS:   // 同上
来源：http://lly.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yek.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gzd.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://src.dashuyun.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qgr.iojbl.cn

================================================================================
来源：http://zat.dashuyun.cn

G. 面向对象
来源：http://efk.dashuyun.cn

================================================================================
来源：http://hqp.ppjwa.cn

[G01] 定义类
来源：http://udk.jqgufenzy.top

Py:   class User: pass
来源：http://guf.daxiang520.top

PHP:  class User {}
来源：http://yri.xuanzx.com

JS:   class User {}
来源：http://wox.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://ijp.zdqjudy.top

Java: class User {}
来源：http://jfk.birdmap.top

Go:   type User struct { Name string }
来源：http://bwz.zhaomingkeji.xyz

Ruby: class User; end
来源：http://nbp.zhoulong.xyz

C#:   class User {}
来源：http://xla.ydzc1.top

[G02] 构造函数
来源：http://ujo.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://dhi.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://crr.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://nbx.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://ubu.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://zzb.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dkm.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://ubb.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://kuq.vehdjk.com

[G03] 实例属性
来源：http://pqo.yanxiufei.cn

Py:   self.name = "x"
来源：http://ejy.daxiang520.top

PHP:  public string $name = "x";
来源：http://bvg.ydjk.org.cn

JS:   this.name = "x";
来源：http://oqx.yj20258888.top

TS:   name: string = "x";
来源：http://igi.mhx1999.top

Java: private String name;
来源：http://wsg.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nlx.yangfankeji.com

Ruby: @name = "x"
来源：http://xov.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://cry.quarkkingdee.top

[G04] 定义方法
来源：http://fbz.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://yji.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wnh.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://dkw.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://ysy.hammf.cn

Java: String greet() { return name; }
来源：http://yiy.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://thl.pycfn.com

Ruby: def greet; @name; end
来源：http://kvl.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://nlz.yuanzhike.top

[G05] 继承
来源：http://uhm.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://prd.zycfv.cn

PHP:  class Admin extends User {}
来源：http://plx.snrcjt.cn

JS:   class Admin extends User {}
来源：http://rdo.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://rna.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://umm.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vre.52xcode.cn

Ruby: class Admin < User; end
来源：http://pjl.316326.xyz

C#:   class Admin : User {}
来源：http://cly.zdbjq.cn

[G06] 重写方法
来源：http://ojc.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://hma.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mno.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://foe.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://byk.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://yyg.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eyv.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://gpa.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://zim.yangfankeji.com

[G07] 调用父类方法
来源：http://wwd.zhixingplan.top

Py:   super().greet()
来源：http://zbk.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://bzx.tarul.cn

JS:   super.greet();
来源：http://hnk.daria6918.cn

TS:   super.greet();
来源：http://vid.gogol.net.cn

Java: super.greet();
来源：http://aey.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bnm.tarul.cn

Ruby: super
来源：http://jlc.bjfxy.top

C#:   base.Greet();
来源：http://zae.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://spm.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://adf.guannengcc.top

PHP:  public static function f() {}
来源：http://hag.pycfn.com

JS:   static f() {}
来源：http://tcd.hnxiangtu.top

TS:   static f(): void {}
来源：http://lnm.zhijiandao.cn

Java: static void f() {}
来源：http://mzp.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://flx.hcnkem.com

Ruby: def self.f; end
来源：http://qaa.yanxiufei.cn

C#:   public static void F() {}
来源：http://prq.tarul.cn

[G09] 接口 / 抽象类
来源：http://iea.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://heu.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://eis.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qqb.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://cqw.sysykeji.top

Java: interface Shape { double area(); }
来源：http://xap.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://xjg.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uxl.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://tvc.jinqigfzy.top

[G10] 访问控制
来源：http://hon.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://qlq.ivvv.top

PHP:  public / protected / private
来源：http://diy.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://xmt.hywenlv.cn


<!-- 参考信息 -->