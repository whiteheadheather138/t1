代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://wxd.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qar.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://okz.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fac.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://ewk.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ldt.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uwv.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://uyt.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://pyl.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://ahf.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tyu.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://htx.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kmq.tianlin.xyz

[E11] 反转字符串
来源：http://pyh.guowangkeji.top

Py:   s[::-1]
来源：http://bzt.jyoumei.cn

PHP:  strrev($s);
来源：http://gux.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://asg.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://tlb.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vkx.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iox.c1oappe.top

Ruby: s.reverse
来源：http://ewz.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fnp.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://lph.dianchejie.cn

Py:   s.count("a")
来源：http://xmu.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://twd.hcnkem.com

JS:   s.split("a").length - 1
来源：http://xpn.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://mis.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eon.cheryme.top

Go:   strings.Count(s, "a")
来源：http://qed.xuanzx.com

Ruby: s.count("a")
来源：http://opg.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://xgx.epnwcf.com

[E13] 逐字符遍历
来源：http://puc.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://wai.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tll.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://tmp.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nbu.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kzq.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kaa.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pnt.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eaa.tarul.cn

[E14] URL 编码与 Base64
来源：http://xvz.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lif.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nqa.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lls.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nqv.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tdw.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pua.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ncf.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xfo.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://oio.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nbn.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nal.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kla.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lwc.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://paq.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cri.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bnn.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dga.yj202588.top

[E16] 数字千分位
来源：http://lxd.316326.xyz

Py:   f"{1234567:,}"
来源：http://rjb.mhx1999.top

PHP:  number_format(1234567);
来源：http://ftp.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ubn.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lqz.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://csl.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://osj.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zvm.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://zaa.sjlbkw.cn

[E17] 首字母大写
来源：http://ukw.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yit.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cqb.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qeb.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://olg.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dky.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://igl.gotoacloud.top

Ruby: s.capitalize
来源：http://dsg.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ltf.havefunace.top

[E18] 模板占位符替换
来源：http://rsr.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jvk.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://arh.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lbw.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wuz.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gom.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sop.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dgx.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://soa.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://isc.bjfxy.top

Py:   s.splitlines()
来源：http://tva.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lev.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://nqi.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://dmt.aibaodan.cn

Java: s.lines().toList()
来源：http://tpz.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://iby.zhiwuduotai.top

Ruby: s.lines
来源：http://prz.pycfn.com

C#:   s.Split('\n')
来源：http://tic.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://spr.ppjwa.cn

Py:   if not s:
来源：http://eky.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ubm.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pil.hammf.cn

TS:   if (s === "") {}
来源：http://ejl.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://gyw.xinyue.icu

Go:   if s == "" {}
来源：http://jwn.9152youxi.cn

Ruby: if s.empty?
来源：http://zvq.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fdv.chenlongwang.top

[E21] 超长截断加省略号
来源：http://kvn.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zio.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://naa.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owq.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsk.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ous.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://hel.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ktd.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ail.yfazqb.com

[E22] 字节长度与字符长度
来源：http://eqx.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qfx.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cad.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsi.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lcv.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nqk.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cuw.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://ylm.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ciq.jlsjyb.cn

================================================================================
来源：http://wzj.gotoacloud.top

F. 文件与目录
来源：http://yfi.316326.xyz

================================================================================
来源：http://hao.fengsongda.top

[F01] 读取整个文件
来源：http://wpt.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ysx.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://kpf.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xjn.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zgu.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lbj.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vvr.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://zxj.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://dag.yuanzhike.top

[F02] 逐行读取文件
来源：http://gfn.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmx.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tkn.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cil.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfx.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://noz.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oey.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://quz.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lpl.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://yxk.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fsg.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://shw.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nbg.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdz.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://awn.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvv.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://ddj.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dle.andypj.xyz

[F04] 追加写入文件
来源：http://gxm.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vqk.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://czy.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjx.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imv.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mjx.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hop.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gdo.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vvi.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://udm.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kvp.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://rkn.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://avv.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://bfw.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gxv.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ism.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://ats.316326.xyz

C#:   File.Exists("a.txt")
来源：http://hoc.mhx1999.top

[F06] 删除文件
来源：http://udb.316326.xyz

