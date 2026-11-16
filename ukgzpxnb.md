代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wyx.ybcxt.top

Ruby: s.count("a")
来源：http://ljf.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://pzm.gzhubu.top

[E13] 逐字符遍历
来源：http://qzl.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://xsn.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noh.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zlv.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://gwc.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://shb.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sjh.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bog.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mpp.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://qep.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cmt.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xko.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sgy.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wtj.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tlb.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uja.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oea.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hje.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://gvj.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iql.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ukq.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://swl.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://inm.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nlr.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wje.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://apv.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yfv.zhoulong.xyz

[E16] 数字千分位
来源：http://tbt.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://kjs.52xcode.cn

PHP:  number_format(1234567);
来源：http://aik.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wkq.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://hbz.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xip.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bwa.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pin.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://plg.redwolf501.top

[E17] 首字母大写
来源：http://fma.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mvd.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cvk.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjq.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmr.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zvs.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://epe.tanke756.top

Ruby: s.capitalize
来源：http://vge.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bmd.hnqzz.top

[E18] 模板占位符替换
来源：http://iyy.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qbn.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qdl.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eba.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://itx.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwi.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hjd.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lyc.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tqq.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://xtk.316326.xyz

Py:   s.splitlines()
来源：http://mea.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tww.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://cvt.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://iod.fengsongda.top

Java: s.lines().toList()
来源：http://qmc.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://oso.redwolf501.top

Ruby: s.lines
来源：http://otl.yangfankeji.com

C#:   s.Split('\n')
来源：http://out.fengsongda.top

[E20] 判断字符串是否为空
来源：http://nyj.xziqi.cn

Py:   if not s:
来源：http://ypi.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://egn.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gen.xziqi.cn

TS:   if (s === "") {}
来源：http://axy.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://log.birdmap.top

Go:   if s == "" {}
来源：http://ybu.zhijiandao.cn

Ruby: if s.empty?
来源：http://ijf.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hkv.yuanzhike.top

[E21] 超长截断加省略号
来源：http://vyx.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ubd.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kqf.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbw.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbn.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xnh.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://lui.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hhc.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://urv.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://env.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://smw.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tla.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mra.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://opv.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nyq.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xjm.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://eyj.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ttg.gaohongyu789.top

================================================================================
来源：http://ilu.jinghuilouyu.cn

F. 文件与目录
来源：http://ymo.jianghu66.top

================================================================================
来源：http://asl.tianlin.xyz

[F01] 读取整个文件
来源：http://wyy.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dgd.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://vgt.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jda.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://inl.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zpv.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ygr.chenzaomai.com

Ruby: File.read("a.txt")
来源：http://oyx.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://lew.guowangkeji.top

[F02] 逐行读取文件
来源：http://bie.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zpu.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wrn.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ivc.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqg.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://twg.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvx.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cla.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hen.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://eib.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mwl.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://epc.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fuo.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://opb.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xhk.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gin.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://qfj.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ejf.mhx1999.top

[F04] 追加写入文件
来源：http://oic.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yno.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://von.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xlr.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ksp.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://phg.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bwm.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xwv.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sio.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://rsk.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uuo.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://cbw.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://ygc.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://sho.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fgy.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwm.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://xbw.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://sac.andypj.xyz

[F06] 删除文件
来源：http://qrp.daria6918.cn

Py:   os.remove("a.txt")
来源：http://oxm.pycfn.com

PHP:  unlink("a.txt");
来源：http://sbg.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sck.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://tdt.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mgs.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://pwc.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://psk.yonumen.top

C#:   File.Delete("a.txt");
来源：http://zvu.redwolf501.top

[F07] 创建目录（含多级）
来源：http://mhi.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hce.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oqi.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bij.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zjz.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kux.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xap.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nxv.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fsp.zhiwuduotai.top

[F08] 遍历目录
来源：http://spq.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xkj.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nkw.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://upf.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://jkp.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yhw.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mql.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://hul.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://dpk.sjlbkw.cn

[F09] 获取文件大小
来源：http://dhx.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://emz.birdmap.top

PHP:  filesize("a.txt");
来源：http://evf.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://keq.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://plm.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://qgz.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lco.zycfv.cn

Ruby: File.size("a.txt")
来源：http://mmj.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://wpx.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://yuq.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dmq.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jrk.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mce.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://cvv.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ulk.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fvm.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kki.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uzg.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://kqr.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cve.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://smj.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqo.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jad.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pod.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ecv.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fmq.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lzi.ehwqpu.com

[F12] CSV 读写
来源：http://cqk.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlb.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kwu.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yam.ctjpmb.com

TS:   // 同上
来源：http://qoz.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uiv.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uar.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xwf.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fev.ctjpmb.com

