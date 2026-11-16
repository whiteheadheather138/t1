代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kef.jyoumei.cn

[E03] 截取子串
来源：http://gtp.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mkl.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nzc.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kix.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://ofw.fzhhl.top

Java: s.substring(1, 4)
来源：http://cyx.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://irt.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://mhr.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://gxz.xylfe.cn

[E04] 查找子串位置
来源：http://vfp.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://vvo.daria6918.cn

PHP:  strpos($s, "x");
来源：http://kwz.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hzd.shuidangran.top

TS:   s.indexOf("x")
来源：http://ttt.epnwcf.com

Java: s.indexOf("x")
来源：http://pwt.ivvv.top

Go:   strings.Index(s, "x")
来源：http://hxl.aibaodan.cn

Ruby: s.index("x")
来源：http://aks.aizwys.cn

C#:   s.IndexOf("x")
来源：http://rfp.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vfp.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nyh.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pgv.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ajy.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ubu.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxi.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tmd.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://veq.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvp.chenlongwang.top

[E06] 替换子串
来源：http://eyi.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sou.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://zhl.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbe.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://oyv.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ohd.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://evc.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gsp.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://wts.andypj.xyz

[E07] 按分隔符拆分
来源：http://nzu.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qjn.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hvo.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kdf.yangfankeji.com

TS:   s.split(",")
来源：http://nzn.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://xsy.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qwu.316326.xyz

Ruby: s.split(",");  s.split
来源：http://mcc.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ubf.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://orn.hongshengwenyu.top

Py:   ",".join(items)
来源：http://mgy.chenzaomai.com

PHP:  implode(",", $items);
来源：http://xkd.svipenyu.cn

JS:   items.join(",")
来源：http://eyb.dashuyun.cn

TS:   items.join(",")
来源：http://pqv.gotoacloud.top

Java: String.join(",", items)
来源：http://mbp.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://csl.wangdashe.top

Ruby: items.join(",")
来源：http://ygb.yangfankeji.com

C#:   string.Join(",", items)
来源：http://gwa.sxryk.cn

[E09] 去除所有空白字符
来源：http://gqn.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pgt.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypd.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://etk.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://jfu.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://vaa.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qel.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vpp.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bsd.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://xvk.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fye.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pml.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://zen.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://ddx.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://bxi.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yix.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fmu.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ezj.tian-w.cn

[E11] 反转字符串
来源：http://sau.ehwqpu.com

Py:   s[::-1]
来源：http://bns.yvedp.cn

PHP:  strrev($s);
来源：http://nyy.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://iup.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://qiu.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gew.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cge.kuanghao11.cn

Ruby: s.reverse
来源：http://nps.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://baz.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://jbx.hnqzz.top

Py:   s.count("a")
来源：http://udr.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://dvd.ivvv.top

JS:   s.split("a").length - 1
来源：http://enc.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://ciq.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kpo.birdmap.top

Go:   strings.Count(s, "a")
来源：http://ibi.tian-w.cn

Ruby: s.count("a")
来源：http://enn.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://ree.snrcjt.cn

[E13] 逐字符遍历
来源：http://edu.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://ped.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ysi.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rdu.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bme.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://shs.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hns.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://hqn.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dzs.birdmap.top

[E14] URL 编码与 Base64
来源：http://ygv.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mlb.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fce.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://azu.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nmn.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qie.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://whd.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://urd.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hsf.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://low.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bts.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lhx.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hrn.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zod.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qek.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yzv.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kbn.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sro.xuetiantiany.cn

[E16] 数字千分位
来源：http://diu.fengsongda.top

Py:   f"{1234567:,}"
来源：http://fyq.ybcxt.top

PHP:  number_format(1234567);
来源：http://yto.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rpa.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://joc.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jmm.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhu.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lle.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://duv.dashuyun.cn

[E17] 首字母大写
来源：http://liz.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ewp.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mjb.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtv.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lsz.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nfv.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ijg.aibaodan.cn

Ruby: s.capitalize
来源：http://vgn.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yeo.316326.xyz

[E18] 模板占位符替换
来源：http://zey.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lwm.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yld.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ciu.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://efd.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vuw.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vqc.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nkt.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ykv.daria6918.cn

