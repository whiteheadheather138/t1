代发 wailian999

Go:   strings.Count(s, "a")
来源：http://dyf.shangyingyoupin.top

Ruby: s.count("a")
来源：http://khm.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://bou.epnwcf.com

[E13] 逐字符遍历
来源：http://zjs.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://zef.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rfj.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eet.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kwh.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uaa.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ymb.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://etw.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cct.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://tjq.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lxo.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eur.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tke.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://acf.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uls.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fss.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vhj.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://udh.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://lxu.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xgp.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oom.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eze.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bsm.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dgw.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jzv.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://waj.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wtz.aibaodan.cn

[E16] 数字千分位
来源：http://qfa.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://ojb.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://zbg.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fwh.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dov.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://anc.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gec.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://knp.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://wgi.yfazqb.com

[E17] 首字母大写
来源：http://ynv.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hks.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eih.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ioj.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://znn.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fpv.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jpm.andypj.xyz

Ruby: s.capitalize
来源：http://ikt.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://epq.yangfankeji.com

[E18] 模板占位符替换
来源：http://kvn.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qym.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gwt.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://huz.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yll.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qbc.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wyq.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwc.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opc.tarul.cn

[E19] 多行文本按行拆分
来源：http://mvz.birdmap.top

Py:   s.splitlines()
来源：http://dqd.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bwa.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://kes.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://ika.ppjwa.cn

Java: s.lines().toList()
来源：http://uta.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://qao.ivvv.top

Ruby: s.lines
来源：http://ubr.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://wyu.pycfn.com

[E20] 判断字符串是否为空
来源：http://aht.dianchejie.cn

Py:   if not s:
来源：http://ely.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hmj.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://myz.kuanghao11.cn

TS:   if (s === "") {}
来源：http://yhv.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://afz.yanxiufei.cn

Go:   if s == "" {}
来源：http://hjs.jyoumei.cn

Ruby: if s.empty?
来源：http://gto.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sgn.chenlongwang.top

[E21] 超长截断加省略号
来源：http://hvv.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbq.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mio.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oma.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egd.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wgv.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://nqy.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ciw.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vet.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://hzc.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aaz.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pcd.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rea.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqp.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mkn.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fls.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://wky.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lak.tian-w.cn

================================================================================
来源：http://gtg.zhijiandao.cn

F. 文件与目录
来源：http://njf.9152youxi.cn

================================================================================
来源：http://akz.hywenlv.cn

[F01] 读取整个文件
来源：http://dch.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eph.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://ian.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zzw.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lgu.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ecs.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ium.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://bod.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://zev.zhijiandao.cn

[F02] 逐行读取文件
来源：http://nfq.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bro.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lyp.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwe.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifm.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqm.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npz.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mbi.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tli.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://wpn.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ker.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://omb.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozk.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tjd.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tja.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zhl.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://yns.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zou.yueranfly.top

[F04] 追加写入文件
来源：http://zwy.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fed.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xbk.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxt.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjk.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bin.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pml.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vka.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ffo.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://xux.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzd.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://fbt.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://ljn.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://jlf.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rkg.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qps.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://axx.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://ywj.andypj.xyz

[F06] 删除文件
来源：http://yap.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://lxx.xziqi.cn

PHP:  unlink("a.txt");
来源：http://reh.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://tfr.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://juf.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbf.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://bzr.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://hwj.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://fua.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://ddt.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kxv.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iky.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dpg.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awd.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ade.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zsx.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wxb.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cxe.cashguo.top

[F08] 遍历目录
来源：http://ppa.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qsw.svipenyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aeb.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://frv.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://guq.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxt.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vzw.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://jxb.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://bkx.jlsjyb.cn

[F09] 获取文件大小
来源：http://tlz.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://vmf.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://wqb.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://shr.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://qqd.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://dhb.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wtf.hnqzz.top

Ruby: File.size("a.txt")
来源：http://ond.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://mkq.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://nxt.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qqm.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ppb.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xbt.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://bbw.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pjd.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hhc.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tcu.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ldd.svipenyu.cn

[F11] 复制与移动文件
来源：http://kms.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://apz.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fxt.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tek.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exz.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mzj.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gif.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jwg.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wkl.shuidangran.top

[F12] CSV 读写
来源：http://yrn.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxf.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dxx.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rmm.jinyuanbaomall.cn

