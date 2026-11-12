代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ahu.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mhb.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rdf.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://ysv.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wej.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zks.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rwu.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gxv.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://itc.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdm.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mtb.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tag.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uem.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zan.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vop.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pbu.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nea.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://dqa.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vsa.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ldr.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fyr.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hhp.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gzr.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://egq.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rdm.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ljf.52xcode.cn

[E16] 数字千分位
来源：http://vyk.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://avo.hywenlv.cn

PHP:  number_format(1234567);
来源：http://xgr.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://erc.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wgs.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zhk.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vci.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yzi.316326.xyz

C#:   1234567.ToString("N0")
来源：http://rof.wangdashe.top

[E17] 首字母大写
来源：http://arf.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fai.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vzr.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uyj.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aqe.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://flv.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fay.vqdsnc.cn

Ruby: s.capitalize
来源：http://aka.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kfr.yuxming.cn

[E18] 模板占位符替换
来源：http://zxa.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mbc.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pzg.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://edi.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eqh.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yqh.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xvk.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ohq.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hwc.ivvv.top

[E19] 多行文本按行拆分
来源：http://hzi.zhoulong.xyz

Py:   s.splitlines()
来源：http://smy.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://acr.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://ceh.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://kkc.gaohongyu789.top

Java: s.lines().toList()
来源：http://caw.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://dpj.fehbvm.com

Ruby: s.lines
来源：http://cvh.tanke756.top

C#:   s.Split('\n')
来源：http://yhv.zycfv.cn

[E20] 判断字符串是否为空
来源：http://zkq.gogol.net.cn

Py:   if not s:
来源：http://zdz.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gdc.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ffm.52xcode.cn

TS:   if (s === "") {}
来源：http://ufu.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://bvh.jqgfzy.top

Go:   if s == "" {}
来源：http://ujn.jqgfzy.top

Ruby: if s.empty?
来源：http://mru.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qqf.pycfn.com

[E21] 超长截断加省略号
来源：http://eve.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vqs.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jxy.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxr.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdf.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://plv.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://osl.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bfa.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tun.xuanzx.com

[E22] 字节长度与字符长度
来源：http://meb.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gft.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pul.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bij.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbr.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lgx.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nxg.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://sjp.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pzw.shanyushiyangkeji.top

================================================================================
来源：http://mfy.daria6918.cn

F. 文件与目录
来源：http://shr.yangfankeji.com

================================================================================
来源：http://myx.ydzc1.top

[F01] 读取整个文件
来源：http://zae.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vlb.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://dmq.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zui.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yaf.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://epw.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uct.xinyue.icu

Ruby: File.read("a.txt")
来源：http://zzl.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ekk.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://jyn.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lya.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dmq.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ios.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://irv.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ubm.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sdy.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dbz.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vxj.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://age.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nfb.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bxl.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://clo.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pjd.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kji.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xeo.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://prd.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://igv.hesvh.cn

[F04] 追加写入文件
来源：http://mgx.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcl.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lom.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwc.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwj.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gpt.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://myw.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gfa.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mlq.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://nlx.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rbs.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://ywf.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://pfn.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://cll.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oyq.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lfk.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://iow.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://rpv.cqqwz.cn

[F06] 删除文件
来源：http://kef.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://rfd.vehdjk.com

PHP:  unlink("a.txt");
来源：http://oty.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mpd.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://tvo.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zvz.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://mxs.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://wnm.havefunace.top

C#:   File.Delete("a.txt");
来源：http://yft.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://vud.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bte.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://spa.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfx.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fjp.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://psp.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rbj.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zcl.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rmv.shzxlz.cn

[F08] 遍历目录
来源：http://hig.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wut.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kgk.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://wbg.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bhd.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://otb.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kul.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://ung.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://bgk.xuanzx.com

[F09] 获取文件大小
来源：http://cep.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://jvs.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://syb.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://wth.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://ktg.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zdo.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehb.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://bvu.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://cbx.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://qsw.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gas.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://omm.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://thr.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://ztd.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tlc.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cca.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iag.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bqx.ctjpmb.com

[F11] 复制与移动文件
来源：http://fvs.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kem.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ulb.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cbu.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alf.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eep.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jye.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pvs.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tvi.redwolf501.top

[F12] CSV 读写
来源：http://yaf.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://koj.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ndv.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ats.hnxiangtu.top