================================================================================
来源：http://pwn.hywenlv.cn

G. 面向对象
来源：http://yve.nanxinkj.top

================================================================================
来源：http://dio.yanxiufei.cn

[G01] 定义类
来源：http://ywv.chenjidiqi.icu

Py:   class User: pass
来源：http://ult.yuxming.cn

PHP:  class User {}
来源：http://raj.yvedp.cn

JS:   class User {}
来源：http://jol.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://rds.xylfe.cn

Java: class User {}
来源：http://agj.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://iqu.tianlin.xyz

Ruby: class User; end
来源：http://arv.ppjwa.cn

C#:   class User {}
来源：http://tpx.gogol.net.cn

[G02] 构造函数
来源：http://elh.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://dzq.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://bsi.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://osd.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://jkn.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://koa.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pzh.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://fyy.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://dom.hfpthk.cn

[G03] 实例属性
来源：http://abp.sjlbkw.cn

Py:   self.name = "x"
来源：http://orr.xylfe.cn

PHP:  public string $name = "x";
来源：http://jpw.zhongyouzk.top

JS:   this.name = "x";
来源：http://yna.shangyingyoupin.top

TS:   name: string = "x";
来源：http://scm.jinqigfzy.top

Java: private String name;
来源：http://fag.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://udh.xuetiantiany.cn

Ruby: @name = "x"
来源：http://bjn.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cde.hnxiangtu.top

[G04] 定义方法
来源：http://qon.sysykeji.top

Py:   def greet(self): return self.name
来源：http://qrg.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://pen.andypj.xyz

JS:   greet() { return this.name; }
来源：http://wjk.sweek.top

TS:   greet(): string { return this.name; }
来源：http://dly.zhixingplan.top

Java: String greet() { return name; }
来源：http://isg.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ovr.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://pzm.xziqi.cn

C#:   public string Greet() => Name;
来源：http://tdv.yvedp.cn

[G05] 继承
来源：http://tmh.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://lzd.tanke756.top

PHP:  class Admin extends User {}
来源：http://ozn.zhengqikj.top

JS:   class Admin extends User {}
来源：http://qje.vehdjk.com

TS:   class Admin extends User {}
来源：http://dmb.hammf.cn

Java: class Admin extends User {}
来源：http://bsm.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kci.vehdjk.com

Ruby: class Admin < User; end
来源：http://wfi.jianghu66.top

C#:   class Admin : User {}
来源：http://rlz.svipenyu.cn

[G06] 重写方法
来源：http://pbg.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://qwg.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ufp.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://ypi.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://tuj.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://tfj.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vuc.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://nub.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://zhx.ppjwa.cn

[G07] 调用父类方法
来源：http://hro.gogol.net.cn

Py:   super().greet()
来源：http://dvm.snrcjt.cn

PHP:  parent::greet();
来源：http://ebh.0kj1m.cn

JS:   super.greet();
来源：http://ulf.gotoacloud.top

TS:   super.greet();
来源：http://wqg.shzxlz.cn

Java: super.greet();
来源：http://qag.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yol.meibo888.top

Ruby: super
来源：http://mur.sysykeji.top

C#:   base.Greet();
来源：http://bxk.shzxlz.cn

[G08] 静态方法与属性
来源：http://sny.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ivn.jlsjyb.cn

PHP:  public static function f() {}
来源：http://zvg.smart0.xyz

JS:   static f() {}
来源：http://wtx.quarkkingdee.top

TS:   static f(): void {}
来源：http://yuo.xuanzx.com

Java: static void f() {}
来源：http://kcu.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pno.nanxuanxn.top

Ruby: def self.f; end
来源：http://gxr.bbcook.cn

C#:   public static void F() {}
来源：http://bih.zycfv.cn

[G09] 接口 / 抽象类
来源：http://hxp.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://tsj.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jnh.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://snf.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://xls.fktsv.cn

Java: interface Shape { double area(); }
来源：http://xfn.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://jfq.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rnl.sweek.top

C#:   interface IShape { double Area(); }
来源：http://xks.redwolf501.top

[G10] 访问控制
来源：http://aoh.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sgt.birdmap.top

PHP:  public / protected / private
来源：http://dje.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://vxv.gzhubu.top

TS:   public / protected / private
来源：http://nkg.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://zbv.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cka.fengsongda.top

Ruby: public / protected / private
来源：http://ada.zdbjq.cn

C#:   public / protected / private / internal
来源：http://pcj.zhongyouzk.top

[G11] getter / setter
来源：http://qxk.c1oappe.top

Py:   @property 与 @x.setter
来源：http://oeu.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://osf.daria6918.cn


<!-- 参考信息 -->