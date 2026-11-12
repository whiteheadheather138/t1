代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://olb.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ysr.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zbi.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://otf.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tjo.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hlh.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mpu.nanxinkj.top

[D26] 数组转字符串
来源：http://ixp.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://gtt.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://hcv.fktsv.cn

JS:   arr.join(", ")
来源：http://ynq.cucudq.cn

TS:   arr.join(", ")
来源：http://iuc.svipenyu.cn

Java: String.join(", ", list)
来源：http://ppy.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://set.jianghu66.top

Ruby: arr.join(", ")
来源：http://imk.cucudq.cn

C#:   string.Join(", ", list)
来源：http://mag.smart0.xyz

================================================================================
来源：http://smw.zhaomingkeji.xyz

E. 字符串处理
来源：http://hqh.jiagoushi.top

================================================================================
来源：http://jqw.gzhubu.top

[E01] 拼接字符串
来源：http://tty.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xqr.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjv.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kth.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fik.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zff.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bnf.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vol.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rgz.0kj1m.cn

[E02] 重复字符串
来源：http://zjx.ivvv.top

Py:   "ab" * 3
来源：http://nhp.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://hat.cucudq.cn

JS:   "ab".repeat(3)
来源：http://krv.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://rdk.cheryme.top

Java: "ab".repeat(3)
来源：http://oui.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://rbm.ydjk.org.cn

Ruby: "ab" * 3
来源：http://pog.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hfg.bjfxy.top

[E03] 截取子串
来源：http://ytg.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pro.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jcq.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nnh.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://ayw.jyoumei.cn

Java: s.substring(1, 4)
来源：http://mzw.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ngh.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://kda.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://ivi.fengsongda.top

[E04] 查找子串位置
来源：http://vog.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://dme.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://qhq.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ztq.dianchejie.cn

TS:   s.indexOf("x")
来源：http://zrj.jiagoushi.top

Java: s.indexOf("x")
来源：http://mxa.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://hew.jyoumei.cn

Ruby: s.index("x")
来源：http://yvd.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://vqu.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tuh.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ukq.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bwz.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://int.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gus.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivy.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fyz.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wpf.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pjy.fzhhl.top

[E06] 替换子串
来源：http://amj.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pbi.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://wzg.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysf.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://ptl.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kwn.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://beh.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zbz.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://aat.haohaochexian.top

[E07] 按分隔符拆分
来源：http://zcq.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hoa.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ykh.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkw.jinghuilouyu.cn

TS:   s.split(",")
来源：http://mka.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://zpp.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lxh.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://uhl.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dbc.yfazqb.com

[E08] 数组按分隔符合并
来源：http://uzp.ivvv.top

Py:   ",".join(items)
来源：http://tbp.zdqjudy.top

PHP:  implode(",", $items);
来源：http://cic.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://bmp.shzxlz.cn

TS:   items.join(",")
来源：http://ahc.cashguo.top

Java: String.join(",", items)
来源：http://ras.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://lks.ctjpmb.com

Ruby: items.join(",")
来源：http://ptm.jyoumei.cn

C#:   string.Join(",", items)
来源：http://xpl.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://vyi.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kee.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wzo.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://zlo.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://lyh.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://zbd.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nfi.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://mln.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yed.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://ssu.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ibm.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kfp.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://new.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://aaz.yj202588.top

Java: String.format("%03d", 7)
来源：http://hig.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjp.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wxn.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tvo.ivvv.top

[E11] 反转字符串
来源：http://kds.yvedp.cn

Py:   s[::-1]
来源：http://xdw.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://ftg.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://gbt.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://lvu.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://bar.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yux.xziqi.cn

Ruby: s.reverse
来源：http://yqv.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ssu.nwbrower.top

[E12] 统计某字符出现次数
来源：http://rwv.yj20258.top

Py:   s.count("a")
来源：http://cyj.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://anc.aizwys.cn

JS:   s.split("a").length - 1
来源：http://xxr.yueranfly.top