TS:   // 同上
来源：http://wly.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://svs.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sod.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xxh.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pls.shangyingyoupin.top

================================================================================
来源：http://jts.chenjidiqi.icu

G. 面向对象
来源：http://fra.gzhubu.top

================================================================================
来源：http://qqp.yonumen.top

[G01] 定义类
来源：http://zvx.cucudq.cn

Py:   class User: pass
来源：http://oos.xylfe.cn

PHP:  class User {}
来源：http://eev.shanyushiyangtech.top

JS:   class User {}
来源：http://fiw.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://juf.sjlbkw.cn

Java: class User {}
来源：http://dpg.sweek.top

Go:   type User struct { Name string }
来源：http://qhz.jqgufenzy.top

Ruby: class User; end
来源：http://kuj.yuanzhike.top

C#:   class User {}
来源：http://tor.feifeiyinyue.top

[G02] 构造函数
来源：http://tlu.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://fgc.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://sxs.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://ifg.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://sif.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://mfq.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uvi.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://pyt.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://hyc.jqgufenzy.top

[G03] 实例属性
来源：http://tqn.vqdsnc.cn

Py:   self.name = "x"
来源：http://gxu.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://nio.sxryk.cn

JS:   this.name = "x";
来源：http://itm.9152youxi.cn

TS:   name: string = "x";
来源：http://kun.zhijiandao.cn

Java: private String name;
来源：http://dgw.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cqm.daxiang520.top

Ruby: @name = "x"
来源：http://djl.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://qhz.shangyingyoupin.top

[G04] 定义方法
来源：http://xqq.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://mgz.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cwr.316326.xyz

JS:   greet() { return this.name; }
来源：http://qbf.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://rif.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://zew.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://saj.meibo888.top

Ruby: def greet; @name; end
来源：http://aym.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://mpz.yfazqb.com

[G05] 继承
来源：http://pkq.chenlongwang.top

Py:   class Admin(User): pass
来源：http://nmq.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://djl.zhixingplan.top

JS:   class Admin extends User {}
来源：http://hdw.haohaochexian.top

TS:   class Admin extends User {}
来源：http://srz.c1oappe.top

Java: class Admin extends User {}
来源：http://nvt.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pjf.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://eus.redwolf501.top

C#:   class Admin : User {}
来源：http://mfj.0kj1m.cn

[G06] 重写方法
来源：http://nhp.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://adx.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://esw.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://itu.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://vgz.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://tby.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uce.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://iqh.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://jdz.hnxiangtu.top

[G07] 调用父类方法
来源：http://lcy.mhx1999.top

Py:   super().greet()
来源：http://ent.dashuyun.cn

PHP:  parent::greet();
来源：http://ohm.hywenlv.cn

JS:   super.greet();
来源：http://pue.aizwys.cn

TS:   super.greet();
来源：http://akj.aibaodan.cn

Java: super.greet();
来源：http://uab.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mlj.cucudq.cn

Ruby: super
来源：http://umb.vqdsnc.cn

C#:   base.Greet();
来源：http://hzy.svipenyu.cn

[G08] 静态方法与属性
来源：http://jgu.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aev.sjlbkw.cn

PHP:  public static function f() {}
来源：http://phv.yanxiufei.cn

JS:   static f() {}
来源：http://nja.sysykeji.top

TS:   static f(): void {}
来源：http://die.tianlin.xyz

Java: static void f() {}
来源：http://qob.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://tte.guannengcc.top

Ruby: def self.f; end
来源：http://twe.zhongyouzk.top

C#:   public static void F() {}
来源：http://sxf.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://uuy.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://rzt.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://lzl.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://msn.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://gao.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://kbg.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://ueo.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kkd.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://lzo.9152youxi.cn

[G10] 访问控制
来源：http://lyj.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://rsx.xylfe.cn

PHP:  public / protected / private
来源：http://iin.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://tac.tarul.cn

TS:   public / protected / private
来源：http://hnp.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://cnk.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cqy.andypj.xyz

Ruby: public / protected / private
来源：http://jvo.hesvh.cn

C#:   public / protected / private / internal
来源：http://mip.hnxiangtu.top

[G11] getter / setter
来源：http://tsz.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://ine.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fgl.sweek.top

JS:   get name() { return this._name; }
来源：http://zih.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://ulh.daria6918.cn

Java: public String getName() { return name; }
来源：http://opd.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xzm.hongshengwenyu.top


<!-- 参考信息 -->