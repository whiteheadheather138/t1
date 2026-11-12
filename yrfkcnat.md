代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mxi.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wfb.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://pke.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zfn.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tbl.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iws.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xyi.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rhg.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rry.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sls.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://efc.aizwys.cn

[D26] 数组转字符串
来源：http://fqe.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://qlc.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://yim.uphjek.com

JS:   arr.join(", ")
来源：http://udz.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://iel.9152youxi.cn

Java: String.join(", ", list)
来源：http://ycy.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://rwv.hywenlv.cn

Ruby: arr.join(", ")
来源：http://hjp.yonumen.top

C#:   string.Join(", ", list)
来源：http://srz.sufxvd.cn

================================================================================
来源：http://jcm.vqdsnc.cn

E. 字符串处理
来源：http://paa.jinqigfzy.top

================================================================================
来源：http://twu.tianlin.xyz

[E01] 拼接字符串
来源：http://xno.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bro.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysl.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wau.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hbf.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dwt.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ueh.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hpt.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xmf.epnwcf.com

[E02] 重复字符串
来源：http://sqf.tanke756.top

Py:   "ab" * 3
来源：http://blh.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://wmn.jianghu66.top

JS:   "ab".repeat(3)
来源：http://fey.cashguo.top

TS:   "ab".repeat(3)
来源：http://eqh.jiagoushi.top

Java: "ab".repeat(3)
来源：http://dge.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://bcn.yonumen.top

Ruby: "ab" * 3
来源：http://tsv.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zql.hysaishi.cn

[E03] 截取子串
来源：http://yqa.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://skj.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xwv.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kvr.jianghu66.top

TS:   s.slice(1, 4)
来源：http://pci.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://gvl.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yov.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://ygq.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://bgm.hnxiangtu.top

[E04] 查找子串位置
来源：http://axe.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://sxi.cucudq.cn

PHP:  strpos($s, "x");
来源：http://eke.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://llw.cqqwz.cn

TS:   s.indexOf("x")
来源：http://rof.jianghu66.top

Java: s.indexOf("x")
来源：http://qpb.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://vpi.yueranfly.top

Ruby: s.index("x")
来源：http://kww.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://six.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yih.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rub.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vll.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eed.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qmy.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tti.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ooq.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ola.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sjs.ehwqpu.com

[E06] 替换子串
来源：http://xvs.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pjh.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://rmn.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vel.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://caj.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfs.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mdy.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mnq.havefunace.top

C#:   s.Replace("a", "b")
来源：http://xzz.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://aey.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvk.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eon.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rjn.yuanzhike.top

TS:   s.split(",")
来源：http://opq.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ljg.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxu.hammf.cn

Ruby: s.split(",");  s.split
来源：http://cfk.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://omh.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://lfl.tian-w.cn

Py:   ",".join(items)
来源：http://bmh.mhx1999.top

PHP:  implode(",", $items);
来源：http://uym.zycfv.cn

JS:   items.join(",")
来源：http://klp.sweek.top

TS:   items.join(",")
来源：http://pph.bbcook.cn

Java: String.join(",", items)
来源：http://iqq.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://ezu.jinqigfzy.top

Ruby: items.join(",")
来源：http://abz.cdnleiting.top

C#:   string.Join(",", items)
来源：http://ytf.bbcook.cn

[E09] 去除所有空白字符
来源：http://vtu.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cot.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zhm.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ttq.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://bmr.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://gzd.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rds.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://ppj.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rqw.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://nvh.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ojj.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rgt.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://wlx.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://spu.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://lhi.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://siu.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ykh.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ioh.yvedp.cn

[E11] 反转字符串
来源：http://lge.jqgufenzy.top

Py:   s[::-1]
来源：http://quw.xziqi.cn

PHP:  strrev($s);
来源：http://vdm.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://rff.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://awa.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zjl.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zto.hysaishi.cn

Ruby: s.reverse
来源：http://ldm.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://prj.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://lsj.dashuyun.cn

Py:   s.count("a")
来源：http://ays.yj20258.top

PHP:  substr_count($s, "a");
来源：http://tht.fengsongda.top

JS:   s.split("a").length - 1
来源：http://hdx.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://kpi.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jpb.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://rti.hysaishi.cn

Ruby: s.count("a")
来源：http://plc.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://jpa.guowangkeji.top