TS:   s.split("a").length - 1
来源：http://ivx.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uzu.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://lpw.aibaodan.cn

Ruby: s.count("a")
来源：http://qey.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://nzi.yangfankeji.com

[E13] 逐字符遍历
来源：http://wzi.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://dpv.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vuq.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://btl.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cns.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sxf.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zuo.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://vqd.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wdz.meibo888.top

[E14] URL 编码与 Base64
来源：http://fli.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hrp.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://pjq.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ydb.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhd.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://syx.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hlx.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://klq.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vtq.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://lmh.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://odi.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eev.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgw.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://naw.c1oappe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yyr.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ugs.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yyb.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tqp.daria6918.cn

[E16] 数字千分位
来源：http://gpc.xuanzx.com

Py:   f"{1234567:,}"
来源：http://wtc.xinyue.icu

PHP:  number_format(1234567);
来源：http://tie.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rqy.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rgq.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://flt.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eqe.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ohk.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://uht.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://ggx.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blh.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://alw.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://acz.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://glp.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kqf.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vco.jyoumei.cn

Ruby: s.capitalize
来源：http://rcx.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uha.chenlongwang.top

[E18] 模板占位符替换
来源：http://fqk.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://exq.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ymc.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qls.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uzw.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lto.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iab.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://srw.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vou.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://hpq.ydjk.org.cn

Py:   s.splitlines()
来源：http://duv.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pnw.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://gom.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://nez.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://gxd.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://hvs.aibaodan.cn

Ruby: s.lines
来源：http://exz.uphjek.com

C#:   s.Split('\n')
来源：http://cza.yuxming.cn

[E20] 判断字符串是否为空
来源：http://hgs.shuidangran.top

Py:   if not s:
来源：http://qik.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lwm.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lvj.gogol.net.cn

TS:   if (s === "") {}
来源：http://bfe.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://jzg.zdbjq.cn

Go:   if s == "" {}
来源：http://hxk.sweek.top

Ruby: if s.empty?
来源：http://pwb.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ott.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://azz.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ypr.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpc.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zma.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nmc.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pkh.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://axa.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ggj.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lna.jianghu66.top

[E22] 字节长度与字符长度
来源：http://soi.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://atu.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmf.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://twt.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipm.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://crr.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rxd.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://hab.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pep.yonumen.top

================================================================================
来源：http://puv.sufxvd.cn

F. 文件与目录
来源：http://qke.nwbrower.top

================================================================================
来源：http://tag.redwolf501.top

[F01] 读取整个文件
来源：http://bma.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zum.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://wtx.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pzg.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://axd.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wpa.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eoj.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://bwq.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://liz.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://ppn.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pyj.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cxm.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrf.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aqm.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yso.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kee.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://krn.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xlp.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://tgg.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xni.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mrj.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jiw.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ybt.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://drm.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zgj.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://lyl.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xmg.nanxuanxn.top

[F04] 追加写入文件
来源：http://omm.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cuk.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ecj.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lek.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eef.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bjy.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bkg.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hkw.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zxa.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://iqi.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://swg.pycfn.com

PHP:  file_exists("a.txt");
来源：http://bfs.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://zcg.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://nmc.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://anc.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://axj.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://fbn.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://bcy.zhijiandao.cn

[F06] 删除文件
来源：http://uuu.sxryk.cn

Py:   os.remove("a.txt")
来源：http://sje.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://tud.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://igx.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://ecf.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tjv.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://vlq.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://stl.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://gmm.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://dqk.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oei.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rmw.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cyb.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enp.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ofb.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xok.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://drl.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oih.hfpthk.cn

[F08] 遍历目录
来源：http://yxs.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zgh.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bme.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://cwq.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://yom.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xmx.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cpz.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://uku.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://toj.xuanzx.com

[F09] 获取文件大小
来源：http://yjb.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://rsb.fktsv.cn

PHP:  filesize("a.txt");
来源：http://gpb.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://zen.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://yiw.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://dbn.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zlj.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://gnt.jiagoushi.top


<!-- 参考信息 -->