[E19] 多行文本按行拆分
来源：http://wzg.nwbrower.top

Py:   s.splitlines()
来源：http://cix.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mgw.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://nkg.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://apk.yongpay.top

Java: s.lines().toList()
来源：http://edb.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://fek.zhongyouzk.top

Ruby: s.lines
来源：http://kpl.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://kwf.aizwys.cn

[E20] 判断字符串是否为空
来源：http://mvj.nanxinkj.top

Py:   if not s:
来源：http://kjb.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kun.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wzr.jyoumei.cn

TS:   if (s === "") {}
来源：http://pkw.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://bje.0kj1m.cn

Go:   if s == "" {}
来源：http://ijs.zhoulong.xyz

Ruby: if s.empty?
来源：http://fii.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://via.shzxlz.cn

[E21] 超长截断加省略号
来源：http://yof.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qtp.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ysn.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://laq.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tdl.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nub.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://ccy.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kdi.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://skd.yvedp.cn

[E22] 字节长度与字符长度
来源：http://dgw.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ipt.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mww.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpx.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://smh.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nfp.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmm.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://rpl.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cxl.jqgfzy.top

================================================================================
来源：http://wnb.ctjpmb.com

F. 文件与目录
来源：http://siv.chenjidiqi.icu

================================================================================
来源：http://bzg.gotoacloud.top

[F01] 读取整个文件
来源：http://qwo.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://imj.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://uth.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzd.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uwd.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mfb.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nkb.andypj.xyz

Ruby: File.read("a.txt")
来源：http://xow.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://lam.jqgfzy.top

[F02] 逐行读取文件
来源：http://gjs.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ghv.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lsi.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iub.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kux.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jbd.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bjj.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dmm.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zvn.tanke756.top

[F03] 写入文件（覆盖）
来源：http://nyz.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ktj.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://byf.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ros.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cow.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lha.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqa.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://swt.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eie.yvedp.cn

[F04] 追加写入文件
来源：http://jco.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pkc.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tvn.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://joq.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxk.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wyz.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://whq.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://apn.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rqv.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://aug.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tei.yj202588.top

PHP:  file_exists("a.txt");
来源：http://bbc.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://opd.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://qyu.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pdi.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rya.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://zdx.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://jlc.yangfankeji.com

[F06] 删除文件
来源：http://jdu.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://lmu.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://ttx.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://tce.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://jbv.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tlz.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://hhp.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://aqc.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://nba.nwbrower.top

[F07] 创建目录（含多级）
来源：http://xjd.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmu.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ilu.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sqo.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwt.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://epb.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pql.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tkn.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ztz.haohaochexian.top

[F08] 遍历目录
来源：http://zzt.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://avr.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wqw.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://mlq.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://ntz.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ika.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dxq.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://zaf.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://edc.316326.xyz

[F09] 获取文件大小
来源：http://thg.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://nyf.ydzc1.top

PHP:  filesize("a.txt");
来源：http://mbs.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://ylt.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://uia.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zje.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pxr.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://fcp.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://hns.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://spf.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jcx.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aoj.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gaf.sysykeji.top

TS:   path.extname("a.txt")
来源：http://nqb.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zpo.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pae.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oof.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tzw.gaohongyu789.top

[F11] 复制与移动文件
来源：http://udv.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xhu.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fgx.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pdn.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xlp.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://evu.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vfp.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xvl.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ovk.9152youxi.cn

[F12] CSV 读写
来源：http://gdf.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jyd.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://udw.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xqb.quarkkingdee.top

TS:   // 同上
来源：http://dbm.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hqb.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pwp.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rzs.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wdv.nanxuanxn.top

================================================================================
来源：http://tsu.vehdjk.com

G. 面向对象
来源：http://oqm.cdnleiting.top

================================================================================
来源：http://kws.gogol.net.cn

[G01] 定义类
来源：http://yaq.jyoumei.cn

Py:   class User: pass
来源：http://ysr.hnxiangtu.top

PHP:  class User {}
来源：http://orx.sjlbkw.cn

JS:   class User {}
来源：http://wds.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://xpa.quarkkingdee.top


<!-- 参考信息 -->