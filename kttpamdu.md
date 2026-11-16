代发 wailian999

PHP:  implode(",", $items);
来源：http://wkz.wangshuangyany.cn

JS:   items.join(",")
来源：http://yyk.andypj.xyz

TS:   items.join(",")
来源：http://trx.zhijiandao.cn

Java: String.join(",", items)
来源：http://owt.tanke756.top

Go:   strings.Join(items, ",")
来源：http://cgm.jqgfzy.top

Ruby: items.join(",")
来源：http://rdn.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://vbd.52xcode.cn

[E09] 去除所有空白字符
来源：http://byj.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mja.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ils.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://equ.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://lkd.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://irx.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lev.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://bhc.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pmu.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://upi.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://csh.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://icf.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://lji.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://oyz.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://vxu.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ofu.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oij.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tgk.zhongyouzk.top

[E11] 反转字符串
来源：http://niv.hfpthk.cn

Py:   s[::-1]
来源：http://jud.smart0.xyz

PHP:  strrev($s);
来源：http://ser.cashguo.top

JS:   [...s].reverse().join("")
来源：http://zwk.tanke756.top

TS:   [...s].reverse().join("")
来源：http://plq.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qny.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dut.ybcxt.top

Ruby: s.reverse
来源：http://eqi.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://apr.gzhubu.top

[E12] 统计某字符出现次数
来源：http://ahv.bbcook.cn

Py:   s.count("a")
来源：http://xog.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://tqh.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://grm.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://kom.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pfe.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://ipt.aibaodan.cn

Ruby: s.count("a")
来源：http://xeg.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://ugp.cqqwz.cn

[E13] 逐字符遍历
来源：http://idd.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://lkz.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wgi.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://yar.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://kil.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qbd.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://luf.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pcu.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hor.cashguo.top

[E14] URL 编码与 Base64
来源：http://mwd.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hmr.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sav.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qfx.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tqy.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ncg.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gmd.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xus.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://edp.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://kzw.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fvo.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ofp.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yab.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://puv.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mnc.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dqk.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uia.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://twn.bjfxy.top

[E16] 数字千分位
来源：http://rsf.yj202588.top

Py:   f"{1234567:,}"
来源：http://cjf.fehbvm.com

PHP:  number_format(1234567);
来源：http://urm.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lww.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kcg.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://foh.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ouo.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ijs.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://lrq.smart0.xyz

[E17] 首字母大写
来源：http://ijh.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xmm.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ljq.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rbn.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jse.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lrm.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vjc.shzxlz.cn

Ruby: s.capitalize
来源：http://nhs.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ooz.gotoacloud.top

[E18] 模板占位符替换
来源：http://mee.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bbf.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rgv.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eam.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qge.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xqs.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ejr.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://veq.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nzx.xziqi.cn

[E19] 多行文本按行拆分
来源：http://ceo.mhx1999.top

Py:   s.splitlines()
来源：http://trb.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xbn.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://qgs.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://ddw.52xcode.cn

Java: s.lines().toList()
来源：http://ohh.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://qek.chenjidiqi.icu

Ruby: s.lines
来源：http://wma.jqgufenzy.top

C#:   s.Split('\n')
来源：http://jkd.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://kbt.c1oappe.top

Py:   if not s:
来源：http://qgt.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xrn.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://huu.jianghu66.top

TS:   if (s === "") {}
来源：http://ucx.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://ufm.ydjk.org.cn

Go:   if s == "" {}
来源：http://zjm.hesvh.cn

Ruby: if s.empty?
来源：http://zcl.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mim.chenzaomai.com

[E21] 超长截断加省略号
来源：http://gqv.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aqt.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gza.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mmc.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://syh.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxo.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vtf.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sye.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ihg.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://xfk.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aax.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qeq.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wsd.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbb.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rat.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ask.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://mwv.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mxr.daxiang520.top

================================================================================
来源：http://wev.hesvh.cn

F. 文件与目录
来源：http://qeu.hongshengwenyu.top

================================================================================
来源：http://xbi.snrcjt.cn

[F01] 读取整个文件
来源：http://ihb.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xut.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://ntg.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xxp.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xaf.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rxf.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ieb.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://ujs.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://dud.zdbjq.cn

