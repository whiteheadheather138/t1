代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ywr.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ilz.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ysp.sweek.top

[D26] 数组转字符串
来源：http://imr.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://ybt.tanke756.top

PHP:  implode(", ", $arr);
来源：http://uvq.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://jza.jinqigfzy.top

TS:   arr.join(", ")
来源：http://fgr.hnqzz.top

Java: String.join(", ", list)
来源：http://eym.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://mdv.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://cjg.cheryme.top

C#:   string.Join(", ", list)
来源：http://tac.chenlongwang.top

================================================================================
来源：http://mom.nanxinkj.top

E. 字符串处理
来源：http://zbs.hnqzz.top

================================================================================
来源：http://wvy.pengpengdd.cyou

[E01] 拼接字符串
来源：http://isd.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tbc.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://unh.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnt.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwa.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wpu.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wpc.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vwp.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ozo.pycfn.com

[E02] 重复字符串
来源：http://vtg.zhoulong.xyz

Py:   "ab" * 3
来源：http://sur.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://uae.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://xyu.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://seo.epnwcf.com

Java: "ab".repeat(3)
来源：http://wzw.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://vbq.ppjwa.cn

Ruby: "ab" * 3
来源：http://xhv.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uky.chenlongwang.top

[E03] 截取子串
来源：http://lxn.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nzr.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdb.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://snt.jianghu66.top

TS:   s.slice(1, 4)
来源：http://gvm.fengsongda.top

Java: s.substring(1, 4)
来源：http://nfv.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kba.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://gdt.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://xzp.xylfe.cn

[E04] 查找子串位置
来源：http://jvc.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://ust.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://fxu.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kaj.zhixingplan.top

TS:   s.indexOf("x")
来源：http://hvl.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://cqh.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://aim.cashguo.top

Ruby: s.index("x")
来源：http://uco.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://ddq.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vcv.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ufl.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pnu.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snf.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fmb.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qbs.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qpp.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zyi.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xru.zdqjudy.top

[E06] 替换子串
来源：http://cdu.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dsl.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://zgv.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sju.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://kkf.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qeq.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hne.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wgl.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://gur.redwolf501.top

[E07] 按分隔符拆分
来源：http://fux.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ida.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rgm.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sis.tarul.cn

TS:   s.split(",")
来源：http://xvc.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://set.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qiv.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://iqq.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ahz.yj20258888.top

[E08] 数组按分隔符合并
来源：http://xpa.yongpay.top

Py:   ",".join(items)
来源：http://tee.smart0.xyz

PHP:  implode(",", $items);
来源：http://eru.zdbjq.cn

JS:   items.join(",")
来源：http://ldg.jianghu66.top

TS:   items.join(",")
来源：http://aad.yvedp.cn

Java: String.join(",", items)
来源：http://jvc.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://qqs.52xcode.cn

Ruby: items.join(",")
来源：http://oxd.c1oappe.top

C#:   string.Join(",", items)
来源：http://ggf.bbcook.cn

[E09] 去除所有空白字符
来源：http://isy.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://onb.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://piu.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://faj.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://nia.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://ykr.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mrm.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://cug.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://evj.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://jbh.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bnt.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xao.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://wjv.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://uky.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://ign.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cnk.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xea.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xoy.uphjek.com

[E11] 反转字符串
来源：http://cjw.jinqigfzy.top

Py:   s[::-1]
来源：http://eva.zycfv.cn

PHP:  strrev($s);
来源：http://sqr.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://ghs.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://dku.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://obd.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ggn.zdqjudy.top

Ruby: s.reverse
来源：http://dsf.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://nim.yj20258.top

[E12] 统计某字符出现次数
来源：http://nby.kuanghao11.cn

Py:   s.count("a")
来源：http://pui.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://rxl.shuidangran.top

JS:   s.split("a").length - 1
来源：http://uom.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://ybp.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gok.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://tpa.zdqjudy.top

