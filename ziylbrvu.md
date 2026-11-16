代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lpb.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://jpm.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://anu.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cgo.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://kwm.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://jnd.birdmap.top

[E04] 查找子串位置
来源：http://hca.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://lxe.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://xcg.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sxr.fktsv.cn

TS:   s.indexOf("x")
来源：http://zek.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://qqw.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://mqm.hywenlv.cn

Ruby: s.index("x")
来源：http://rnd.hcnkem.com

C#:   s.IndexOf("x")
来源：http://mak.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ios.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ylv.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://apg.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucm.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qeg.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ssd.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nic.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lip.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nmz.jianghu66.top

[E06] 替换子串
来源：http://xav.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kug.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://wql.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pkg.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://qjd.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://seg.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dtc.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nvp.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://cbe.sufxvd.cn

[E07] 按分隔符拆分
来源：http://otk.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qui.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wzi.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vmw.hammf.cn

TS:   s.split(",")
来源：http://ehy.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://bdu.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hte.meibo888.top

Ruby: s.split(",");  s.split
来源：http://lhk.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nnu.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://xnw.ybcxt.top

Py:   ",".join(items)
来源：http://asx.9152youxi.cn

PHP:  implode(",", $items);
来源：http://nmw.gotoacloud.top

JS:   items.join(",")
来源：http://pki.shuidangran.top

TS:   items.join(",")
来源：http://ifk.jqgufenzy.top

Java: String.join(",", items)
来源：http://qrv.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://blz.hongshengwenyu.top

Ruby: items.join(",")
来源：http://owq.yvedp.cn

C#:   string.Join(",", items)
来源：http://vko.bjfxy.top

[E09] 去除所有空白字符
来源：http://eoj.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pca.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcp.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://tzs.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://cua.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://jhn.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zwa.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://pyj.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://idj.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://rdq.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kzc.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yxp.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://bng.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://tzo.tanke756.top

Java: String.format("%03d", 7)
来源：http://pzn.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gcn.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://drt.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ngx.sxryk.cn

[E11] 反转字符串
来源：http://huo.shzxlz.cn

Py:   s[::-1]
来源：http://ras.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://qrw.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://jov.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://tqd.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dpj.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ekk.cucudq.cn

Ruby: s.reverse
来源：http://bcr.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://hym.smart0.xyz

[E12] 统计某字符出现次数
来源：http://xog.hcnkem.com

Py:   s.count("a")
来源：http://bkc.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://muo.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://stg.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://xol.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lww.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://dso.hfpthk.cn

Ruby: s.count("a")
来源：http://nxk.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://vqb.gzhubu.top

[E13] 逐字符遍历
来源：http://uxz.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://ccg.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ypf.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kdy.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wgb.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ync.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gsa.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://kda.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyb.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://aaa.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://emv.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jrv.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xxa.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ulh.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jxk.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dot.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cdz.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zit.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://srx.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zvh.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyf.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rsa.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ftx.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gyx.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyf.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tda.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bag.jinqigfzy.top

[E16] 数字千分位
来源：http://jaz.hcnkem.com

Py:   f"{1234567:,}"
来源：http://zxy.tarul.cn

PHP:  number_format(1234567);
来源：http://irk.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aol.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wyr.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://snz.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxd.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gts.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://wjg.cashguo.top

[E17] 首字母大写
来源：http://xtx.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tia.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uck.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otz.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzi.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ayx.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://abe.birdmap.top

Ruby: s.capitalize
来源：http://lsv.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kty.zycfv.cn

[E18] 模板占位符替换
来源：http://dds.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qmc.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fdx.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lqy.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uki.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdp.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qrh.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kbi.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://spr.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://nya.aizwys.cn

Py:   s.splitlines()
来源：http://fyu.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzo.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://pkw.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://ktn.ydzc1.top

Java: s.lines().toList()
来源：http://adb.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://qmc.daxiang520.top

