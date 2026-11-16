代发 wailian999

PHP:  implode(",", $items);
来源：http://hxu.wangshuangyany.cn

JS:   items.join(",")
来源：http://cxk.yonumen.top

TS:   items.join(",")
来源：http://jjf.yueranfly.top

Java: String.join(",", items)
来源：http://lcs.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://eev.ctjpmb.com

Ruby: items.join(",")
来源：http://lir.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://wpm.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://kvd.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yjx.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oil.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://whu.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://nti.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://dmi.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oiz.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qdj.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yep.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://utw.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qgp.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jxe.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://tup.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://hqk.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://dvj.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wtm.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qko.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ufy.xuanzx.com

[E11] 反转字符串
来源：http://efp.wangdashe.top

Py:   s[::-1]
来源：http://zve.tianlin.xyz

PHP:  strrev($s);
来源：http://wge.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://eeu.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://mpp.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uaf.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://von.hnxiangtu.top

Ruby: s.reverse
来源：http://nix.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yqx.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://qbp.haohaochexian.top

Py:   s.count("a")
来源：http://tvl.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://jom.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://zew.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://taa.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cng.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://mdd.shangyingyoupin.top

Ruby: s.count("a")
来源：http://jre.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://zxi.chenzaomai.com

[E13] 逐字符遍历
来源：http://qau.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://kmw.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rrx.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zel.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qsz.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rqk.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xsw.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pcp.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://obh.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://hjn.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cvw.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vhg.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://asl.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rvr.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vne.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ugl.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqs.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hdt.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://zmb.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yxs.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tkd.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qyz.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tqr.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhz.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tdu.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zwb.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kte.xylfe.cn

[E16] 数字千分位
来源：http://uyz.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://xwp.c1oappe.top

PHP:  number_format(1234567);
来源：http://kkr.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vsk.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gvm.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://moy.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xxe.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kkc.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://aef.jlsjyb.cn

[E17] 首字母大写
来源：http://gax.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://won.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://max.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dok.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lkd.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qck.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eay.ctjpmb.com

Ruby: s.capitalize
来源：http://rps.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eif.aizwys.cn

[E18] 模板占位符替换
来源：http://drp.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ipa.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aba.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lpl.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://puf.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bck.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqp.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ozz.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oso.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://nyj.zhoulong.xyz

Py:   s.splitlines()
来源：http://cqt.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ngg.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://hnq.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://xel.feifeiyinyue.top

Java: s.lines().toList()
来源：http://mhw.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://gts.9152youxi.cn

Ruby: s.lines
来源：http://uwl.ivvv.top

C#:   s.Split('\n')
来源：http://svc.316326.xyz

[E20] 判断字符串是否为空
来源：http://ttx.gzhubu.top

Py:   if not s:
来源：http://une.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdw.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eam.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://fbk.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://atc.jianghu66.top

Go:   if s == "" {}
来源：http://awp.yuxming.cn

Ruby: if s.empty?
来源：http://jag.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mdb.wangdashe.top

[E21] 超长截断加省略号
来源：http://xqn.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uqz.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fds.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://riw.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpn.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rhc.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://zjq.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cws.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://twn.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://wsr.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jyo.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxl.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tpl.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uam.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kbq.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gkm.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://gub.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://liy.chenlongwang.top

================================================================================
来源：http://klg.zhixingplan.top

F. 文件与目录
来源：http://rmj.jinqigfzy.top

================================================================================
来源：http://wyt.ivvv.top

[F01] 读取整个文件
来源：http://jmr.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gjo.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://dxn.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qxg.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hqc.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pra.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tga.fehbvm.com

Ruby: File.read("a.txt")
来源：http://orb.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://hfa.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://kbn.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ayl.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ndy.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vrb.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lft.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kag.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dcz.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ncg.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://skj.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://aic.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://efv.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://foj.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mpe.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wvw.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dpw.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ope.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://ywa.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lwq.jyoumei.cn

[F04] 追加写入文件
来源：http://byk.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cnb.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cmr.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gqp.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jnw.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vox.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdl.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://edz.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dxw.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://fds.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lth.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://jbd.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://dti.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://xfw.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fyw.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iyy.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://dwh.tanke756.top

