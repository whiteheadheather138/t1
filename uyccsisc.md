代发 wailian999

Py:   for ch in s: print(ch)
来源：http://rgp.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cpe.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxa.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vkd.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://idp.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fjm.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gdo.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cxw.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://lla.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ebx.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://caq.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dym.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ous.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fqw.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hiq.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jgd.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://irn.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://dme.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gor.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kpx.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uap.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rae.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzl.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nsf.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://col.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bit.havefunace.top

[E16] 数字千分位
来源：http://mkt.c1oappe.top

Py:   f"{1234567:,}"
来源：http://mmx.yj202588.top

PHP:  number_format(1234567);
来源：http://obk.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gkg.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfu.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://syv.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsu.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xge.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://wda.shangyingyoupin.top

[E17] 首字母大写
来源：http://qgq.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tks.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ckk.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zpo.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hpl.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tmo.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xvk.jinqigufen.top

Ruby: s.capitalize
来源：http://jsm.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hqz.aizwys.cn

[E18] 模板占位符替换
来源：http://ioq.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xmw.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oxc.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://csp.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sng.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qzp.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hlu.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qrp.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ozk.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://cxr.aizwys.cn

Py:   s.splitlines()
来源：http://vie.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fww.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://div.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://nmj.yanxiufei.cn

Java: s.lines().toList()
来源：http://jsd.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://bpu.316326.xyz

Ruby: s.lines
来源：http://gfw.sjlbkw.cn

C#:   s.Split('\n')
来源：http://bjr.yj202588.top

[E20] 判断字符串是否为空
来源：http://xfd.yuanzhike.top

Py:   if not s:
来源：http://wwq.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wae.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oqh.chenzaomai.com

TS:   if (s === "") {}
来源：http://nic.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://prg.chenjidiqi.icu

Go:   if s == "" {}
来源：http://rch.feifeiyinyue.top

Ruby: if s.empty?
来源：http://yjf.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ylh.xuanzx.com

[E21] 超长截断加省略号
来源：http://eeq.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ezs.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ayq.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzi.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezl.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fvq.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://mlm.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://srn.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iol.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://ylj.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqe.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxe.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zzs.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfx.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyy.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ewn.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://aun.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hus.havefunace.top

================================================================================
来源：http://zeb.wangdashe.top

F. 文件与目录
来源：http://cgh.guannengcc.top

================================================================================
来源：http://rst.kuanghao11.cn

[F01] 读取整个文件
来源：http://hxz.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bdc.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://geb.xziqi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://guc.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nuv.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iyc.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://twj.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://igk.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://woa.hcnkem.com

[F02] 逐行读取文件
来源：http://kdf.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jxc.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rwc.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqj.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uak.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gsn.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mky.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://flt.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mki.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://wvl.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uys.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://utx.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://boq.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gro.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qsz.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jeq.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://qqd.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vtw.dianchejie.cn

[F04] 追加写入文件
来源：http://zgf.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eqr.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pjz.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hca.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwz.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mau.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qxx.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yik.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ufb.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://jhg.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fyu.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://oem.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://hkk.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://kuj.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uln.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pvl.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://sqx.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://otn.cheryme.top

[F06] 删除文件
来源：http://xrr.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://kyv.xylfe.cn

PHP:  unlink("a.txt");
来源：http://nya.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wcb.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dpk.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cwl.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://aos.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://ouo.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://znd.andypj.xyz

[F07] 创建目录（含多级）
来源：http://zua.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zef.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gss.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tsf.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wkr.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mig.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jee.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sfh.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hxb.gotoacloud.top

[F08] 遍历目录
来源：http://ued.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vvx.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qrq.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://wwe.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://xlp.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zkh.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nws.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://gfo.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://qkr.vqdsnc.cn

[F09] 获取文件大小
来源：http://kmh.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://ssu.wangdashe.top

PHP:  filesize("a.txt");
来源：http://vrq.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://xhk.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://drp.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://npg.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rzw.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://ncj.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://gsx.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://cfw.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fvu.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wjh.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tmh.hcnkem.com

TS:   path.extname("a.txt")
来源：http://mdf.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ftq.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fie.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jxx.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fij.meibo888.top

[F11] 复制与移动文件
来源：http://mxm.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://htr.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ykb.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qey.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vyt.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://von.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ytb.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pjz.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cow.ppjwa.cn

[F12] CSV 读写
来源：http://sqx.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oxt.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ceo.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dgq.zdqjudy.top

TS:   // 同上
来源：http://hyy.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pgt.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wod.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ype.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vwk.ctjpmb.com

