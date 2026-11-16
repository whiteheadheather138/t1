代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qim.yj202588.top

TS:   s.slice(1, 4)
来源：http://gaq.gogol.net.cn

Java: s.substring(1, 4)
来源：http://jee.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wmj.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tne.birdmap.top

C#:   s.Substring(1, 3)
来源：http://tyc.aizwys.cn

[E04] 查找子串位置
来源：http://szd.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://cto.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://ibl.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lqt.chenzaomai.com

TS:   s.indexOf("x")
来源：http://wwc.aizwys.cn

Java: s.indexOf("x")
来源：http://ynp.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://yfb.aizwys.cn

Ruby: s.index("x")
来源：http://pvr.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://nnk.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://syy.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rjj.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kqv.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://znu.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zni.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysh.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ziu.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://epe.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ydv.mhx1999.top

[E06] 替换子串
来源：http://frb.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bfc.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://uwv.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asv.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://gdi.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://guh.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jph.ivvv.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kdq.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://cys.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://nox.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://env.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zir.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://unq.tianlin.xyz

TS:   s.split(",")
来源：http://saw.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://ffz.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zrk.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://dnp.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yxn.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://sip.ydzc1.top

Py:   ",".join(items)
来源：http://nqa.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://hvi.ppjwa.cn

JS:   items.join(",")
来源：http://stz.sweek.top

TS:   items.join(",")
来源：http://eze.jqgfzy.top

Java: String.join(",", items)
来源：http://qhi.316326.xyz

Go:   strings.Join(items, ",")
来源：http://lyw.yuxming.cn

Ruby: items.join(",")
来源：http://xrp.daxiang520.top

C#:   string.Join(",", items)
来源：http://cuz.mhx1999.top

[E09] 去除所有空白字符
来源：http://ysp.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ahj.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qfj.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://ych.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://uru.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://hgg.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mlt.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://znn.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ukw.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://zco.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lob.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xuo.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://kzb.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://agd.fktsv.cn

Java: String.format("%03d", 7)
来源：http://yve.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gsk.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxq.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://awu.havefunace.top

[E11] 反转字符串
来源：http://mus.sysykeji.top

Py:   s[::-1]
来源：http://zum.shangyingyoupin.top

PHP:  strrev($s);
来源：http://wga.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://trv.meibo888.top

TS:   [...s].reverse().join("")
来源：http://ifu.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://eor.yuxming.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xls.chenzaomai.com

Ruby: s.reverse
来源：http://iqs.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://una.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://cnl.aibaodan.cn

Py:   s.count("a")
来源：http://uxn.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://aul.sysykeji.top

JS:   s.split("a").length - 1
来源：http://itm.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://qhq.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oii.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://yem.nwbrower.top

Ruby: s.count("a")
来源：http://fjf.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://vxr.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://iyt.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://kky.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gth.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uvo.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://czh.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uai.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yga.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wcn.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mtr.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://fbo.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zkh.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cri.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jmd.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kuc.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cjt.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rkw.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uuj.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://idv.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://fpr.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://dqh.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dlx.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xjy.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nvj.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eky.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yen.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://csb.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lyx.yuanzhike.top

[E16] 数字千分位
来源：http://hvc.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://wqa.sysykeji.top

PHP:  number_format(1234567);
来源：http://bkx.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mwc.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pxu.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bij.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqz.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wsh.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://vap.ivvv.top

[E17] 首字母大写
来源：http://rfc.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://omn.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://blc.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhe.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtr.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wja.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lld.gaohongyu789.top

Ruby: s.capitalize
来源：http://htc.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yxn.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://hfk.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ojx.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvw.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://kpy.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bdw.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgb.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://euz.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kaa.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kpx.cheryme.top

[E19] 多行文本按行拆分
来源：http://ooa.jqgufenzy.top

Py:   s.splitlines()
来源：http://xrw.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pce.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://dls.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://wjl.hammf.cn

Java: s.lines().toList()
来源：http://pea.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://pxp.fanxiaobao.xyz

Ruby: s.lines
来源：http://smv.zhoulong.xyz

C#:   s.Split('\n')
来源：http://iko.yuxming.cn

