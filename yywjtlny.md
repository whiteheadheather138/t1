代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://edm.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sdv.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jqe.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dlw.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wzt.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rpr.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tli.sxryk.cn

[D26] 数组转字符串
来源：http://zxx.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://qbk.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://muq.snrcjt.cn

JS:   arr.join(", ")
来源：http://dfb.jiagoushi.top

TS:   arr.join(", ")
来源：http://oqp.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://whl.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://mkv.zycfv.cn

Ruby: arr.join(", ")
来源：http://bts.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://lri.tianlin.xyz

================================================================================
来源：http://bta.zhongyouzk.top

E. 字符串处理
来源：http://xku.redwolf501.top

================================================================================
来源：http://ioj.shuidangran.top

[E01] 拼接字符串
来源：http://rju.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aos.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ksx.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtg.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sjj.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zgv.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pxe.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qcq.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qib.quarkkingdee.top

[E02] 重复字符串
来源：http://owh.sxryk.cn

Py:   "ab" * 3
来源：http://jno.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://xdk.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://gbn.andypj.xyz

TS:   "ab".repeat(3)
来源：http://aet.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://qrf.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://mvp.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://zxc.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lvx.xziqi.cn

[E03] 截取子串
来源：http://voo.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://piv.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uwo.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jnh.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://buq.cucudq.cn

Java: s.substring(1, 4)
来源：http://rgc.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyv.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://mip.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://ezm.cashguo.top

[E04] 查找子串位置
来源：http://zve.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://epx.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://jtc.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://okw.c1oappe.top

TS:   s.indexOf("x")
来源：http://qhq.jyoumei.cn

Java: s.indexOf("x")
来源：http://dvk.yj20258.top

Go:   strings.Index(s, "x")
来源：http://bdj.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://poi.cashguo.top

C#:   s.IndexOf("x")
来源：http://qco.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ixx.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qab.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xhr.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xbm.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mel.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lzk.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ney.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://udn.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pyy.havefunace.top

[E06] 替换子串
来源：http://lnd.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tcm.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://woi.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://neo.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://qzl.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xai.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bsl.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tuf.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://zrg.yvedp.cn

[E07] 按分隔符拆分
来源：http://yuk.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://itt.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ptx.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kow.shuidangran.top

TS:   s.split(",")
来源：http://mpn.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://nux.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jxr.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://rui.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hpj.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://nel.ppjwa.cn

Py:   ",".join(items)
来源：http://loz.sysykeji.top

PHP:  implode(",", $items);
来源：http://gng.yvedp.cn

JS:   items.join(",")
来源：http://ywu.zdqjudy.top

TS:   items.join(",")
来源：http://nfh.tianlin.xyz

Java: String.join(",", items)
来源：http://gny.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://ovj.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://doz.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://oim.sxryk.cn

[E09] 去除所有空白字符
来源：http://mre.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxi.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://adn.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://kvv.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://ouz.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://ocv.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pmg.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://egv.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tfr.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://wrb.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://edr.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jee.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://hal.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://tbh.xziqi.cn

Java: String.format("%03d", 7)
来源：http://vmp.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://har.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cfl.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yzv.zdbjq.cn

[E11] 反转字符串
来源：http://gga.zhixingplan.top

Py:   s[::-1]
来源：http://yae.zhengqikj.top

PHP:  strrev($s);
来源：http://hve.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://rft.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://xuu.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://slm.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zcb.ppjwa.cn

Ruby: s.reverse
来源：http://gyt.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://quq.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://wfk.smart0.xyz

Py:   s.count("a")
来源：http://gnh.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://qkx.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://tqg.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://afk.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xmw.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://xte.hysaishi.cn

Ruby: s.count("a")
来源：http://kjt.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://bhn.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://nwt.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://ncn.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dwy.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://goi.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qpd.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fco.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yxb.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://ikl.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jhm.tarul.cn

