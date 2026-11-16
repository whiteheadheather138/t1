代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://tlc.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vof.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://win.jinqigfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zjq.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://mxu.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://byz.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ykl.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://rhc.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://qdg.meibo888.top

Java: String.format("%03d", 7)
来源：http://vek.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gve.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xue.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rec.yonumen.top

[E11] 反转字符串
来源：http://pnx.ehwqpu.com

Py:   s[::-1]
来源：http://wlb.xziqi.cn

PHP:  strrev($s);
来源：http://emh.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://ycq.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://vur.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tir.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vvp.ppjwa.cn

Ruby: s.reverse
来源：http://xko.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://ipc.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://fsk.gogol.net.cn

Py:   s.count("a")
来源：http://xpz.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://gwy.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://laj.wangdashe.top

TS:   s.split("a").length - 1
来源：http://vuw.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pzz.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://anb.pengpengdd.cyou

Ruby: s.count("a")
来源：http://nqp.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://baw.ybcxt.top

[E13] 逐字符遍历
来源：http://uao.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://buz.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zoz.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dgi.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wte.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rpu.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aug.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gda.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://crs.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://muh.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yqo.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gwl.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gpl.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fdt.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llb.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yqq.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gph.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zur.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://xtb.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vvv.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qge.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dje.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qbl.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zpv.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://plh.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xnp.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qim.wangshuangyany.cn

[E16] 数字千分位
来源：http://rjj.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://dgq.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://dcb.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cwg.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dbf.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gwa.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://izq.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jum.ivvv.top

C#:   1234567.ToString("N0")
来源：http://gki.iojbl.cn

[E17] 首字母大写
来源：http://ukh.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bed.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ggm.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fjt.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://joy.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://owg.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jha.daxiang520.top

Ruby: s.capitalize
来源：http://oht.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sul.haohaochexian.top

[E18] 模板占位符替换
来源：http://fiy.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xst.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zsi.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://nzm.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cac.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wqk.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iif.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mgc.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rou.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://rko.wangdashe.top

Py:   s.splitlines()
来源：http://kmb.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kub.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://krp.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://wxi.hnxiangtu.top

Java: s.lines().toList()
来源：http://nfq.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://qtf.sjlbkw.cn

Ruby: s.lines
来源：http://rtw.yangfankeji.com

C#:   s.Split('\n')
来源：http://nce.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://zrq.hfpthk.cn

Py:   if not s:
来源：http://lbp.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kca.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dsr.ehwqpu.com

TS:   if (s === "") {}
来源：http://cbh.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://acu.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://vha.ybcxt.top

Ruby: if s.empty?
来源：http://pbq.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xwc.sxryk.cn

[E21] 超长截断加省略号
来源：http://otv.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tyb.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lue.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tjg.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ped.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wrh.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://jnq.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://etz.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://quc.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://mpr.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uus.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yxv.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wuz.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://byy.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jxr.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://anj.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://zar.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ack.daxiang520.top

================================================================================
来源：http://cha.fanxiaobao.xyz

F. 文件与目录
来源：http://wbt.xuetiantiany.cn

================================================================================
来源：http://xhh.hcnkem.com

[F01] 读取整个文件
来源：http://zfa.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pza.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://qyx.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://scz.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kgy.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://vpl.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vup.hammf.cn

Ruby: File.read("a.txt")
来源：http://ogg.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://pfw.jyoumei.cn

[F02] 逐行读取文件
来源：http://nrg.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wzm.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jql.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puh.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcc.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bwe.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tnv.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zwf.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wpl.meibo888.top

[F03] 写入文件（覆盖）
来源：http://kvt.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pem.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lty.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ayq.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iat.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zsh.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uce.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://xrd.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yos.vehdjk.com

[F04] 追加写入文件
来源：http://lmb.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zko.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tpt.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swr.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jkw.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qvm.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pbz.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lcj.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mzm.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://muh.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ovb.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://fvr.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://hmh.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://gkr.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ghc.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nxf.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://llq.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://gyy.guowangkeji.top

[F06] 删除文件
来源：http://mxp.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://tmv.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://wlp.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://kbm.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://its.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ocd.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://ccd.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://ktr.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://qzl.ybcxt.top

