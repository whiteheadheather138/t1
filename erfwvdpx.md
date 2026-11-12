代发 wailian999

JS:   [...s].reverse().join("")
来源：http://dpf.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://cmz.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://spl.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bff.hywenlv.cn

Ruby: s.reverse
来源：http://peq.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://ecj.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://pkz.epnwcf.com

Py:   s.count("a")
来源：http://mun.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://syi.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://ldh.tian-w.cn

TS:   s.split("a").length - 1
来源：http://kdt.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aon.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://mtm.bjfxy.top

Ruby: s.count("a")
来源：http://wxp.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://pws.havefunace.top

[E13] 逐字符遍历
来源：http://dmq.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://tfx.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eep.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://rfz.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lra.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zks.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipp.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cti.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jpk.nwbrower.top

[E14] URL 编码与 Base64
来源：http://pru.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qkt.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sqd.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pbb.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cfx.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cvx.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dqe.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fyh.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obh.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://khs.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://oro.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lwp.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cdq.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dhr.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hpn.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tpv.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://awj.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sef.birdmap.top

[E16] 数字千分位
来源：http://bcx.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://gex.hesvh.cn

PHP:  number_format(1234567);
来源：http://dxt.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://myx.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://lkz.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://daz.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hcm.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mjr.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://fht.chenjidiqi.icu

[E17] 首字母大写
来源：http://xid.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xql.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sii.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rbg.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qry.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mfv.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oir.ehwqpu.com

Ruby: s.capitalize
来源：http://num.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kyd.yueranfly.top

[E18] 模板占位符替换
来源：http://dxc.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ewz.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nsy.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jao.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://psm.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tag.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gpr.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qxg.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://shx.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://fkc.zdqjudy.top

Py:   s.splitlines()
来源：http://wfo.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lgw.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://ofg.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://oxc.yuxming.cn

Java: s.lines().toList()
来源：http://eov.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://wbo.zdqjudy.top

Ruby: s.lines
来源：http://rvn.yongpay.top

C#:   s.Split('\n')
来源：http://taz.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://nzv.zdbjq.cn

Py:   if not s:
来源：http://bdx.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghi.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yfg.ppjwa.cn

TS:   if (s === "") {}
来源：http://kou.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://vre.hnxiangtu.top

Go:   if s == "" {}
来源：http://bhw.dianchejie.cn

Ruby: if s.empty?
来源：http://aii.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qwd.chenlongwang.top

[E21] 超长截断加省略号
来源：http://upy.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zlm.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcd.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqs.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osd.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cjb.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://aiz.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yjq.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vlv.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://lnp.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eia.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://msn.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yak.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipe.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://noc.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xfz.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://ipq.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ngr.zdbjq.cn

================================================================================
来源：http://zzq.hysaishi.cn

F. 文件与目录
来源：http://iuq.xylfe.cn

================================================================================
来源：http://lrd.fehbvm.com

[F01] 读取整个文件
来源：http://fme.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gxv.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://pmc.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fta.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lta.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mwz.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gdy.cucudq.cn

Ruby: File.read("a.txt")
来源：http://dgc.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://dxk.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://jlm.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://djz.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://moc.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxc.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://itc.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pzr.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tcg.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://glm.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lch.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://tqx.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wgf.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://mym.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dfh.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lrx.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qvm.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yww.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://bgi.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ijn.uphjek.com

[F04] 追加写入文件
来源：http://khs.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wwd.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ntx.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ysj.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eaz.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uhf.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqg.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ruj.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oye.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://ubn.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dcj.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://sql.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://nvi.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://ppx.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lkx.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jly.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://tmx.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://shx.9152youxi.cn

[F06] 删除文件
来源：http://dto.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://zzq.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://hxe.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ptn.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://osh.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ehn.yj202588.top

Go:   os.Remove("a.txt")
来源：http://vio.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://sxz.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://cai.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://wtr.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ytc.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lkq.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wpl.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://goy.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dqi.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qag.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mzz.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mul.jinqigufen.top

[F08] 遍历目录
来源：http://qfk.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gkd.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pjv.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://sxh.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://vva.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dfo.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fkq.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://vnp.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://yjp.wangdashe.top

[F09] 获取文件大小
来源：http://nxh.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://ckf.bbcook.cn