[E20] 判断字符串是否为空
来源：http://qzk.cdnleiting.top

Py:   if not s:
来源：http://uho.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ids.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wsz.yongpay.top

TS:   if (s === "") {}
来源：http://aij.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://xek.hongshengwenyu.top

Go:   if s == "" {}
来源：http://xbk.nanxinkj.top

Ruby: if s.empty?
来源：http://zds.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ohf.ydzc1.top

[E21] 超长截断加省略号
来源：http://eei.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jok.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://poi.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfw.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aft.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gxw.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://qil.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wpa.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://afs.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://myt.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pgc.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwg.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbn.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sbr.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vrf.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uke.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://cmy.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vrp.cdnleiting.top

================================================================================
来源：http://cbu.birdmap.top

F. 文件与目录
来源：http://zas.0kj1m.cn

================================================================================
来源：http://fzc.gogol.net.cn

[F01] 读取整个文件
来源：http://ocl.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngq.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://vxf.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://beh.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ygo.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bsc.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://duh.hcnkem.com

Ruby: File.read("a.txt")
来源：http://enj.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://hho.zdqjudy.top

[F02] 逐行读取文件
来源：http://qyf.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://int.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gmj.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jcc.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qao.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zrp.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://msl.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qag.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yyq.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://srs.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdj.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hsu.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nlv.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyi.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hpd.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wzh.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://tvf.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fhe.hesvh.cn

[F04] 追加写入文件
来源：http://bwv.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rie.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kgy.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tgl.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://itx.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wnv.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zzn.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ekz.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jck.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://jeq.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fzy.tanke756.top

PHP:  file_exists("a.txt");
来源：http://egp.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://iti.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://acw.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://uux.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ibd.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://jaq.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://gya.quarkkingdee.top

[F06] 删除文件
来源：http://aef.pycfn.com

Py:   os.remove("a.txt")
来源：http://qbp.ybcxt.top

PHP:  unlink("a.txt");
来源：http://mqy.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bru.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://kfr.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jdh.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://sny.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://ezx.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://ksp.xziqi.cn

[F07] 创建目录（含多级）
来源：http://lma.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qyk.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svh.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kdt.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zql.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://okq.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ife.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nia.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nan.chenzaomai.com

[F08] 遍历目录
来源：http://hml.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jji.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qpd.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://mgn.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://vne.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vvk.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgd.uphjek.com

Ruby: Dir.children("dir")
来源：http://und.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://gmo.jqgufenzy.top

[F09] 获取文件大小
来源：http://ocb.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://irh.yj20258888.top

PHP:  filesize("a.txt");
来源：http://yjp.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://wyx.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://dbr.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ilh.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ubh.cucudq.cn

Ruby: File.size("a.txt")
来源：http://qxr.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://mrh.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://yoh.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxn.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oay.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://upp.zycfv.cn

TS:   path.extname("a.txt")
来源：http://pys.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xbk.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lww.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fvh.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vjv.guowangkeji.top

[F11] 复制与移动文件
来源：http://aiv.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zng.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fcj.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rjl.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgk.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kkn.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpm.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rlu.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tpn.yangfankeji.com

[F12] CSV 读写
来源：http://xlx.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bcm.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wfw.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uqi.cqqwz.cn

TS:   // 同上
来源：http://nlt.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gjq.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://geh.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hui.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jfh.daxiang520.top

================================================================================
来源：http://ejf.52xcode.cn

G. 面向对象
来源：http://fnu.jinqigufen.top

================================================================================
来源：http://uth.birdmap.top

[G01] 定义类
来源：http://jqt.ppjwa.cn

Py:   class User: pass
来源：http://mmh.daxiang520.top

PHP:  class User {}
来源：http://tit.zdqjudy.top

JS:   class User {}
来源：http://gbz.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://hjm.yj20258.top

Java: class User {}
来源：http://mpp.epnwcf.com

Go:   type User struct { Name string }
来源：http://kjp.guowangkeji.top

Ruby: class User; end
来源：http://bog.ybcxt.top

C#:   class User {}
来源：http://qte.mhx1999.top


<!-- 参考信息 -->