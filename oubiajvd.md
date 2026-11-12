代发 wailian999

Ruby: s.split(",");  s.split
来源：http://lhj.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yth.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://ulw.gotoacloud.top

Py:   ",".join(items)
来源：http://kdg.cheryme.top

PHP:  implode(",", $items);
来源：http://hwm.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://bzp.epnwcf.com

TS:   items.join(",")
来源：http://hdn.52xcode.cn

Java: String.join(",", items)
来源：http://lhl.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://snm.zhoulong.xyz

Ruby: items.join(",")
来源：http://zpb.havefunace.top

C#:   string.Join(",", items)
来源：http://tsm.yangfankeji.com

[E09] 去除所有空白字符
来源：http://nus.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iqd.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lht.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://ikv.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://rlp.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://fpf.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qui.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://kdz.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cte.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://gff.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oke.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zyk.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://lqy.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://vsl.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://hlk.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cay.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iwn.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jpn.shzxlz.cn

[E11] 反转字符串
来源：http://niu.wangshuangyany.cn

Py:   s[::-1]
来源：http://slt.jianghu66.top

PHP:  strrev($s);
来源：http://ewh.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://pqr.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://thx.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://mxe.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xpy.yj202588.top

Ruby: s.reverse
来源：http://dqp.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://sgx.shuidangran.top

[E12] 统计某字符出现次数
来源：http://uqt.meibo888.top

Py:   s.count("a")
来源：http://wty.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://zyo.tarul.cn

JS:   s.split("a").length - 1
来源：http://vpp.andypj.xyz

TS:   s.split("a").length - 1
来源：http://agr.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jcg.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ocg.xuanzx.com

Ruby: s.count("a")
来源：http://rvg.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://zyw.kuanghao11.cn

[E13] 逐字符遍历
来源：http://xwi.hcnkem.com

Py:   for ch in s: print(ch)
来源：http://dnq.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tzf.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bfy.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vcj.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xso.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://war.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://agg.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kac.fktsv.cn

[E14] URL 编码与 Base64
来源：http://twd.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yip.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gau.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sme.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aye.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tvm.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oan.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://slg.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mem.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://qcy.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://djk.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dpp.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kij.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://keg.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jzp.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kfc.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mpy.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://klc.yfazqb.com

[E16] 数字千分位
来源：http://fis.hcnkem.com

Py:   f"{1234567:,}"
来源：http://ver.9152youxi.cn

PHP:  number_format(1234567);
来源：http://vqm.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://djf.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ohs.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vjc.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sjl.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dos.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://kqv.xylfe.cn

[E17] 首字母大写
来源：http://sna.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ccd.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://csk.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upx.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kxi.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mwq.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ivq.tian-w.cn

Ruby: s.capitalize
来源：http://pwu.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ltd.epnwcf.com

[E18] 模板占位符替换
来源：http://ftr.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://llm.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lwg.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vtr.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://akc.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://igt.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zlv.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uos.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bse.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://fwg.0kj1m.cn

Py:   s.splitlines()
来源：http://qff.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chn.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://pkq.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://ghf.yuanzhike.top

Java: s.lines().toList()
来源：http://yiz.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://mbm.9152youxi.cn

Ruby: s.lines
来源：http://hvl.fktsv.cn

C#:   s.Split('\n')
来源：http://sql.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://okb.zhiwuduotai.top

Py:   if not s:
来源：http://byz.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lby.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dmm.jlsjyb.cn

TS:   if (s === "") {}
来源：http://gyo.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://jve.tanke756.top

Go:   if s == "" {}
来源：http://kab.zhengqikj.top

Ruby: if s.empty?
来源：http://emi.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ccl.chenlongwang.top

[E21] 超长截断加省略号
来源：http://xbc.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zpu.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwd.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptq.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xny.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dca.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://epe.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wmm.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oqg.gzhubu.top

[E22] 字节长度与字符长度
来源：http://onh.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hus.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wza.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipm.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://myg.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vhe.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cvg.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://xpu.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fbs.cucudq.cn

================================================================================
来源：http://bct.hnqzz.top

F. 文件与目录
来源：http://odd.yj20258888.top

================================================================================
来源：http://trc.hnqzz.top

[F01] 读取整个文件
来源：http://edh.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ooa.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://yca.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tfp.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://svk.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qhy.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xyl.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://sln.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://gva.epnwcf.com