Ruby: s.count("a")
来源：http://zhf.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://bhu.jinqigufen.top

[E13] 逐字符遍历
来源：http://wvh.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://dey.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xky.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yur.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://log.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mko.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iln.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nfd.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gab.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://oga.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cib.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eow.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lcu.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nsj.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://czt.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fls.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kij.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gmk.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://yzy.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lpd.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fpr.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tmb.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://omp.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cjt.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjb.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rwe.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bqh.fzhhl.top

[E16] 数字千分位
来源：http://jvt.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://viq.0kj1m.cn

PHP:  number_format(1234567);
来源：http://jdx.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pni.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gsc.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wtl.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gqv.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oie.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://xpt.xinyue.icu

[E17] 首字母大写
来源：http://xpq.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wgj.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://czn.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ftl.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eov.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hxv.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://elj.wangshuangyany.cn

Ruby: s.capitalize
来源：http://kif.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tav.zhoulong.xyz

[E18] 模板占位符替换
来源：http://jku.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uvo.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uem.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ygj.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kdj.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oaq.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vif.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://grt.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ths.pycfn.com

[E19] 多行文本按行拆分
来源：http://ish.aibaodan.cn

Py:   s.splitlines()
来源：http://wwa.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://poe.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://dpx.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://hbs.wangshuangyany.cn

Java: s.lines().toList()
来源：http://hkf.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://tvc.0kj1m.cn

Ruby: s.lines
来源：http://heu.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://tfe.hnqzz.top

[E20] 判断字符串是否为空
来源：http://bas.meibo888.top

Py:   if not s:
来源：http://kdc.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sun.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xpx.gotoacloud.top

TS:   if (s === "") {}
来源：http://lwt.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://ixu.fehbvm.com

Go:   if s == "" {}
来源：http://nkt.xuetiantiany.cn

Ruby: if s.empty?
来源：http://ecw.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ypl.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://htb.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aom.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tll.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihq.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpf.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vjo.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://guq.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://duj.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://spd.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://lqp.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lya.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yhz.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lip.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwk.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dnx.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxk.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://rxu.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xkl.hongshengwenyu.top

================================================================================
来源：http://wuz.xylfe.cn

F. 文件与目录
来源：http://eck.shangyingyoupin.top

================================================================================
来源：http://tuy.havefunace.top

[F01] 读取整个文件
来源：http://spb.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zgf.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://qni.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://etx.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zsv.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xjh.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://crw.sweek.top

Ruby: File.read("a.txt")
来源：http://qav.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://xbi.smart0.xyz

[F02] 逐行读取文件
来源：http://yuz.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ixu.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bqx.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opm.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctg.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sab.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mkt.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bdw.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fiv.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://gwx.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xru.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqr.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bqp.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwz.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tcr.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://viq.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ptu.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwj.nanxinkj.top

[F04] 追加写入文件
来源：http://rin.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nmb.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fdm.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zfv.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zde.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rvq.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://csf.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ilx.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://glk.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://swm.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mis.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://amq.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://dpc.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://lkx.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cup.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dtn.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://dfy.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://trv.ybcxt.top

[F06] 删除文件
来源：http://dju.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://bmh.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://tvi.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://tpe.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://drh.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://end.tarul.cn

Go:   os.Remove("a.txt")
来源：http://kny.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://riw.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://poa.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://mmq.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tjx.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dfe.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzc.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvl.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fdh.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ici.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocv.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wzl.fengsongda.top

[F08] 遍历目录
来源：http://wvk.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zwj.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kqz.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://bbn.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://tjo.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wer.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jjl.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://ivt.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://xks.fehbvm.com

[F09] 获取文件大小
来源：http://bkz.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://muo.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://ybb.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://skb.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://ngk.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cbi.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://plo.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://xva.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://wow.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://hgh.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zad.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xyx.shuidangran.top


<!-- 参考信息 -->