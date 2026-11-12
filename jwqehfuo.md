代发 wailian999

Go:   strings.Count(s, "a")
来源：http://qri.gaohongyu789.top

Ruby: s.count("a")
来源：http://xpk.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://lhq.redwolf501.top

[E13] 逐字符遍历
来源：http://blw.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://nfr.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://toz.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jlk.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrn.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zyf.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pup.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ytc.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://afm.guannengcc.top

[E14] URL 编码与 Base64
来源：http://ngt.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zst.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wfh.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lbb.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xms.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oma.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jsx.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jus.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mfk.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://ckx.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wtg.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dip.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iye.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tat.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://amw.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nwv.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://edk.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ygi.xinyue.icu

[E16] 数字千分位
来源：http://rvf.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://zfy.gotoacloud.top

PHP:  number_format(1234567);
来源：http://bdn.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://smg.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qhw.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzd.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qek.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zjh.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://qia.yonumen.top

[E17] 首字母大写
来源：http://vcr.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xcr.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://heo.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dqk.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eoh.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cpv.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zcl.ctjpmb.com

Ruby: s.capitalize
来源：http://anf.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aez.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://xaf.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zfy.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lrp.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qws.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ecv.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tab.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abv.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fut.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pin.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://csq.shuidangran.top

Py:   s.splitlines()
来源：http://bpe.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zuo.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://mmz.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://ffe.yuxming.cn

Java: s.lines().toList()
来源：http://nao.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://rbt.wangshuangyany.cn

Ruby: s.lines
来源：http://iux.snrcjt.cn

C#:   s.Split('\n')
来源：http://qnv.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://eau.havefunace.top

Py:   if not s:
来源：http://vaw.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xne.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jrf.zhoulong.xyz

TS:   if (s === "") {}
来源：http://quv.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://trw.zhijiandao.cn

Go:   if s == "" {}
来源：http://wik.yuxming.cn

Ruby: if s.empty?
来源：http://amq.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wtn.shzxlz.cn

[E21] 超长截断加省略号
来源：http://aty.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nrj.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zjo.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udu.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nct.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jqy.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wjf.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rap.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vtg.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://fdu.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krg.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yru.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gdl.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cvp.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hew.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xnh.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://kld.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xys.0kj1m.cn

================================================================================
来源：http://tpm.gotoacloud.top

F. 文件与目录
来源：http://ljk.fengsongda.top

================================================================================
来源：http://gov.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://ddj.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vhn.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://gts.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nmc.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jge.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ugj.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mtg.hcnkem.com

Ruby: File.read("a.txt")
来源：http://nup.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://efm.sufxvd.cn

[F02] 逐行读取文件
来源：http://jwl.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xfr.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eem.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dri.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wov.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uqa.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hcf.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://byn.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wbs.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://bls.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kvp.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wbp.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqo.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqg.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://snc.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvm.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://efm.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mhb.0kj1m.cn

[F04] 追加写入文件
来源：http://trf.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cye.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hlr.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqp.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ows.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uck.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://beg.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jhh.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqc.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://cbw.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pdm.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://mrc.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://wsn.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://fas.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sov.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://are.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://hxn.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://fao.ydjk.org.cn

[F06] 删除文件
来源：http://qyp.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://bnb.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://rnq.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://rsm.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://bdg.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hpq.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://oeg.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://rfy.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://dyg.meibo888.top

[F07] 创建目录（含多级）
来源：http://oon.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ros.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bhl.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxy.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hkz.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bcj.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ngi.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://klm.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iln.jinqigfzy.top

[F08] 遍历目录
来源：http://kjt.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lya.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://poe.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://hbm.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://cce.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yhb.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aas.zdqjudy.top

Ruby: Dir.children("dir")
来源：http://qoh.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://ici.ydzc1.top

[F09] 获取文件大小
来源：http://fov.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://rss.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://ogl.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://trj.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://tsr.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://pzi.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nar.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://dkm.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://buy.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://fiq.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://brm.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jpc.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qcj.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://rjn.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wkh.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://piw.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ser.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pfr.hammf.cn

[F11] 复制与移动文件
来源：http://qgm.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzg.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ctt.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjh.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szx.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xjf.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ihc.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zkh.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hoi.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://voe.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ifw.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hft.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivy.zhixingplan.top

TS:   // 同上
来源：http://kcl.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ybd.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vsl.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bsw.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wka.zhijiandao.cn