TS:   // 同上
来源：http://jxm.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hoo.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cgk.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lxs.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rsp.zhixingplan.top

================================================================================
来源：http://tvk.bbcook.cn

G. 面向对象
来源：http://ctb.zhongyouzk.top

================================================================================
来源：http://ckg.zdbjq.cn

[G01] 定义类
来源：http://ywx.zhaomingkeji.xyz

Py:   class User: pass
来源：http://fbr.tarul.cn

PHP:  class User {}
来源：http://dmn.hnxiangtu.top

JS:   class User {}
来源：http://brr.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://hbj.andypj.xyz

Java: class User {}
来源：http://oqw.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://rpp.yanxiufei.cn

Ruby: class User; end
来源：http://kmf.quarkkingdee.top

C#:   class User {}
来源：http://oyr.0kj1m.cn

[G02] 构造函数
来源：http://xru.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://boh.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://uce.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://pyz.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://ler.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://ipp.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://shj.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://wrf.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://arr.yvedp.cn

[G03] 实例属性
来源：http://mel.hfpthk.cn

Py:   self.name = "x"
来源：http://nqt.nwbrower.top

PHP:  public string $name = "x";
来源：http://spf.jyoumei.cn

JS:   this.name = "x";
来源：http://zdx.yanxiufei.cn

TS:   name: string = "x";
来源：http://wkz.0kj1m.cn

Java: private String name;
来源：http://odq.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uyl.tarul.cn

Ruby: @name = "x"
来源：http://uux.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://dyn.xylfe.cn

[G04] 定义方法
来源：http://ktv.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://jdd.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kqz.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://fyd.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://ytw.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://fjh.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://xll.xuanzx.com

Ruby: def greet; @name; end
来源：http://tfv.vehdjk.com

C#:   public string Greet() => Name;
来源：http://nyp.yj202588.top

[G05] 继承
来源：http://cjz.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://jlo.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://vxv.yueranfly.top

JS:   class Admin extends User {}
来源：http://nnx.meibo888.top

TS:   class Admin extends User {}
来源：http://zbn.c1oappe.top

Java: class Admin extends User {}
来源：http://pyl.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fqt.jianghu66.top

Ruby: class Admin < User; end
来源：http://mat.sysykeji.top

C#:   class Admin : User {}
来源：http://eye.chenjidiqi.icu

[G06] 重写方法
来源：http://yeh.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://vkh.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://amo.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://ksm.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://imv.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://wwc.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://afp.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://hkv.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://feu.xuanzx.com

[G07] 调用父类方法
来源：http://ctc.jqgfzy.top

Py:   super().greet()
来源：http://dlt.xuetiantiany.cn

PHP:  parent::greet();
来源：http://fyp.sysykeji.top

JS:   super.greet();
来源：http://szg.sweek.top

TS:   super.greet();
来源：http://fjc.ctjpmb.com

Java: super.greet();
来源：http://azu.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pvn.birdmap.top

Ruby: super
来源：http://icu.fehbvm.com

C#:   base.Greet();
来源：http://dmv.zhongyouzk.top

[G08] 静态方法与属性
来源：http://tkn.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wvs.redwolf501.top

PHP:  public static function f() {}
来源：http://xqy.jinqigufen.top

JS:   static f() {}
来源：http://oeg.gogol.net.cn

TS:   static f(): void {}
来源：http://cqx.mhx1999.top

Java: static void f() {}
来源：http://blz.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://itc.dianchejie.cn

Ruby: def self.f; end
来源：http://hcb.yfazqb.com

C#:   public static void F() {}
来源：http://rxj.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://ziu.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://kjo.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://kos.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://trz.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://hmn.sxryk.cn

Java: interface Shape { double area(); }
来源：http://taj.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://awh.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sno.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://glh.yj202588.top

[G10] 访问控制
来源：http://bsa.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://wxd.zhiwuduotai.top

PHP:  public / protected / private
来源：http://yfs.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://tcv.9152youxi.cn

TS:   public / protected / private
来源：http://biy.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://gnu.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wuj.vehdjk.com

Ruby: public / protected / private
来源：http://cwo.shuidangran.top

C#:   public / protected / private / internal
来源：http://sfu.ctjpmb.com

[G11] getter / setter
来源：http://png.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://eod.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mdk.316326.xyz


<!-- 参考信息 -->