[F07] 创建目录（含多级）
来源：http://nsf.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ual.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cgd.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqi.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://udz.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nnx.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yye.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wyr.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ihz.hywenlv.cn

[F08] 遍历目录
来源：http://def.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tjg.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xms.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://som.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://cpl.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xlm.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aim.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://nxb.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://sae.yuxming.cn

[F09] 获取文件大小
来源：http://vdy.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://qlz.yvedp.cn

PHP:  filesize("a.txt");
来源：http://nsj.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://knk.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://gxx.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dvh.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://odh.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://dhs.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://agm.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://rxq.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yky.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjj.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hnl.daria6918.cn

TS:   path.extname("a.txt")
来源：http://gze.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zra.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ren.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cij.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zmr.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://pyv.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ked.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okz.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhs.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qmk.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dxc.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wmo.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wzh.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbc.cucudq.cn

[F12] CSV 读写
来源：http://byy.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dzs.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ryz.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://akb.c1oappe.top

TS:   // 同上
来源：http://kor.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ysa.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ksl.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dwo.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://utk.birdmap.top

================================================================================
来源：http://dpl.sweek.top

G. 面向对象
来源：http://wkn.chenjidiqi.icu

================================================================================
来源：http://jix.shuidangran.top

[G01] 定义类
来源：http://yrn.sxryk.cn

Py:   class User: pass
来源：http://tsn.shanyushiyangtech.top

PHP:  class User {}
来源：http://hxu.ctjpmb.com

JS:   class User {}
来源：http://lhf.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://lqj.shanyushiyangkeji.top

Java: class User {}
来源：http://kjx.xylfe.cn

Go:   type User struct { Name string }
来源：http://jxa.ydjk.org.cn

Ruby: class User; end
来源：http://obr.haohaochexian.top

C#:   class User {}
来源：http://scg.tanke756.top

[G02] 构造函数
来源：http://jiv.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://poz.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://rst.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://utg.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://vvg.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://dog.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uai.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://vjy.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://nhv.shanyushiyangtech.top

[G03] 实例属性
来源：http://nvr.ybcxt.top

Py:   self.name = "x"
来源：http://ndc.9152youxi.cn

PHP:  public string $name = "x";
来源：http://qbn.cheryme.top

JS:   this.name = "x";
来源：http://won.yangfankeji.com

TS:   name: string = "x";
来源：http://vgi.epnwcf.com

Java: private String name;
来源：http://dax.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hwz.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://mhd.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://iwj.ywan-chungtsiang.top

[G04] 定义方法
来源：http://iim.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://awi.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ilc.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://ler.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://gqg.yuxming.cn

Java: String greet() { return name; }
来源：http://ado.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzx.gzhubu.top

Ruby: def greet; @name; end
来源：http://kkf.sxryk.cn

C#:   public string Greet() => Name;
来源：http://dmh.mhx1999.top

[G05] 继承
来源：http://cst.fktsv.cn

Py:   class Admin(User): pass
来源：http://pvc.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://xcr.tianlin.xyz

JS:   class Admin extends User {}
来源：http://fxu.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://klo.ehwqpu.com

Java: class Admin extends User {}
来源：http://hzm.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nwd.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://utd.svipenyu.cn

C#:   class Admin : User {}
来源：http://skc.haohaochexian.top

[G06] 重写方法
来源：http://zsf.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://gwf.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dga.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://hcw.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://yrt.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://rrw.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hco.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://noa.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://lqn.svipenyu.cn

[G07] 调用父类方法
来源：http://zao.yvedp.cn

Py:   super().greet()
来源：http://kbg.yfazqb.com

PHP:  parent::greet();
来源：http://dti.gaohongyu789.top

JS:   super.greet();
来源：http://luq.vehdjk.com

TS:   super.greet();
来源：http://vke.jlsjyb.cn

Java: super.greet();
来源：http://swn.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xty.andypj.xyz

Ruby: super
来源：http://acw.guowangkeji.top

C#:   base.Greet();
来源：http://gak.meibo888.top

[G08] 静态方法与属性
来源：http://rlc.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ofu.yongpay.top


<!-- 参考信息 -->