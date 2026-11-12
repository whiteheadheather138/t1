代发 wailian999

Ruby: s.reverse
来源：http://xhp.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://vuq.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://rbq.jinqigufen.top

Py:   s.count("a")
来源：http://dgr.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://xht.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://ywj.cucudq.cn

TS:   s.split("a").length - 1
来源：http://hlc.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qny.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://eiw.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://zse.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://hkt.zhijiandao.cn

[E13] 逐字符遍历
来源：http://sqi.tarul.cn

Py:   for ch in s: print(ch)
来源：http://mje.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gfw.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xhy.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://zwl.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ydf.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afo.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pxk.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yky.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://akk.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kzd.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://byb.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwn.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ziy.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rqo.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mku.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://usj.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xmj.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://pqk.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nkd.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nda.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nwk.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://cbz.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://drg.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cka.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hmh.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mcp.hongshengwenyu.top

[E16] 数字千分位
来源：http://ter.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://ymt.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://iqv.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://auw.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wbh.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lst.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vte.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baz.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://aez.cheryme.top

[E17] 首字母大写
来源：http://htn.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://huu.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://yyi.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wep.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hpa.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knc.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vsr.jyoumei.cn

Ruby: s.capitalize
来源：http://bot.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xhk.yvedp.cn

[E18] 模板占位符替换
来源：http://vvu.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hzn.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pzb.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://zyi.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qgu.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fri.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zbb.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rak.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vjg.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://aef.yangfankeji.com

Py:   s.splitlines()
来源：http://fmt.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pcl.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://oty.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://pwo.ydzc1.top

Java: s.lines().toList()
来源：http://iwa.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ufx.yuxming.cn

Ruby: s.lines
来源：http://ytq.daria6918.cn

C#:   s.Split('\n')
来源：http://eqk.bjfxy.top

[E20] 判断字符串是否为空
来源：http://bjj.tianlin.xyz

Py:   if not s:
来源：http://wel.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tjw.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zdo.hnqzz.top

TS:   if (s === "") {}
来源：http://dqj.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://mzd.snrcjt.cn

Go:   if s == "" {}
来源：http://jhc.haohaochexian.top

Ruby: if s.empty?
来源：http://aed.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nhm.daxiang520.top

[E21] 超长截断加省略号
来源：http://abw.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qdc.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kjz.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usv.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcu.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://crz.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://loo.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ktc.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xui.hnqzz.top

[E22] 字节长度与字符长度
来源：http://gpd.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dxb.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jrh.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxr.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hmm.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wiq.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qrw.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://imy.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tuh.zhixingplan.top

================================================================================
来源：http://gls.zhaomingkeji.xyz

F. 文件与目录
来源：http://vda.haohaochexian.top

================================================================================
来源：http://rmf.yuanzhike.top

[F01] 读取整个文件
来源：http://uxs.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qcg.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://aho.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://diq.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ftt.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ydw.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rez.fzhhl.top

Ruby: File.read("a.txt")
来源：http://mjv.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://dob.nanxuanxn.top

[F02] 逐行读取文件
来源：http://ycy.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwz.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ujg.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arv.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpw.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hxy.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ijp.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bcm.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fcr.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://cnv.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bmi.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fca.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xyb.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyv.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nen.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xtq.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vop.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xey.cqqwz.cn

[F04] 追加写入文件
来源：http://mvr.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bnb.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gop.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brk.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efl.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cpg.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ube.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zsc.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rvt.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://vqn.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hai.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://xap.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://qxj.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://wmi.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jgs.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ovk.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://dab.cashguo.top

C#:   File.Exists("a.txt")
来源：http://vec.tian-w.cn

[F06] 删除文件
来源：http://qqw.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://fri.tarul.cn

PHP:  unlink("a.txt");
来源：http://ihj.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hjk.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nxl.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vfg.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://yig.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://xhi.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://rae.yj20258.top

[F07] 创建目录（含多级）
来源：http://wkf.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sbu.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vjm.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhx.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mou.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ivz.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://clu.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gwf.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aah.gaohongyu789.top

[F08] 遍历目录
来源：http://qia.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qkh.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hjh.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://vun.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://euk.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mkw.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nth.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://plo.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://jbg.wangdashe.top

[F09] 获取文件大小
来源：http://uug.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://hea.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://mea.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://bsf.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://dpq.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://aug.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dqw.smart0.xyz

Ruby: File.size("a.txt")
来源：http://guf.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://dgp.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://uax.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://neh.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvg.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kbb.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://ndm.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gef.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lkl.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vjc.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cit.jqgfzy.top