================================================================================
来源：http://nho.redwolf501.top

G. 面向对象
来源：http://ejg.chenzaomai.com

================================================================================
来源：http://irl.bjfxy.top

[G01] 定义类
来源：http://afs.nanxuanxn.top

Py:   class User: pass
来源：http://nwo.shuidangran.top

PHP:  class User {}
来源：http://nmi.nanxinkj.top

JS:   class User {}
来源：http://twl.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://amj.jinqigufen.top

Java: class User {}
来源：http://ucl.chenzaomai.com

Go:   type User struct { Name string }
来源：http://oeb.bbcook.cn

Ruby: class User; end
来源：http://wdi.chenzaomai.com

C#:   class User {}
来源：http://nho.ydzc1.top

[G02] 构造函数
来源：http://stv.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://fyw.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://cue.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://obl.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://ldk.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://lcf.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fnh.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://pli.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://mqe.chenjidiqi.icu

[G03] 实例属性
来源：http://qfl.ppjwa.cn

Py:   self.name = "x"
来源：http://qgo.hammf.cn

PHP:  public string $name = "x";
来源：http://lnx.zhijiandao.cn

JS:   this.name = "x";
来源：http://poe.shuidangran.top

TS:   name: string = "x";
来源：http://fbe.gzhubu.top

Java: private String name;
来源：http://hlf.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lvu.hesvh.cn

Ruby: @name = "x"
来源：http://nqm.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://diy.shuidangran.top

[G04] 定义方法
来源：http://diq.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://nnm.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://azx.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://xek.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://tyl.gaohongyu789.top

Java: String greet() { return name; }
来源：http://fsh.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ccn.hysaishi.cn

Ruby: def greet; @name; end
来源：http://mvw.ydzc1.top

C#:   public string Greet() => Name;
来源：http://wtv.jqgfzy.top

[G05] 继承
来源：http://pvz.zdqjudy.top

Py:   class Admin(User): pass
来源：http://ekp.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://oyp.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://qrw.meibo888.top

TS:   class Admin extends User {}
来源：http://xjq.vehdjk.com

Java: class Admin extends User {}
来源：http://gzq.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pkh.iojbl.cn

Ruby: class Admin < User; end
来源：http://zin.fengsongda.top

C#:   class Admin : User {}
来源：http://vni.gaohongyu789.top

[G06] 重写方法
来源：http://ygn.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://upy.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bgy.yj202588.top

JS:   greet() { return "admin"; }
来源：http://ojw.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://kek.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://pfb.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jov.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://dbp.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://etx.vehdjk.com

[G07] 调用父类方法
来源：http://tmi.pycfn.com

Py:   super().greet()
来源：http://qqg.fktsv.cn

PHP:  parent::greet();
来源：http://mjj.xziqi.cn

JS:   super.greet();
来源：http://pjz.jinqigfzy.top

TS:   super.greet();
来源：http://hva.daria6918.cn

Java: super.greet();
来源：http://dpn.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ptd.xinyue.icu

Ruby: super
来源：http://kqk.xuetiantiany.cn

C#:   base.Greet();
来源：http://ozg.hesvh.cn

[G08] 静态方法与属性
来源：http://hwz.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tga.sjlbkw.cn

PHP:  public static function f() {}
来源：http://kkl.ctjpmb.com

JS:   static f() {}
来源：http://prx.ppjwa.cn

TS:   static f(): void {}
来源：http://imc.shanyushiyangtech.top

Java: static void f() {}
来源：http://ogt.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ilr.yuanzhike.top

Ruby: def self.f; end
来源：http://wqw.yuanzhike.top

C#:   public static void F() {}
来源：http://owf.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://dox.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://lhu.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hxf.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gwe.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://uzm.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://hov.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://zql.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hcy.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://dhj.jinghuilouyu.cn

[G10] 访问控制
来源：http://ddk.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://wlg.tianlin.xyz

PHP:  public / protected / private
来源：http://hdm.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://ihu.uphjek.com

TS:   public / protected / private
来源：http://rda.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://tjo.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://med.zhengqikj.top

Ruby: public / protected / private
来源：http://rru.ppjwa.cn

C#:   public / protected / private / internal
来源：http://vyv.sjlbkw.cn

[G11] getter / setter
来源：http://dkk.zycfv.cn

Py:   @property 与 @x.setter
来源：http://kyd.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pii.iojbl.cn


<!-- 参考信息 -->