C#:   File.Exists("a.txt")
来源：http://drx.dashuyun.cn

[F06] 删除文件
来源：http://rof.xuanzx.com

Py:   os.remove("a.txt")
来源：http://yus.tanke756.top

PHP:  unlink("a.txt");
来源：http://fgy.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://dww.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://pzz.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uon.yj20258.top

Go:   os.Remove("a.txt")
来源：http://yyf.yongpay.top

Ruby: File.delete("a.txt")
来源：http://avk.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://fpz.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://kwf.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ava.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mis.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mvv.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fzz.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pgt.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tny.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rbb.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dxb.vqdsnc.cn

[F08] 遍历目录
来源：http://awk.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tql.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iox.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://hzk.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://chv.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mbs.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aup.wangdashe.top

Ruby: Dir.children("dir")
来源：http://esi.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://nyk.aizwys.cn

[F09] 获取文件大小
来源：http://nfb.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ykn.bjfxy.top

PHP:  filesize("a.txt");
来源：http://cpl.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://ryk.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://uqn.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://xbu.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://son.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://pux.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://fzh.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://mxh.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bpr.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cew.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfh.hcnkem.com

TS:   path.extname("a.txt")
来源：http://uae.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzz.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ubs.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dtn.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ilz.ivvv.top

[F11] 复制与移动文件
来源：http://kll.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xri.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nws.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qol.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rer.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gxw.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hbz.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ayp.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://egj.vehdjk.com

[F12] CSV 读写
来源：http://tlf.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hhv.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rme.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qug.uphjek.com

TS:   // 同上
来源：http://xoy.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://byk.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dsj.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hti.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ivo.gogol.net.cn

================================================================================
来源：http://atj.316326.xyz

G. 面向对象
来源：http://cjf.ywan-chungtsiang.top

================================================================================
来源：http://uzp.yueranfly.top

[G01] 定义类
来源：http://qbu.chenlongwang.top

Py:   class User: pass
来源：http://can.tian-w.cn

PHP:  class User {}
来源：http://hif.hfpthk.cn

JS:   class User {}
来源：http://edp.yj202588.top

TS:   class User { name: string = ""; }
来源：http://ylr.fktsv.cn

Java: class User {}
来源：http://imt.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://nwc.ywan-chungtsiang.top

Ruby: class User; end
来源：http://nbm.fanxiaobao.xyz

C#:   class User {}
来源：http://prq.jyoumei.cn

[G02] 构造函数
来源：http://tqk.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://dwb.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://zlv.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://fiq.birdmap.top

TS:   constructor(public name: string) {}
来源：http://due.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://rmb.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvx.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://qyq.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://mnr.jlsjyb.cn

[G03] 实例属性
来源：http://ywe.epnwcf.com

Py:   self.name = "x"
来源：http://pgi.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://gqu.tarul.cn

JS:   this.name = "x";
来源：http://vqw.iojbl.cn

TS:   name: string = "x";
来源：http://thg.sjlbkw.cn

Java: private String name;
来源：http://bir.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hev.meibo888.top

Ruby: @name = "x"
来源：http://czl.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://rbc.birdmap.top

[G04] 定义方法
来源：http://qib.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://tzb.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yyx.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://ahw.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://kuq.cheryme.top

Java: String greet() { return name; }
来源：http://njx.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbj.zdqjudy.top

Ruby: def greet; @name; end
来源：http://ebl.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://smv.xylfe.cn

[G05] 继承
来源：http://ixt.zycfv.cn

Py:   class Admin(User): pass
来源：http://nke.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://qem.chenzaomai.com

JS:   class Admin extends User {}
来源：http://snr.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://lgw.nanxinkj.top

Java: class Admin extends User {}
来源：http://ibv.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wqx.jqgfzy.top

Ruby: class Admin < User; end
来源：http://doe.cashguo.top

C#:   class Admin : User {}
来源：http://uww.tian-w.cn

[G06] 重写方法
来源：http://mre.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://qwn.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fsk.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://zbj.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://edf.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ppz.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bdo.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://dwc.ehwqpu.com


<!-- 参考信息 -->