[F11] 复制与移动文件
来源：http://utr.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qtm.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://viv.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlc.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjs.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tth.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gyu.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oqt.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gmu.jinqigufen.top

[F12] CSV 读写
来源：http://xim.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://swt.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ako.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vvg.fanxiaobao.xyz

TS:   // 同上
来源：http://jjb.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mbd.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fpo.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qpu.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mwu.aizwys.cn

================================================================================
来源：http://xub.tianlin.xyz

G. 面向对象
来源：http://fnx.fengsongda.top

================================================================================
来源：http://wgs.tarul.cn

[G01] 定义类
来源：http://cbe.jyoumei.cn

Py:   class User: pass
来源：http://gho.yangfankeji.com

PHP:  class User {}
来源：http://inr.tanke756.top

JS:   class User {}
来源：http://klg.cashguo.top

TS:   class User { name: string = ""; }
来源：http://uoe.yangfankeji.com

Java: class User {}
来源：http://obr.yj20258.top

Go:   type User struct { Name string }
来源：http://zqn.smart0.xyz

Ruby: class User; end
来源：http://fee.xziqi.cn

C#:   class User {}
来源：http://pzb.feifeiyinyue.top

[G02] 构造函数
来源：http://vgn.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://dhi.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://irh.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://vbw.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://pvj.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://pmj.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mlt.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://gta.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://iki.gogol.net.cn

[G03] 实例属性
来源：http://tcm.quarkkingdee.top

Py:   self.name = "x"
来源：http://lhn.yongpay.top

PHP:  public string $name = "x";
来源：http://uum.jianghu66.top

JS:   this.name = "x";
来源：http://fvl.sweek.top

TS:   name: string = "x";
来源：http://iwo.zhaomingkeji.xyz

Java: private String name;
来源：http://rnm.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ysq.sysykeji.top

Ruby: @name = "x"
来源：http://yng.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://hgd.andypj.xyz

[G04] 定义方法
来源：http://kcj.andypj.xyz

Py:   def greet(self): return self.name
来源：http://llp.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pyo.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://hbv.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://uew.sysykeji.top

Java: String greet() { return name; }
来源：http://cza.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ipf.wangdashe.top

Ruby: def greet; @name; end
来源：http://bdk.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://npn.jinqigfzy.top

[G05] 继承
来源：http://rwe.tanke756.top

Py:   class Admin(User): pass
来源：http://win.iojbl.cn

PHP:  class Admin extends User {}
来源：http://rwl.yangfankeji.com

JS:   class Admin extends User {}
来源：http://bcn.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://hxp.dashuyun.cn

Java: class Admin extends User {}
来源：http://ebj.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vnh.gotoacloud.top

Ruby: class Admin < User; end
来源：http://cva.jianghu66.top

C#:   class Admin : User {}
来源：http://lay.pycfn.com

[G06] 重写方法
来源：http://gba.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://xny.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tjx.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://dda.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://tsj.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://kkr.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fzi.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://rev.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://kkz.fehbvm.com

[G07] 调用父类方法
来源：http://guj.daria6918.cn

Py:   super().greet()
来源：http://fzr.hcnkem.com

PHP:  parent::greet();
来源：http://eao.sxryk.cn

JS:   super.greet();
来源：http://ifm.yanxiufei.cn

TS:   super.greet();
来源：http://uky.xuanzx.com

Java: super.greet();
来源：http://iqj.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pqg.zhongyouzk.top

Ruby: super
来源：http://sgo.hongshengwenyu.top

C#:   base.Greet();
来源：http://ztj.yj20258888.top

[G08] 静态方法与属性
来源：http://kqi.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nla.vqdsnc.cn

PHP:  public static function f() {}
来源：http://ajo.snrcjt.cn

JS:   static f() {}
来源：http://zjo.ehwqpu.com

TS:   static f(): void {}
来源：http://yws.shanyushiyangtech.top

Java: static void f() {}
来源：http://mwu.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qbn.yuanzhike.top

Ruby: def self.f; end
来源：http://slh.tian-w.cn

C#:   public static void F() {}
来源：http://krq.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://lfj.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://lim.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://gsc.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jym.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://mbr.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://dpy.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ujw.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nao.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://jcx.yongpay.top

[G10] 访问控制
来源：http://bci.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://cyd.gzhubu.top

PHP:  public / protected / private
来源：http://bff.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://pkc.xuanzx.com


<!-- 参考信息 -->