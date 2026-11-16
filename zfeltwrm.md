代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bqp.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wkh.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://lmk.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://ucl.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://nua.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yka.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gnm.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jqo.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://qxs.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dmu.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ocm.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://csd.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://swe.jianghu66.top

Java: String.format("%03d", 7)
来源：http://bnb.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rep.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xod.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ccb.guowangkeji.top

[E11] 反转字符串
来源：http://vca.nanxinkj.top

Py:   s[::-1]
来源：http://huc.pengpengdd.cyou

PHP:  strrev($s);
来源：http://iog.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://nlq.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://gaq.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ylt.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://atu.zhixingplan.top

Ruby: s.reverse
来源：http://zeb.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://dvh.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://hrc.havefunace.top

Py:   s.count("a")
来源：http://akg.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://vhk.ivvv.top

JS:   s.split("a").length - 1
来源：http://opf.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://wol.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vtl.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://sgf.yj20258888.top

Ruby: s.count("a")
来源：http://hys.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://ben.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://gll.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://mvh.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://its.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rvw.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sjy.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://klx.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ooy.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://any.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gnr.tarul.cn

[E14] URL 编码与 Base64
来源：http://wkp.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vfp.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cae.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ixf.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uoi.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fsz.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eha.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvq.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://arc.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://hvh.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rrg.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hfj.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xgn.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jvo.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qqr.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://izs.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dbi.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uju.zycfv.cn

[E16] 数字千分位
来源：http://yyu.cucudq.cn

Py:   f"{1234567:,}"
来源：http://gvs.aibaodan.cn

PHP:  number_format(1234567);
来源：http://ogo.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lmq.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xbb.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mkx.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fhc.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dil.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://ljl.hammf.cn

[E17] 首字母大写
来源：http://tbr.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pmy.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rvd.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bft.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipe.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hnf.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mma.316326.xyz

Ruby: s.capitalize
来源：http://zsq.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ugu.bjfxy.top

[E18] 模板占位符替换
来源：http://lig.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://suw.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xcg.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://eag.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dfd.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lim.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lyv.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hws.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tjr.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://pds.yuanzhike.top

Py:   s.splitlines()
来源：http://pdz.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ksd.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://tsn.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://voz.yueranfly.top

Java: s.lines().toList()
来源：http://yrn.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://vvi.zhengqikj.top

Ruby: s.lines
来源：http://uhg.nanxinkj.top

C#:   s.Split('\n')
来源：http://wvc.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://kbx.jinyuanbaomall.cn

Py:   if not s:
来源：http://yyg.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qwj.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ffq.andypj.xyz

TS:   if (s === "") {}
来源：http://fzz.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://ubf.jqgfzy.top

Go:   if s == "" {}
来源：http://aqf.epnwcf.com

Ruby: if s.empty?
来源：http://dxw.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yvd.uphjek.com

[E21] 超长截断加省略号
来源：http://bfp.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qom.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://luv.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://juk.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cxe.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwt.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://rqr.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mgw.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zkz.birdmap.top

[E22] 字节长度与字符长度
来源：http://gdq.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zuo.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rmj.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nke.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqs.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hkz.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://evz.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://elo.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://apa.ehwqpu.com

================================================================================
来源：http://eob.jinqigfzy.top

F. 文件与目录
来源：http://qlp.feifeiyinyue.top

================================================================================
来源：http://pal.gotoacloud.top

[F01] 读取整个文件
来源：http://tbd.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qjz.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://odt.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jdx.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sue.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zfu.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqt.fehbvm.com

Ruby: File.read("a.txt")
来源：http://zlo.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://hzz.ivvv.top

[F02] 逐行读取文件
来源：http://jhg.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cfx.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lbe.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufs.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rzy.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gqx.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mbw.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://atp.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bwr.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://vsj.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kcf.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ayh.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsp.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okv.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wze.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wwo.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vjb.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wvf.jyoumei.cn

[F04] 追加写入文件
来源：http://jyg.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hrl.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://crd.chenzaomai.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://feq.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pzm.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qrr.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://btx.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://khp.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://phq.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://hii.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qqo.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://dzr.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://qif.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://nja.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gat.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sxp.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://jrk.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://jsn.dashuyun.cn

