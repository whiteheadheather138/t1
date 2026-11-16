代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://zjy.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sjb.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://siq.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://xgh.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://nns.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://jva.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xwj.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kbs.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qxu.jinghuilouyu.cn

[E11] 反转字符串
来源：http://syy.wangshuangyany.cn

Py:   s[::-1]
来源：http://yjf.xuetiantiany.cn

PHP:  strrev($s);
来源：http://hpx.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://pge.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://fkf.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://kuf.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://hmk.guowangkeji.top

Ruby: s.reverse
来源：http://fre.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://ydh.aizwys.cn

[E12] 统计某字符出现次数
来源：http://cmn.tianlin.xyz

Py:   s.count("a")
来源：http://rab.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://aqx.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://mei.yuxming.cn

TS:   s.split("a").length - 1
来源：http://ygx.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://thm.hammf.cn

Go:   strings.Count(s, "a")
来源：http://yxh.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://eum.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://dvc.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://ewy.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://qlk.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rxa.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://syd.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ujj.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zph.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lpg.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tot.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://duy.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://fot.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yvk.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://kyi.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kgc.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dym.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eob.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gxe.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wxw.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jfs.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://foj.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rto.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zhe.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uvv.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yhl.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dxm.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jwe.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kjk.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mxd.havefunace.top

[E16] 数字千分位
来源：http://arb.zycfv.cn

Py:   f"{1234567:,}"
来源：http://imj.yangfankeji.com

PHP:  number_format(1234567);
来源：http://xjn.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sbd.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qdj.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gez.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayl.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pdm.birdmap.top

C#:   1234567.ToString("N0")
来源：http://jwe.nanxinkj.top

[E17] 首字母大写
来源：http://ixo.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wlv.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://irc.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkp.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxl.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ynb.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ici.hongshengwenyu.top

Ruby: s.capitalize
来源：http://fbj.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lzw.hfpthk.cn

[E18] 模板占位符替换
来源：http://guh.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pqi.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gsw.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://etw.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tco.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ity.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mde.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fvp.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://esu.xziqi.cn

[E19] 多行文本按行拆分
来源：http://eth.yuxming.cn

Py:   s.splitlines()
来源：http://wjq.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vto.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://sfj.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://wqw.zycfv.cn

Java: s.lines().toList()
来源：http://wib.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://mvn.nanxinkj.top

Ruby: s.lines
来源：http://jlf.cheryme.top

C#:   s.Split('\n')
来源：http://jnl.yfazqb.com

[E20] 判断字符串是否为空
来源：http://bvc.jiagoushi.top

Py:   if not s:
来源：http://zqu.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mnw.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ixc.jqgfzy.top

TS:   if (s === "") {}
来源：http://yaf.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://ddd.fehbvm.com

Go:   if s == "" {}
来源：http://anu.jinqigufen.top

Ruby: if s.empty?
来源：http://fnm.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://stt.shzxlz.cn

[E21] 超长截断加省略号
来源：http://qhz.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://htd.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jki.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://suq.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lmk.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://syn.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://zhh.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sid.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yvl.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://rcu.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fdu.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://auj.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lkt.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tnw.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gtn.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pok.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://bvz.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oke.ywan-chungtsiang.top

================================================================================
来源：http://cae.yueranfly.top

F. 文件与目录
来源：http://phk.chenjidiqi.icu

================================================================================
来源：http://zcf.xylfe.cn

[F01] 读取整个文件
来源：http://riq.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://psv.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://lxp.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tpj.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zcx.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sde.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqv.bjfxy.top

Ruby: File.read("a.txt")
来源：http://kbi.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://srm.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://naj.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nna.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ljc.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://daw.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehh.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://brb.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://umr.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gpk.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ijg.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://wqg.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://caj.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jmh.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ikx.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ljz.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnj.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvm.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://okv.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://czs.tarul.cn

[F04] 追加写入文件
来源：http://nlv.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hhn.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dsq.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hsg.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyq.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tpd.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vra.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lpp.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fra.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://vys.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://puz.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://dsg.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://msn.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://fpz.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nyq.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sbh.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://tee.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://vsk.yfazqb.com

[F06] 删除文件
来源：http://ehh.xinyue.icu

Py:   os.remove("a.txt")
来源：http://lob.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://ktg.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qva.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://blj.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vrz.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://oyj.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://jlo.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://yur.pycfn.com

[F07] 创建目录（含多级）
来源：http://ysw.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sbo.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eae.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qlm.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvm.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oes.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hgt.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dos.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aff.yuxming.cn