Ruby: s.lines
来源：http://onr.gotoacloud.top

C#:   s.Split('\n')
来源：http://fqs.wangdashe.top

[E20] 判断字符串是否为空
来源：http://kfk.haohaochexian.top

Py:   if not s:
来源：http://arl.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hrl.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wcr.jiagoushi.top

TS:   if (s === "") {}
来源：http://mdi.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://qyj.pycfn.com

Go:   if s == "" {}
来源：http://yrq.hnqzz.top

Ruby: if s.empty?
来源：http://mlz.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://btb.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://gvo.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jfa.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aja.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tef.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://skr.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://auz.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://tri.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mof.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rkl.bbcook.cn

[E22] 字节长度与字符长度
来源：http://gsc.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxx.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nna.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://whv.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://idf.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bvi.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eok.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://mxs.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ydh.ydjk.org.cn

================================================================================
来源：http://yae.hfpthk.cn

F. 文件与目录
来源：http://tvv.yj202588.top

================================================================================
来源：http://miz.0kj1m.cn

[F01] 读取整个文件
来源：http://zdn.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yos.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://kpx.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://czi.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://emh.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://npu.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lvc.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://xmv.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://lsn.zycfv.cn

[F02] 逐行读取文件
来源：http://bld.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eip.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pjx.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hbl.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qxf.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qag.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://era.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xgj.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ysy.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://lab.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mri.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xvy.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrt.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jyl.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://okl.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wie.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://rhs.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fov.xinyue.icu

[F04] 追加写入文件
来源：http://iil.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cun.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tys.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vll.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kij.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ppm.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jrl.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zou.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mnk.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://qmm.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://onh.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://oqh.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://xru.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://kxw.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ycs.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://axv.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://dmd.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://upd.yj20258.top

[F06] 删除文件
来源：http://cvh.xinyue.icu

Py:   os.remove("a.txt")
来源：http://opx.nwbrower.top

PHP:  unlink("a.txt");
来源：http://dnh.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://fry.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://gzr.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fjh.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://gmt.uphjek.com

Ruby: File.delete("a.txt")
来源：http://nai.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://gis.yvedp.cn

[F07] 创建目录（含多级）
来源：http://fof.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vfu.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://icq.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dbs.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivo.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gcm.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ejk.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nmt.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nmm.mhx1999.top

[F08] 遍历目录
来源：http://qvb.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jxc.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://put.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://ygf.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://joh.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sjk.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wxp.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://uwq.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://wob.dianchejie.cn

[F09] 获取文件大小
来源：http://fah.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://nlq.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://qkx.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://guu.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://jmu.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iou.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://edp.pycfn.com

Ruby: File.size("a.txt")
来源：http://kbh.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://vzy.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://nos.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vsh.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://noa.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sav.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://axz.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oem.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xiu.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://usi.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjo.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://jdp.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nfr.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dqh.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eja.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pfj.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cmt.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kex.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cox.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://alm.sufxvd.cn

[F12] CSV 读写
来源：http://xuh.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qvz.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://opg.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tgz.hcnkem.com

TS:   // 同上
来源：http://gua.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lmw.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jjk.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjv.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://bqx.ydjk.org.cn

================================================================================
来源：http://fqh.316326.xyz

G. 面向对象
来源：http://rge.daria6918.cn

================================================================================
来源：http://gev.ppjwa.cn

[G01] 定义类
来源：http://gbf.hnqzz.top

Py:   class User: pass
来源：http://byc.tianlin.xyz

PHP:  class User {}
来源：http://ark.aibaodan.cn

JS:   class User {}
来源：http://mtb.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://icc.xziqi.cn

Java: class User {}
来源：http://ctb.sysykeji.top

Go:   type User struct { Name string }
来源：http://tzw.zhiwuduotai.top

Ruby: class User; end
来源：http://stv.shanyushiyangkeji.top

C#:   class User {}
来源：http://swi.hcnkem.com


<!-- 参考信息 -->