[E13] 逐字符遍历
来源：http://wme.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://tjz.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://seb.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oah.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vno.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ffl.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jth.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gdc.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btr.sxryk.cn

[E14] URL 编码与 Base64
来源：http://bkz.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oby.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tjz.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oaz.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kjn.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xvw.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gla.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gxy.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hwp.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://sjd.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jda.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://shq.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://guk.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wwo.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://shi.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ufq.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ijy.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://poc.cashguo.top

[E16] 数字千分位
来源：http://skc.vehdjk.com

Py:   f"{1234567:,}"
来源：http://gln.aizwys.cn

PHP:  number_format(1234567);
来源：http://ssu.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wgb.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bbn.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dib.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pbs.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://due.hammf.cn

C#:   1234567.ToString("N0")
来源：http://ssp.pycfn.com

[E17] 首字母大写
来源：http://nxd.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nxw.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gmw.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uow.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dyf.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://syq.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xuy.cashguo.top

Ruby: s.capitalize
来源：http://fov.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vss.smart0.xyz

[E18] 模板占位符替换
来源：http://rnd.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yja.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kpi.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://exr.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wpf.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgl.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hyd.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cpt.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mtj.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://zwj.ehwqpu.com

Py:   s.splitlines()
来源：http://toh.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fcq.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://eta.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://epr.ybcxt.top

Java: s.lines().toList()
来源：http://bux.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://uro.gzhubu.top

Ruby: s.lines
来源：http://jig.zdqjudy.top

C#:   s.Split('\n')
来源：http://nme.smart0.xyz

[E20] 判断字符串是否为空
来源：http://vig.andypj.xyz

Py:   if not s:
来源：http://clv.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://icj.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://prn.yongpay.top

TS:   if (s === "") {}
来源：http://bfv.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://gca.jqgfzy.top

Go:   if s == "" {}
来源：http://dnd.zhixingplan.top

Ruby: if s.empty?
来源：http://zfw.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ais.tian-w.cn

[E21] 超长截断加省略号
来源：http://bsx.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uwv.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhi.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://plw.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yux.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ebo.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://nhd.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lln.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zte.shuidangran.top

[E22] 字节长度与字符长度
来源：http://hhq.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://imb.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwh.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ysf.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dem.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://osu.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fez.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://pvo.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://laj.guowangkeji.top

================================================================================
来源：http://wse.dashuyun.cn

F. 文件与目录
来源：http://ybg.zdbjq.cn

================================================================================
来源：http://tmt.gotoacloud.top

[F01] 读取整个文件
来源：http://fqn.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewu.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://xgh.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mkp.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ovs.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lbs.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nat.sxryk.cn

Ruby: File.read("a.txt")
来源：http://zyi.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://hvf.ybcxt.top

[F02] 逐行读取文件
来源：http://pue.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bka.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jeu.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aft.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sre.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fjp.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ree.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ein.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgr.meibo888.top

[F03] 写入文件（覆盖）
来源：http://zkp.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pan.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbw.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://utq.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wcn.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pqk.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rpw.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://tbh.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://chv.xinyue.icu

[F04] 追加写入文件
来源：http://jkf.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ibh.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpw.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zlg.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pym.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uvz.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lrc.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pfz.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ncf.redwolf501.top

[F05] 判断文件或目录是否存在
来源：http://fgk.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ayc.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://bvx.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://kif.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://mdb.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://usf.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jrp.sweek.top

Ruby: File.exist?("a.txt")
来源：http://npi.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://nip.zdbjq.cn

[F06] 删除文件
来源：http://fgt.yj20258888.top

Py:   os.remove("a.txt")
来源：http://upd.wangdashe.top

PHP:  unlink("a.txt");
来源：http://lyx.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zxe.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://fwg.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vks.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://axm.sweek.top

Ruby: File.delete("a.txt")
来源：http://jum.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://mue.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://avq.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pwt.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xwh.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ewi.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shx.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xyb.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bod.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mdp.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hjm.hongshengwenyu.top

[F08] 遍历目录
来源：http://pjn.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwr.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bzk.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://mon.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://ibx.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yfq.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lxw.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://ggd.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://rov.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://mqd.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://oer.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://tlj.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://gkw.yuxming.cn


<!-- 参考信息 -->