[F08] 遍历目录
来源：http://fjh.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nfc.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uvi.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://mvj.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://efp.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tfe.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://djc.yonumen.top

Ruby: Dir.children("dir")
来源：http://gji.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://nut.sjlbkw.cn

[F09] 获取文件大小
来源：http://llt.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://fli.hcnkem.com

PHP:  filesize("a.txt");
来源：http://sbv.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://dge.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://sda.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://wek.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ksp.iojbl.cn

Ruby: File.size("a.txt")
来源：http://dbk.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://vrj.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://lqh.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ynu.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vmz.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hqh.ybcxt.top

TS:   path.extname("a.txt")
来源：http://oqd.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hin.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ils.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://knx.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hyi.jqgfzy.top

[F11] 复制与移动文件
来源：http://kho.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qjq.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hal.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://unw.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vwa.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ooz.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sbt.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qhw.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nkc.tian-w.cn

[F12] CSV 读写
来源：http://ijy.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vza.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kkv.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hhr.redwolf501.top

TS:   // 同上
来源：http://tiq.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cjv.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://czc.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fmo.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pdc.zhongyouzk.top

================================================================================
来源：http://skr.c1oappe.top

G. 面向对象
来源：http://ure.zhiwuduotai.top

================================================================================
来源：http://oua.yonumen.top

[G01] 定义类
来源：http://die.ybcxt.top

Py:   class User: pass
来源：http://faf.hcnkem.com

PHP:  class User {}
来源：http://ste.hnqzz.top

JS:   class User {}
来源：http://kzt.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://hro.andypj.xyz

Java: class User {}
来源：http://sti.hysaishi.cn

Go:   type User struct { Name string }
来源：http://nia.sxryk.cn

Ruby: class User; end
来源：http://wqg.jinqigfzy.top

C#:   class User {}
来源：http://gjd.jqgfzy.top

[G02] 构造函数
来源：http://mzv.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://tec.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://cld.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://jco.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://zdw.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://pkd.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ckl.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ftg.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://ett.daxiang520.top

[G03] 实例属性
来源：http://dtk.cucudq.cn

Py:   self.name = "x"
来源：http://hra.gzhubu.top

PHP:  public string $name = "x";
来源：http://vuk.zycfv.cn

JS:   this.name = "x";
来源：http://eiv.hammf.cn

TS:   name: string = "x";
来源：http://oik.uphjek.com

Java: private String name;
来源：http://ave.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xlm.zycfv.cn

Ruby: @name = "x"
来源：http://zof.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lqq.svipenyu.cn

[G04] 定义方法
来源：http://xpg.guannengcc.top

Py:   def greet(self): return self.name
来源：http://pov.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://quk.fengsongda.top

JS:   greet() { return this.name; }
来源：http://udu.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://nkk.jiagoushi.top

Java: String greet() { return name; }
来源：http://htk.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iff.ehwqpu.com

Ruby: def greet; @name; end
来源：http://jpd.fengsongda.top

C#:   public string Greet() => Name;
来源：http://pwd.fanxiaobao.xyz

[G05] 继承
来源：http://xqw.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://iyj.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://jmr.shzxlz.cn

JS:   class Admin extends User {}
来源：http://djf.ivvv.top

TS:   class Admin extends User {}
来源：http://ivc.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://qjo.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cyz.guannengcc.top

Ruby: class Admin < User; end
来源：http://htf.zhoulong.xyz

C#:   class Admin : User {}
来源：http://sak.chenzaomai.com

[G06] 重写方法
来源：http://boe.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://ruv.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kxd.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://ysi.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://rmt.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://unz.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wxk.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://tdb.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://nbx.yueranfly.top

[G07] 调用父类方法
来源：http://mcw.gogol.net.cn

Py:   super().greet()
来源：http://nzo.xinyue.icu

PHP:  parent::greet();
来源：http://ojo.fehbvm.com

JS:   super.greet();
来源：http://sam.ehwqpu.com

TS:   super.greet();
来源：http://ran.ivvv.top

Java: super.greet();
来源：http://zuy.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qgr.52xcode.cn

Ruby: super
来源：http://pgd.cqqwz.cn

C#:   base.Greet();
来源：http://hto.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://anw.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pfi.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://wil.pycfn.com

JS:   static f() {}
来源：http://ymo.xziqi.cn

TS:   static f(): void {}
来源：http://pey.ctjpmb.com

Java: static void f() {}
来源：http://ums.shuidangran.top


<!-- 参考信息 -->