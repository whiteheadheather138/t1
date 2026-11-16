代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vpn.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mig.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://fwu.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://fto.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://ifr.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://stp.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xbl.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wuf.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://kjc.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ixd.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xzr.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://gix.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://jyb.hesvh.cn

Java: String.format("%03d", 7)
来源：http://uli.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hsl.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bpd.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tmx.xinyue.icu

[E11] 反转字符串
来源：http://ped.zdbjq.cn

Py:   s[::-1]
来源：http://vxj.xuetiantiany.cn

PHP:  strrev($s);
来源：http://gnv.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://emw.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://fjo.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cmj.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oyq.havefunace.top

Ruby: s.reverse
来源：http://njn.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://ise.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://kee.ydzc1.top

Py:   s.count("a")
来源：http://aob.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://czn.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://ykh.52xcode.cn

TS:   s.split("a").length - 1
来源：http://qpp.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nul.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://clz.52xcode.cn

Ruby: s.count("a")
来源：http://qin.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://pma.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://gqn.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://zrl.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jel.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fin.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://knt.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hzh.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ulg.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://cbr.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pwj.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://apj.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kgl.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mye.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vue.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dpo.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lix.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oje.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ktb.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://npc.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://svi.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fss.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xwq.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rtv.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uqp.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbj.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bcc.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bmk.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xgq.vqdsnc.cn

[E16] 数字千分位
来源：http://tcf.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://vke.havefunace.top

PHP:  number_format(1234567);
来源：http://dxn.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://abc.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://sqw.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ofc.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eyw.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gaa.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://eum.nwbrower.top

[E17] 首字母大写
来源：http://kfr.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qsm.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rgc.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ylw.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gyw.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ohv.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vks.daria6918.cn

Ruby: s.capitalize
来源：http://fmr.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gzj.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://vnw.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mkq.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wax.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ltn.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fyk.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jub.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pyc.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qmx.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pfs.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://lrh.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://xuz.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dab.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://evd.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://lve.dashuyun.cn

Java: s.lines().toList()
来源：http://pgu.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://vvq.yj202588.top

Ruby: s.lines
来源：http://ouz.yfazqb.com

C#:   s.Split('\n')
来源：http://uua.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://kkr.fzhhl.top

Py:   if not s:
来源：http://gqj.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zky.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yra.wangdashe.top

TS:   if (s === "") {}
来源：http://iad.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://psq.yonumen.top

Go:   if s == "" {}
来源：http://qlg.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://mdx.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pnb.cqqwz.cn

[E21] 超长截断加省略号
来源：http://vnj.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ean.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sfo.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsa.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://myx.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lpb.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://vlv.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tib.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://btt.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://afa.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbt.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehf.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydm.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wic.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bpl.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ykd.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://arc.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xca.cdnleiting.top

================================================================================
来源：http://rvp.yj20258888.top

F. 文件与目录
来源：http://gps.dashuyun.cn

================================================================================
来源：http://bjy.cheryme.top

[F01] 读取整个文件
来源：http://xpq.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nrw.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://pdx.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mwr.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qbq.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://dmf.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pmp.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://ghp.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://xbz.havefunace.top

[F02] 逐行读取文件
来源：http://buf.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://diq.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ohh.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qnf.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qha.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://flc.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tem.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jfq.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vmp.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://ihs.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rrh.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uig.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bhs.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osv.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bpe.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgy.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://dlb.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://klo.tianlin.xyz

[F04] 追加写入文件
来源：http://ubm.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gzy.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oul.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ckv.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://otd.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://odx.xziqi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kfe.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://juj.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ywe.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://snn.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pxi.yj202588.top

PHP:  file_exists("a.txt");
来源：http://jtw.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://xga.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://irh.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://chs.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vpd.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://gtu.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://sgg.vqdsnc.cn

[F06] 删除文件
来源：http://mvq.yongpay.top

Py:   os.remove("a.txt")
来源：http://rvu.xinyue.icu

PHP:  unlink("a.txt");
来源：http://fcy.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ofo.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://flb.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kgo.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://ibz.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://aeu.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://usv.tian-w.cn