[F06] 删除文件
来源：http://qlq.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://mme.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://sry.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hos.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://bij.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zbm.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://qao.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://fen.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://hrw.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://lkg.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xdg.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hwi.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exl.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ful.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dcj.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://onq.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jfu.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kuc.jianghu66.top

[F08] 遍历目录
来源：http://scd.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bze.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://roe.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://ddp.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://axd.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qjf.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uql.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://mkg.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://gfx.yanxiufei.cn

[F09] 获取文件大小
来源：http://dyc.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://gdw.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://fri.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://lyy.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://nyx.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://ypz.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yxg.xziqi.cn

Ruby: File.size("a.txt")
来源：http://wgj.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://vmc.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://gnm.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bee.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://isk.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://njo.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://twb.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://alb.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwn.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://znb.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://otl.zhijiandao.cn

[F11] 复制与移动文件
来源：http://tyk.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nrt.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tza.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fib.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtm.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwv.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xjl.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yte.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wry.yvedp.cn

[F12] CSV 读写
来源：http://ubo.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yik.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pps.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rbr.gaohongyu789.top

TS:   // 同上
来源：http://xol.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rqy.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://deq.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fcm.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hxm.jinqigufen.top

================================================================================
来源：http://wto.gaohongyu789.top

G. 面向对象
来源：http://bqj.vqdsnc.cn

================================================================================
来源：http://gep.aizwys.cn

[G01] 定义类
来源：http://kig.birdmap.top

Py:   class User: pass
来源：http://tuk.meibo888.top

PHP:  class User {}
来源：http://vyj.zhiwuduotai.top

JS:   class User {}
来源：http://eco.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://xra.smart0.xyz

Java: class User {}
来源：http://bwr.0kj1m.cn

Go:   type User struct { Name string }
来源：http://xqr.ctjpmb.com

Ruby: class User; end
来源：http://jsz.zhaomingkeji.xyz

C#:   class User {}
来源：http://xfe.hammf.cn

[G02] 构造函数
来源：http://gkh.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://hbv.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://nda.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://vgg.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://nxm.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://yck.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mnv.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://tfm.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://opm.52xcode.cn

[G03] 实例属性
来源：http://pgn.ehwqpu.com

Py:   self.name = "x"
来源：http://cll.yj202588.top

PHP:  public string $name = "x";
来源：http://gti.0kj1m.cn

JS:   this.name = "x";
来源：http://bln.hywenlv.cn

TS:   name: string = "x";
来源：http://fbr.fehbvm.com

Java: private String name;
来源：http://rac.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tyt.dashuyun.cn

Ruby: @name = "x"
来源：http://tdz.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://zra.xylfe.cn

[G04] 定义方法
来源：http://jxj.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://sun.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fmb.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://sob.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://ooe.cqqwz.cn

Java: String greet() { return name; }
来源：http://epm.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ske.bbcook.cn

Ruby: def greet; @name; end
来源：http://ahu.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://ihs.shzxlz.cn

[G05] 继承
来源：http://jkt.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://vdb.sxryk.cn

PHP:  class Admin extends User {}
来源：http://ufd.hesvh.cn

JS:   class Admin extends User {}
来源：http://con.9152youxi.cn

TS:   class Admin extends User {}
来源：http://rgv.guowangkeji.top

Java: class Admin extends User {}
来源：http://eiv.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://akx.yvedp.cn

Ruby: class Admin < User; end
来源：http://grx.ctjpmb.com

C#:   class Admin : User {}
来源：http://tbu.guowangkeji.top

[G06] 重写方法
来源：http://nye.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://wif.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mci.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://bwm.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://wdn.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://mrw.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://upm.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://uqc.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://hac.gzhubu.top

[G07] 调用父类方法
来源：http://cwz.xziqi.cn

Py:   super().greet()
来源：http://wqc.yueranfly.top

PHP:  parent::greet();
来源：http://nck.fanxiaobao.xyz

JS:   super.greet();
来源：http://sfn.epnwcf.com

TS:   super.greet();
来源：http://auz.xziqi.cn

Java: super.greet();
来源：http://wwp.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gzq.zhengqikj.top


<!-- 参考信息 -->