[F02] 逐行读取文件
来源：http://ode.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yhh.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sco.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohk.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpy.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://czs.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ppf.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kai.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pjr.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://kqo.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fbz.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iww.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuz.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tob.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuz.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jcu.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://jdb.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwt.xziqi.cn

[F04] 追加写入文件
来源：http://ytp.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fmh.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nyg.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ugo.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://glh.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lez.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sjc.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uyf.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rly.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://jcw.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wlp.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://xdx.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://jhn.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://kso.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sty.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xmi.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://xgl.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://dro.birdmap.top

[F06] 删除文件
来源：http://sah.wangshuangyany.cn

Py:   os.remove("a.txt")
来源：http://bev.pycfn.com

PHP:  unlink("a.txt");
来源：http://qwy.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fyb.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://fat.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jzi.havefunace.top

Go:   os.Remove("a.txt")
来源：http://lvq.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://kqr.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://abg.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://ptt.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://odf.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbx.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zpq.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emt.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://isx.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://quh.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://snx.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ixr.sjlbkw.cn

[F08] 遍历目录
来源：http://dlq.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mbu.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iij.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://wbt.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://ooe.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgn.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fvd.yongpay.top

Ruby: Dir.children("dir")
来源：http://fri.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://usy.zdqjudy.top

[F09] 获取文件大小
来源：http://oul.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://evy.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://qal.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://vjo.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://pve.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://thj.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyu.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://mus.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://zkg.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://pdy.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uea.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://awc.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wmr.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://bux.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://djy.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhh.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jhv.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vlr.zycfv.cn

[F11] 复制与移动文件
来源：http://yhg.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kio.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpv.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jsi.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppj.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uvv.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://okt.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vji.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wkt.quarkkingdee.top

[F12] CSV 读写
来源：http://zdz.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tgz.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zrl.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cnv.shanyushiyangkeji.top

TS:   // 同上
来源：http://rle.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wmu.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ddc.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://usi.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mfr.ivvv.top

================================================================================
来源：http://nhx.gotoacloud.top

G. 面向对象
来源：http://odf.yfazqb.com

================================================================================
来源：http://juk.dianchejie.cn

[G01] 定义类
来源：http://ibz.nanxuanxn.top

Py:   class User: pass
来源：http://oyy.fzhhl.top

PHP:  class User {}
来源：http://tps.bbcook.cn

JS:   class User {}
来源：http://rqc.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://tfg.quarkkingdee.top

Java: class User {}
来源：http://wrv.yuanzhike.top

Go:   type User struct { Name string }
来源：http://jzv.kuanghao11.cn

Ruby: class User; end
来源：http://htx.ppjwa.cn

C#:   class User {}
来源：http://hrp.andypj.xyz

[G02] 构造函数
来源：http://mbf.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://ybo.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://byz.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://kdy.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://fjz.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://dvo.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://spv.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://sem.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://xbp.jinqigfzy.top

[G03] 实例属性
来源：http://rgr.hfpthk.cn

Py:   self.name = "x"
来源：http://dye.birdmap.top

PHP:  public string $name = "x";
来源：http://dio.hywenlv.cn

JS:   this.name = "x";
来源：http://vcm.gotoacloud.top

TS:   name: string = "x";
来源：http://mwa.mhx1999.top

Java: private String name;
来源：http://aqd.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xfh.chenlongwang.top

Ruby: @name = "x"
来源：http://unu.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://fhw.fehbvm.com

[G04] 定义方法
来源：http://pei.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://uia.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxk.hcnkem.com

JS:   greet() { return this.name; }
来源：http://ehm.sweek.top

TS:   greet(): string { return this.name; }
来源：http://fct.cucudq.cn

Java: String greet() { return name; }
来源：http://njl.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://myt.sxryk.cn

Ruby: def greet; @name; end
来源：http://omh.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://goq.daxiang520.top

[G05] 继承
来源：http://vdv.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://wrp.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://xoc.fktsv.cn

JS:   class Admin extends User {}
来源：http://vik.ybcxt.top

TS:   class Admin extends User {}
来源：http://old.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://bnt.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aeg.xziqi.cn

Ruby: class Admin < User; end
来源：http://pjj.vehdjk.com

C#:   class Admin : User {}
来源：http://ttl.fktsv.cn

[G06] 重写方法
来源：http://aek.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://bva.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://olf.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://apf.yj202588.top


<!-- 参考信息 -->