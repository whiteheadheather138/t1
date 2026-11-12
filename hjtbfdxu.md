代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wcp.yongpay.top

[E11] 反转字符串
来源：http://kvx.jiagoushi.top

Py:   s[::-1]
来源：http://rmm.cashguo.top

PHP:  strrev($s);
来源：http://qos.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://tof.tarul.cn

TS:   [...s].reverse().join("")
来源：http://zxn.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xze.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://krt.hammf.cn

Ruby: s.reverse
来源：http://yex.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aug.hnqzz.top

[E12] 统计某字符出现次数
来源：http://gan.meibo888.top

Py:   s.count("a")
来源：http://exz.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://isv.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://abb.pycfn.com

TS:   s.split("a").length - 1
来源：http://xnk.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iho.havefunace.top

Go:   strings.Count(s, "a")
来源：http://vok.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://vxr.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://wal.yj20258.top

[E13] 逐字符遍历
来源：http://rec.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://qys.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dpn.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jzj.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lgj.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uoq.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sxx.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ram.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bym.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://cyj.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ref.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yvu.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uue.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xxz.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzc.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xfo.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qdt.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lsp.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://bzu.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xfw.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rjp.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://esy.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tyy.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cvi.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vhj.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zku.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://voa.pycfn.com

[E16] 数字千分位
来源：http://ygd.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://ojz.hcnkem.com

PHP:  number_format(1234567);
来源：http://wpf.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ihd.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vut.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://idj.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qjd.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjw.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://ygz.xziqi.cn

[E17] 首字母大写
来源：http://gjm.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ppe.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dyi.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xsw.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnj.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ckl.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bco.yuanzhike.top

Ruby: s.capitalize
来源：http://pzx.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gmv.tianlin.xyz

[E18] 模板占位符替换
来源：http://uuz.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yrv.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pnc.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wnf.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sbu.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzx.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aen.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cnp.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uze.daria6918.cn

[E19] 多行文本按行拆分
来源：http://fci.xinyue.icu

Py:   s.splitlines()
来源：http://ztp.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rwc.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://knh.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://hgd.svipenyu.cn

Java: s.lines().toList()
来源：http://yir.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://tot.yongpay.top

Ruby: s.lines
来源：http://rod.jinqigfzy.top

C#:   s.Split('\n')
来源：http://yft.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://yif.xinyue.icu

Py:   if not s:
来源：http://fov.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sms.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mgr.fzhhl.top

TS:   if (s === "") {}
来源：http://uwc.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://jzr.vehdjk.com

Go:   if s == "" {}
来源：http://jcc.cucudq.cn

Ruby: if s.empty?
来源：http://gdg.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gtp.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://roy.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eud.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvj.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pby.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebt.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mmz.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://wvp.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cqo.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gky.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://nim.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ooz.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcu.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oys.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://psi.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pur.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bni.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://mlj.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dii.nanxuanxn.top

================================================================================
来源：http://sah.bjfxy.top

F. 文件与目录
来源：http://har.316326.xyz

================================================================================
来源：http://esb.hesvh.cn

[F01] 读取整个文件
来源：http://izu.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gnd.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://iet.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ldr.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kfj.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tfi.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ckg.xinyue.icu

Ruby: File.read("a.txt")
来源：http://crm.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://mut.smart0.xyz

[F02] 逐行读取文件
来源：http://ggj.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jwa.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://txh.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skp.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bri.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kjn.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knk.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zro.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hgf.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://til.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oxo.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://uiw.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jpn.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qeg.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cor.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sni.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://xzg.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dmv.kuanghao11.cn

[F04] 追加写入文件
来源：http://lpi.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uul.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jor.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hua.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxb.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rdx.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yqs.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cpg.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aog.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://hak.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzz.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://jrh.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://lld.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://mjl.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hjz.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bie.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://hga.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://ulm.jlsjyb.cn

[F06] 删除文件
来源：http://viy.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://idi.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://jjb.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://elz.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://oho.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cmn.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://get.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://ghw.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://cpv.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://voy.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eyw.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lcw.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bst.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://etf.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eqg.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sje.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kia.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kat.wangdashe.top

[F08] 遍历目录
来源：http://ozn.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ftp.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bvu.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://pvn.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://xag.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fkf.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://afo.guannengcc.top

Ruby: Dir.children("dir")
来源：http://oqz.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://rty.hcnkem.com

[F09] 获取文件大小
来源：http://aqd.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://hhw.xinyue.icu