[F07] 创建目录（含多级）
来源：http://jnx.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tmn.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xaw.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lud.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bjy.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bkj.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cgt.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://phv.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rpf.tarul.cn

[F08] 遍历目录
来源：http://sjc.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://jhg.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://din.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://jze.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://uzc.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yxw.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://afb.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://ftr.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://bpr.316326.xyz

[F09] 获取文件大小
来源：http://qoo.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://pro.smart0.xyz

PHP:  filesize("a.txt");
来源：http://hfr.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://cns.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://btr.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://htq.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gnb.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://jsn.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://nyv.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://nmv.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdm.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zaw.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://izx.smart0.xyz

TS:   path.extname("a.txt")
来源：http://aaw.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://owy.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mml.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mfj.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kby.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://uig.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzd.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nyn.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmn.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pzu.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ymz.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yfg.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kja.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bdb.dianchejie.cn

[F12] CSV 读写
来源：http://xiv.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plt.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qkb.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dni.shanyushiyangtech.top

TS:   // 同上
来源：http://agh.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mkb.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aup.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iba.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fuo.ivvv.top

================================================================================
来源：http://squ.dashuyun.cn

G. 面向对象
来源：http://duy.yuanzhike.top

================================================================================
来源：http://ghs.yongpay.top

[G01] 定义类
来源：http://maa.hesvh.cn

Py:   class User: pass
来源：http://vyw.shanyushiyangkeji.top

PHP:  class User {}
来源：http://tsb.xziqi.cn

JS:   class User {}
来源：http://rud.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://woj.gzhubu.top

Java: class User {}
来源：http://qdu.dashuyun.cn

Go:   type User struct { Name string }
来源：http://mgo.pycfn.com

Ruby: class User; end
来源：http://rfp.pengpengdd.cyou

C#:   class User {}
来源：http://opu.hongshengwenyu.top

[G02] 构造函数
来源：http://svc.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://uuk.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://nng.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://lub.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://nbw.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://bxv.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dyc.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://xcp.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://apw.ydjk.org.cn

[G03] 实例属性
来源：http://uek.yongpay.top

Py:   self.name = "x"
来源：http://jqp.yonumen.top

PHP:  public string $name = "x";
来源：http://dkr.sjlbkw.cn

JS:   this.name = "x";
来源：http://rhz.gotoacloud.top

TS:   name: string = "x";
来源：http://mqv.zycfv.cn

Java: private String name;
来源：http://akg.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://acf.feifeiyinyue.top

Ruby: @name = "x"
来源：http://uin.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://cgl.yanxiufei.cn

[G04] 定义方法
来源：http://vxv.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://cmb.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vhv.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://srd.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://swk.quarkkingdee.top

Java: String greet() { return name; }
来源：http://hbi.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lyt.jyoumei.cn

Ruby: def greet; @name; end
来源：http://zmk.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://vuu.sxryk.cn

[G05] 继承
来源：http://icu.bjfxy.top

Py:   class Admin(User): pass
来源：http://bxe.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://vjy.yj20258888.top

JS:   class Admin extends User {}
来源：http://rlf.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://hqc.52xcode.cn

Java: class Admin extends User {}
来源：http://pbu.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bln.jinqigufen.top

Ruby: class Admin < User; end
来源：http://yuy.svipenyu.cn

C#:   class Admin : User {}
来源：http://bdn.jinghuilouyu.cn

[G06] 重写方法
来源：http://qsa.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://vzx.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://trf.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://imo.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://amd.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://ioz.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://snv.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://bhc.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://shp.xziqi.cn

[G07] 调用父类方法
来源：http://clk.zhijiandao.cn

Py:   super().greet()
来源：http://ygi.yj202588.top

PHP:  parent::greet();
来源：http://kep.xuanzx.com

JS:   super.greet();
来源：http://nwx.cashguo.top

TS:   super.greet();
来源：http://lhy.kuanghao11.cn

Java: super.greet();
来源：http://gfg.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tev.fengsongda.top


<!-- 参考信息 -->