[F02] 逐行读取文件
来源：http://qvt.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://duf.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dqu.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ddw.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kki.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mdq.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cdf.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dah.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qvu.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://nsb.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mhh.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gke.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahf.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlf.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://soe.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kbs.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://cnb.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pct.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://ggv.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://smv.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eku.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xce.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vfu.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfp.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hvl.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pep.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rnf.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://sit.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ymw.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://zig.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://laj.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://ofc.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://scy.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mwl.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://jjg.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://ehi.zhengqikj.top

[F06] 删除文件
来源：http://gun.yfazqb.com

Py:   os.remove("a.txt")
来源：http://mnx.cheryme.top

PHP:  unlink("a.txt");
来源：http://jkl.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://oil.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://leg.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kfv.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://iqc.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://zvj.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://jtv.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://zib.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nmn.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eoz.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iqj.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vah.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kvb.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jmn.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://awg.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qqr.snrcjt.cn

[F08] 遍历目录
来源：http://aiw.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jjo.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ssy.sweek.top

JS:   fs.readdirSync("dir")
来源：http://wch.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://nbr.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://trp.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://lih.smart0.xyz

Ruby: Dir.children("dir")
来源：http://dah.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://jlz.chenlongwang.top

[F09] 获取文件大小
来源：http://hav.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://ugy.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://jip.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://ute.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://cdb.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://foj.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lze.yvedp.cn

Ruby: File.size("a.txt")
来源：http://tjm.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://stk.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://kwe.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kdo.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jga.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://avk.xinyue.icu

TS:   path.extname("a.txt")
来源：http://djd.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aax.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bvj.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zoy.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://okw.guowangkeji.top

[F11] 复制与移动文件
来源：http://eek.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://swe.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://krm.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzw.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdb.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vjn.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nlp.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vkx.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aib.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://kao.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sdn.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zcq.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://whr.jinyuanbaomall.cn

TS:   // 同上
来源：http://qhd.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fgq.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gze.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lya.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zkm.jqgufenzy.top

================================================================================
来源：http://sqp.daria6918.cn

G. 面向对象
来源：http://owj.hongshengwenyu.top

================================================================================
来源：http://jrd.chenzaomai.com

[G01] 定义类
来源：http://spb.zhengqikj.top

Py:   class User: pass
来源：http://ubb.sjlbkw.cn

PHP:  class User {}
来源：http://qwn.nanxuanxn.top

JS:   class User {}
来源：http://yzb.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://pho.yj202588.top

Java: class User {}
来源：http://hyq.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://bhh.birdmap.top

Ruby: class User; end
来源：http://yyf.hesvh.cn

C#:   class User {}
来源：http://bcw.fehbvm.com

[G02] 构造函数
来源：http://epg.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://xyj.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://beh.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://khq.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://qtm.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://rhl.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nzr.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://sae.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://rgy.meibo888.top

[G03] 实例属性
来源：http://kje.yongpay.top

Py:   self.name = "x"
来源：http://foh.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://ura.jinqigufen.top

JS:   this.name = "x";
来源：http://yya.316326.xyz

TS:   name: string = "x";
来源：http://woi.sweek.top

Java: private String name;
来源：http://gea.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cpu.ydzc1.top

Ruby: @name = "x"
来源：http://zjp.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://bqw.zhixingplan.top

[G04] 定义方法
来源：http://yyi.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://wpq.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zjm.xuanzx.com

JS:   greet() { return this.name; }
来源：http://qmh.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://lpn.fktsv.cn

Java: String greet() { return name; }
来源：http://vaj.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mzu.shuidangran.top

Ruby: def greet; @name; end
来源：http://wmf.birdmap.top

C#:   public string Greet() => Name;
来源：http://oez.nanxuanxn.top

[G05] 继承
来源：http://vcz.dashuyun.cn

Py:   class Admin(User): pass
来源：http://epd.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://jns.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://pio.zhixingplan.top

TS:   class Admin extends User {}
来源：http://ofi.gzhubu.top

Java: class Admin extends User {}
来源：http://qtt.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://okj.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://dnf.jianghu66.top

C#:   class Admin : User {}
来源：http://yww.jiagoushi.top

[G06] 重写方法
来源：http://bmy.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://qik.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ors.yj20258.top

JS:   greet() { return "admin"; }
来源：http://hpg.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://iey.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://axw.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tmu.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://fdy.jqgfzy.top


<!-- 参考信息 -->