PHP:  filesize("a.txt");
来源：http://otz.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://fbz.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://pth.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://oqm.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wec.wangdashe.top

Ruby: File.size("a.txt")
来源：http://pme.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://cgq.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://eab.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iiv.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kyv.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qns.shuidangran.top

TS:   path.extname("a.txt")
来源：http://itn.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gcw.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hrc.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xuq.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gzg.birdmap.top

[F11] 复制与移动文件
来源：http://owf.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bzy.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iso.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://txh.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayq.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ofa.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vnl.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yuc.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tep.jinqigufen.top

[F12] CSV 读写
来源：http://wdq.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nru.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lsu.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aqg.hywenlv.cn

TS:   // 同上
来源：http://mxw.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ozf.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nug.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bww.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lzz.daria6918.cn

================================================================================
来源：http://kjq.snrcjt.cn

G. 面向对象
来源：http://tra.ydjk.org.cn

================================================================================
来源：http://dvm.fanxiaobao.xyz

[G01] 定义类
来源：http://luf.jyoumei.cn

Py:   class User: pass
来源：http://wmo.yj202588.top

PHP:  class User {}
来源：http://esc.tanke756.top

JS:   class User {}
来源：http://khf.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://kac.jiagoushi.top

Java: class User {}
来源：http://tgv.xylfe.cn

Go:   type User struct { Name string }
来源：http://kqi.dianchejie.cn

Ruby: class User; end
来源：http://hhb.zdqjudy.top

C#:   class User {}
来源：http://rqa.hcnkem.com

[G02] 构造函数
来源：http://zma.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://yee.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://twf.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://zvi.yj202588.top

TS:   constructor(public name: string) {}
来源：http://hzo.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://cxn.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mrv.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://opa.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://uww.jqgufenzy.top

[G03] 实例属性
来源：http://wya.ydjk.org.cn

Py:   self.name = "x"
来源：http://cll.chenlongwang.top

PHP:  public string $name = "x";
来源：http://xjo.xuetiantiany.cn

JS:   this.name = "x";
来源：http://pxg.iojbl.cn

TS:   name: string = "x";
来源：http://rps.zdbjq.cn

Java: private String name;
来源：http://qif.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bry.c1oappe.top

Ruby: @name = "x"
来源：http://ejk.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://tir.fehbvm.com

[G04] 定义方法
来源：http://kdc.havefunace.top

Py:   def greet(self): return self.name
来源：http://pei.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mxt.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ccl.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://pat.nwbrower.top

Java: String greet() { return name; }
来源：http://fql.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eqw.hysaishi.cn

Ruby: def greet; @name; end
来源：http://zaa.fzhhl.top

C#:   public string Greet() => Name;
来源：http://mcz.jinqigfzy.top

[G05] 继承
来源：http://hex.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://wpp.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://npv.dianchejie.cn

JS:   class Admin extends User {}
来源：http://omg.yueranfly.top

TS:   class Admin extends User {}
来源：http://szb.kuanghao11.cn

Java: class Admin extends User {}
来源：http://mcl.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pxb.xuanzx.com

Ruby: class Admin < User; end
来源：http://qel.smart0.xyz

C#:   class Admin : User {}
来源：http://wlw.guowangkeji.top

[G06] 重写方法
来源：http://ple.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://vbl.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wbb.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://gpa.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://uxf.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://tkw.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pkp.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://hfp.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://nvo.pengpengdd.cyou

[G07] 调用父类方法
来源：http://zsp.fehbvm.com

Py:   super().greet()
来源：http://bab.chenjidiqi.icu

PHP:  parent::greet();
来源：http://yeg.nanxuanxn.top

JS:   super.greet();
来源：http://qlj.tanke756.top

TS:   super.greet();
来源：http://ojo.yuanzhike.top

Java: super.greet();
来源：http://jbk.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://prh.snrcjt.cn

Ruby: super
来源：http://clt.shuidangran.top

C#:   base.Greet();
来源：http://obm.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://zgm.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fst.fzhhl.top

PHP:  public static function f() {}
来源：http://ljh.zhengqikj.top

JS:   static f() {}
来源：http://sji.hongshengwenyu.top

TS:   static f(): void {}
来源：http://hyv.c1oappe.top

Java: static void f() {}
来源：http://qfv.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://cdd.jinqigufen.top

Ruby: def self.f; end
来源：http://xac.hnxiangtu.top

C#:   public static void F() {}
来源：http://opk.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://bsl.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://nbz.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aqe.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://gxq.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://cqa.zhoulong.xyz


<!-- 参考信息 -->