Py:   os.remove("a.txt")
来源：http://wvd.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://hid.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://rqy.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oxr.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rkx.havefunace.top

Go:   os.Remove("a.txt")
来源：http://bew.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://eir.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://cjx.yj202588.top

[F07] 创建目录（含多级）
来源：http://tvv.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ijy.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://alb.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://osx.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhi.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wau.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tte.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sun.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nmq.redwolf501.top

[F08] 遍历目录
来源：http://zsj.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ogj.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://shi.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://pib.nanxuanxn.top

TS:   fs.readdirSync("dir")
来源：http://fuz.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdq.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bzv.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://wqj.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://zcu.daxiang520.top

[F09] 获取文件大小
来源：http://cga.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://jgt.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://kce.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://pwr.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://llc.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://zpn.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iik.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://hzn.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://kct.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://ywg.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hlq.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gpa.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jfu.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://mmw.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nty.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yiq.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tzo.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iij.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://cqz.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yku.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aqz.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twq.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bqb.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qcj.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://upn.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zsm.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://axk.shzxlz.cn

[F12] CSV 读写
来源：http://mix.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://msn.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ndz.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ell.fzhhl.top

TS:   // 同上
来源：http://zwp.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kum.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://arb.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lpl.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://epq.ydjk.org.cn

================================================================================
来源：http://xxp.0kj1m.cn

G. 面向对象
来源：http://sve.hnxiangtu.top

================================================================================
来源：http://qtn.iojbl.cn

[G01] 定义类
来源：http://kjo.sysykeji.top

Py:   class User: pass
来源：http://ifd.jqgfzy.top

PHP:  class User {}
来源：http://xmn.ybcxt.top

JS:   class User {}
来源：http://tvt.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://cgi.pengpengdd.cyou

Java: class User {}
来源：http://dmh.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://typ.zhijiandao.cn

Ruby: class User; end
来源：http://zit.chenjidiqi.icu

C#:   class User {}
来源：http://ipj.xylfe.cn

[G02] 构造函数
来源：http://ahm.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://zfr.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://val.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://tgg.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://xku.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://aat.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ztp.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://tod.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://trm.hcnkem.com

[G03] 实例属性
来源：http://knb.aibaodan.cn

Py:   self.name = "x"
来源：http://wvh.chenlongwang.top

PHP:  public string $name = "x";
来源：http://xzy.zdqjudy.top

JS:   this.name = "x";
来源：http://nus.sweek.top

TS:   name: string = "x";
来源：http://ezv.jiagoushi.top

Java: private String name;
来源：http://uce.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lqz.ehwqpu.com

Ruby: @name = "x"
来源：http://lsc.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://ojk.nwbrower.top

[G04] 定义方法
来源：http://von.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://kpi.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eiz.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://uqi.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://hex.jinqigfzy.top

Java: String greet() { return name; }
来源：http://cpt.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mrv.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://ryn.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://xla.redwolf501.top

[G05] 继承
来源：http://ngw.bbcook.cn

Py:   class Admin(User): pass
来源：http://mlc.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://whs.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://tci.gotoacloud.top

TS:   class Admin extends User {}
来源：http://amv.snrcjt.cn

Java: class Admin extends User {}
来源：http://fcj.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://heo.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://gdz.cdnleiting.top

C#:   class Admin : User {}
来源：http://owt.wangshuangyany.cn

[G06] 重写方法
来源：http://pkf.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://hmo.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://cjp.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://gch.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://wgp.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://hqv.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oqn.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://imi.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://fxu.snrcjt.cn

[G07] 调用父类方法
来源：http://eft.sysykeji.top

Py:   super().greet()
来源：http://aiq.xuanzx.com

PHP:  parent::greet();
来源：http://tfk.ctjpmb.com

JS:   super.greet();
来源：http://sem.mhx1999.top

TS:   super.greet();
来源：http://qvk.tianlin.xyz

Java: super.greet();
来源：http://hil.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ktz.sysykeji.top

Ruby: super
来源：http://cjj.hesvh.cn

C#:   base.Greet();
来源：http://qxh.xziqi.cn

[G08] 静态方法与属性
来源：http://pam.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dzl.jqgfzy.top


<!-- 参考信息 -->