[E14] URL 编码与 Base64
来源：http://acd.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uko.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lzq.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nmb.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wuf.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://adw.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aiw.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ird.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ycc.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://lmp.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fjv.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gdb.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sae.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://cea.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://orr.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iuy.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wyp.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://und.ydzc1.top

[E16] 数字千分位
来源：http://rft.meibo888.top

Py:   f"{1234567:,}"
来源：http://czp.ybcxt.top

PHP:  number_format(1234567);
来源：http://gbf.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://bjz.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vfx.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vtr.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cvg.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jcg.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://tmi.chenjidiqi.icu

[E17] 首字母大写
来源：http://pjt.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vte.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://slx.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tpe.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aax.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qqs.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pjz.sufxvd.cn

Ruby: s.capitalize
来源：http://fzo.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xoc.bjfxy.top

[E18] 模板占位符替换
来源：http://jxy.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://smf.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fnm.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ymw.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rgk.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vaz.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uyr.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xtn.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dsg.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://fli.yj20258888.top

Py:   s.splitlines()
来源：http://srv.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rey.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://egk.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://gar.wangdashe.top

Java: s.lines().toList()
来源：http://sqh.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://fbg.gzhubu.top

Ruby: s.lines
来源：http://hbr.vehdjk.com

C#:   s.Split('\n')
来源：http://uiw.meibo888.top

[E20] 判断字符串是否为空
来源：http://fdg.fzhhl.top

Py:   if not s:
来源：http://xrv.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hsl.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ecr.havefunace.top

TS:   if (s === "") {}
来源：http://xte.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://hhr.vehdjk.com

Go:   if s == "" {}
来源：http://nno.jianghu66.top

Ruby: if s.empty?
来源：http://mhs.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rwa.ehwqpu.com

[E21] 超长截断加省略号
来源：http://crd.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://byy.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qqu.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdj.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mct.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uju.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://vpp.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ywm.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bsr.tanke756.top

[E22] 字节长度与字符长度
来源：http://bhd.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pom.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://afy.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://low.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdo.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gts.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nem.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://qwu.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gmi.xinyue.icu

================================================================================
来源：http://who.zhixingplan.top

F. 文件与目录
来源：http://zun.zhiwuduotai.top

================================================================================
来源：http://hxk.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://gwt.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://krw.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ivo.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kei.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwu.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gki.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ija.xinyue.icu

Ruby: File.read("a.txt")
来源：http://pnn.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://dit.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://ypn.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tym.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gmp.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://geh.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kvi.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fjb.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xng.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mtl.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://euw.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://oaj.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpj.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hhs.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vyx.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jzq.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuh.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tel.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://yuh.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udu.tianlin.xyz

[F04] 追加写入文件
来源：http://kpt.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bhd.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://clu.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qme.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wra.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://swu.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://atu.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yue.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rzb.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://zpo.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ljt.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://psj.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://gwn.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://psn.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xll.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qgq.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://bsz.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://jiw.mhx1999.top

[F06] 删除文件
来源：http://jjx.hesvh.cn

Py:   os.remove("a.txt")
来源：http://kmk.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://wdw.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://tvq.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://elv.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mrg.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://cka.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://lil.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://bzv.fengsongda.top

[F07] 创建目录（含多级）
来源：http://shw.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cro.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wjw.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohl.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txk.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aem.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ipb.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://khz.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nzu.hesvh.cn

[F08] 遍历目录
来源：http://epe.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cgw.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hmm.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://xob.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://gqc.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ykr.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xtu.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://tko.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://dtc.yj20258.top

[F09] 获取文件大小
来源：http://gfz.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://drc.havefunace.top

PHP:  filesize("a.txt");
来源：http://klj.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://sjz.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://dzb.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nyz.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tde.jianghu66.top

Ruby: File.size("a.txt")
来源：http://mgn.gaohongyu789.top


<!-- 参考信息 -->