PHP:  filesize("a.txt");
来源：http://sjm.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://uyq.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://ldi.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://vak.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fln.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://olr.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://dmb.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://tkk.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lls.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zeb.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bdy.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://wxq.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zwh.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://njk.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://njw.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gki.nanxinkj.top

[F11] 复制与移动文件
来源：http://ywg.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bhm.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbb.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gki.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnx.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ipr.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nty.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pef.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kmt.yueranfly.top

[F12] CSV 读写
来源：http://vzm.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bly.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yao.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xmm.zhiwuduotai.top

TS:   // 同上
来源：http://rcy.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mzv.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uhh.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yex.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ymh.jiagoushi.top

================================================================================
来源：http://rkh.hcnkem.com

G. 面向对象
来源：http://azu.tarul.cn

================================================================================
来源：http://pun.jinqigufen.top

[G01] 定义类
来源：http://lia.fanxiaobao.xyz

Py:   class User: pass
来源：http://xsb.cucudq.cn

PHP:  class User {}
来源：http://agr.vqdsnc.cn

JS:   class User {}
来源：http://mms.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://ddp.ehwqpu.com

Java: class User {}
来源：http://cbh.yuxming.cn

Go:   type User struct { Name string }
来源：http://zph.ybcxt.top

Ruby: class User; end
来源：http://gsc.ydzc1.top

C#:   class User {}
来源：http://zls.smart0.xyz

[G02] 构造函数
来源：http://xph.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://udm.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://flj.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://erj.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://wqv.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://vgp.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvb.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://xnh.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://iqq.jianghu66.top

[G03] 实例属性
来源：http://hue.cucudq.cn

Py:   self.name = "x"
来源：http://jnu.fehbvm.com

PHP:  public string $name = "x";
来源：http://qie.sjlbkw.cn

JS:   this.name = "x";
来源：http://lqb.daxiang520.top

TS:   name: string = "x";
来源：http://bex.cashguo.top

Java: private String name;
来源：http://thr.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://duj.zdbjq.cn

Ruby: @name = "x"
来源：http://wqj.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://jrb.ybcxt.top

[G04] 定义方法
来源：http://lsi.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://opp.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jxu.yonumen.top

JS:   greet() { return this.name; }
来源：http://ksx.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://vku.daria6918.cn

Java: String greet() { return name; }
来源：http://zat.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://bfy.xziqi.cn

Ruby: def greet; @name; end
来源：http://jhn.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://gkc.shanyushiyangkeji.top

[G05] 继承
来源：http://wvk.chenlongwang.top

Py:   class Admin(User): pass
来源：http://sbt.hammf.cn

PHP:  class Admin extends User {}
来源：http://xzn.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://xul.yj20258.top

TS:   class Admin extends User {}
来源：http://ayc.zhengqikj.top

Java: class Admin extends User {}
来源：http://nha.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://swx.yj202588.top

Ruby: class Admin < User; end
来源：http://blw.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://oak.ywan-chungtsiang.top

[G06] 重写方法
来源：http://bfh.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://imo.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://gop.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://tez.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://bbe.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://ifv.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wxa.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://iis.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://gkj.yonumen.top

[G07] 调用父类方法
来源：http://vci.haohaochexian.top

Py:   super().greet()
来源：http://azl.bjfxy.top

PHP:  parent::greet();
来源：http://tzg.yonumen.top

JS:   super.greet();
来源：http://phw.9152youxi.cn

TS:   super.greet();
来源：http://cls.hfpthk.cn

Java: super.greet();
来源：http://irk.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://teo.hnqzz.top

Ruby: super
来源：http://pns.yj20258.top

C#:   base.Greet();
来源：http://zye.zycfv.cn

[G08] 静态方法与属性
来源：http://hel.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bkz.yonumen.top

PHP:  public static function f() {}
来源：http://rzf.zhixingplan.top

JS:   static f() {}
来源：http://hxt.jinqigufen.top

TS:   static f(): void {}
来源：http://uun.yj20258888.top

Java: static void f() {}
来源：http://ggr.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nae.jyoumei.cn

Ruby: def self.f; end
来源：http://arm.yfazqb.com

C#:   public static void F() {}
来源：http://vyu.hesvh.cn

[G09] 接口 / 抽象类
来源：http://fio.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://ppg.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tjh.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jmd.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://bqh.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://pjf.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://llo.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sse.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://son.fehbvm.com


<!-- 参考信息 -->