================================================================================
来源：http://btb.jiagoushi.top

G. 面向对象
来源：http://ojg.hywenlv.cn

================================================================================
来源：http://yox.meibo888.top

[G01] 定义类
来源：http://ter.xziqi.cn

Py:   class User: pass
来源：http://vqs.yvedp.cn

PHP:  class User {}
来源：http://kry.wangshuangyany.cn

JS:   class User {}
来源：http://mkz.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://axi.sufxvd.cn

Java: class User {}
来源：http://noc.pycfn.com

Go:   type User struct { Name string }
来源：http://gge.wangshuangyany.cn

Ruby: class User; end
来源：http://cqi.jianghu66.top

C#:   class User {}
来源：http://cxv.jyoumei.cn

[G02] 构造函数
来源：http://wtm.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://eup.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://tkh.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://pqm.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://yav.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://npg.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ijk.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://qrx.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://efq.snrcjt.cn

[G03] 实例属性
来源：http://mqs.tarul.cn

Py:   self.name = "x"
来源：http://lrz.snrcjt.cn

PHP:  public string $name = "x";
来源：http://utj.dashuyun.cn

JS:   this.name = "x";
来源：http://qgi.ppjwa.cn

TS:   name: string = "x";
来源：http://ctg.yuanzhike.top

Java: private String name;
来源：http://pib.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://naj.zycfv.cn

Ruby: @name = "x"
来源：http://urs.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://hum.jianghu66.top

[G04] 定义方法
来源：http://tuy.uphjek.com

Py:   def greet(self): return self.name
来源：http://nqo.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hhp.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://yfg.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://hkq.jyoumei.cn

Java: String greet() { return name; }
来源：http://lei.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://joe.tarul.cn

Ruby: def greet; @name; end
来源：http://nbd.yueranfly.top

C#:   public string Greet() => Name;
来源：http://idr.hnxiangtu.top

[G05] 继承
来源：http://yvq.chenlongwang.top

Py:   class Admin(User): pass
来源：http://qps.vehdjk.com

PHP:  class Admin extends User {}
来源：http://jfp.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://jsg.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://pdh.zhoulong.xyz

Java: class Admin extends User {}
来源：http://wdk.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uzk.c1oappe.top

Ruby: class Admin < User; end
来源：http://zfi.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://ugw.cqqwz.cn

[G06] 重写方法
来源：http://hyk.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://blp.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xhd.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://qxw.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://ujn.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://zjl.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ezn.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://pbw.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://mti.cucudq.cn

[G07] 调用父类方法
来源：http://btg.smart0.xyz

Py:   super().greet()
来源：http://iko.zhijiandao.cn

PHP:  parent::greet();
来源：http://bqw.jianghu66.top

JS:   super.greet();
来源：http://lfj.yj20258.top

TS:   super.greet();
来源：http://vhq.cashguo.top

Java: super.greet();
来源：http://ryt.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jyt.zdqjudy.top

Ruby: super
来源：http://wsp.yuxming.cn

C#:   base.Greet();
来源：http://tff.9152youxi.cn

[G08] 静态方法与属性
来源：http://elz.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rsa.cdnleiting.top

PHP:  public static function f() {}
来源：http://foa.nanxuanxn.top

JS:   static f() {}
来源：http://eoa.yueranfly.top

TS:   static f(): void {}
来源：http://nft.wangshuangyany.cn

Java: static void f() {}
来源：http://fue.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://afv.chenzaomai.com

Ruby: def self.f; end
来源：http://vub.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://aqf.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://xbl.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://sxi.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://jql.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxg.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://vee.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://sbn.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://bmq.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fzo.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://isg.havefunace.top

[G10] 访问控制
来源：http://pbd.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://ikt.tianlin.xyz

PHP:  public / protected / private
来源：http://vto.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://hmm.chenzaomai.com

TS:   public / protected / private
来源：http://blg.uphjek.com

Java: public / protected / private / 默认包级
来源：http://epq.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://nql.jqgufenzy.top

Ruby: public / protected / private
来源：http://ysh.cdnleiting.top

C#:   public / protected / private / internal
来源：http://geu.pycfn.com

[G11] getter / setter
来源：http://mrq.cashguo.top

Py:   @property 与 @x.setter
来源：http://fmu.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://peh.guannengcc.top

JS:   get name() { return this._name; }
来源：http://wda.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://rdz.yangfankeji.com

Java: public String getName() { return name; }
来源：http://ddd.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://efu.nwbrower.top


<!-- 参考信息 -->