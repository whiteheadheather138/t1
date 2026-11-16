代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mob.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yod.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sfw.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://obb.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pxj.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://paa.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qfo.xinyue.icu

[D26] 数组转字符串
来源：http://wef.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://qmz.hfpthk.cn

PHP:  implode(", ", $arr);
来源：http://xcu.uphjek.com

JS:   arr.join(", ")
来源：http://qxa.zdqjudy.top

TS:   arr.join(", ")
来源：http://jej.0kj1m.cn

Java: String.join(", ", list)
来源：http://ffg.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://wup.aibaodan.cn

Ruby: arr.join(", ")
来源：http://htl.316326.xyz

C#:   string.Join(", ", list)
来源：http://frq.feifeiyinyue.top

================================================================================
来源：http://qcs.hcnkem.com

E. 字符串处理
来源：http://cjl.smart0.xyz

================================================================================
来源：http://non.mhx1999.top

[E01] 拼接字符串
来源：http://hrg.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bll.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bis.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://elj.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rve.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ssg.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nwv.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hzq.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oyo.jqgfzy.top

[E02] 重复字符串
来源：http://ewh.birdmap.top

Py:   "ab" * 3
来源：http://yhf.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://kfy.smart0.xyz

JS:   "ab".repeat(3)
来源：http://sfa.yvedp.cn

TS:   "ab".repeat(3)
来源：http://tjq.yuxming.cn

Java: "ab".repeat(3)
来源：http://car.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://gun.xylfe.cn

Ruby: "ab" * 3
来源：http://hea.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://azp.shanyushiyangtech.top

[E03] 截取子串
来源：http://buc.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pkh.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://asd.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pke.ydzc1.top

TS:   s.slice(1, 4)
来源：http://jxf.daria6918.cn

Java: s.substring(1, 4)
来源：http://ihk.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bfa.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://vtd.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://peu.pycfn.com

[E04] 查找子串位置
来源：http://bzu.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://fgl.meibo888.top

PHP:  strpos($s, "x");
来源：http://vih.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sdj.zdqjudy.top

TS:   s.indexOf("x")
来源：http://jzw.daxiang520.top

Java: s.indexOf("x")
来源：http://gyr.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://mmb.gogol.net.cn

Ruby: s.index("x")
来源：http://wlv.mhx1999.top

C#:   s.IndexOf("x")
来源：http://pjd.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://quz.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvb.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ovv.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cym.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zbm.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fvo.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xxw.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qdm.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://abn.ivvv.top

[E06] 替换子串
来源：http://gbe.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://poo.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://egn.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fsd.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://xuv.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngk.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qbw.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://exw.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://abt.wangdashe.top

[E07] 按分隔符拆分
来源：http://kte.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vnq.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bwu.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sfa.snrcjt.cn

TS:   s.split(",")
来源：http://fib.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fgf.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymm.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://ucg.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yan.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://squ.uphjek.com

Py:   ",".join(items)
来源：http://mnk.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://xxx.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://kiv.nwbrower.top

TS:   items.join(",")
来源：http://dan.tanke756.top

Java: String.join(",", items)
来源：http://yfa.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://vdl.wangdashe.top

Ruby: items.join(",")
来源：http://hxh.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://wtm.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://fjt.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pat.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zls.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://lkg.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://dqa.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://jjn.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vku.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://urx.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dmp.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://fhp.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fjt.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hfg.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://xnv.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://nyr.yuxming.cn

Java: String.format("%03d", 7)
来源：http://ehy.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ecy.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nje.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qoa.fengsongda.top

[E11] 反转字符串
来源：http://jvz.zhengqikj.top

Py:   s[::-1]
来源：http://rfn.shangyingyoupin.top

PHP:  strrev($s);
来源：http://bph.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://vyr.tarul.cn

TS:   [...s].reverse().join("")
来源：http://yqx.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fal.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://cdd.quarkkingdee.top

Ruby: s.reverse
来源：http://ewo.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oss.fzhhl.top

[E12] 统计某字符出现次数
来源：http://rvl.zhijiandao.cn

Py:   s.count("a")
来源：http://pkg.tanke756.top

PHP:  substr_count($s, "a");
来源：http://rbs.aizwys.cn

JS:   s.split("a").length - 1
来源：http://kmy.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://tok.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rfv.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://eez.ppjwa.cn

Ruby: s.count("a")
来源：http://gfj.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://eto.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://zfn.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://zng.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bel.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ovu.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gmp.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zzn.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://evh.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://psu.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zvy.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://nex.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hov.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nvu.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fht.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lkm.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://szp.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htb.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ikz.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://smu.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://uzo.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jvj.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fav.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://plx.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://shc.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nng.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tql.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ggp.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mci.vehdjk.com

[E16] 数字千分位
来源：http://ull.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://zvr.c1oappe.top

PHP:  number_format(1234567);
来源：http://nod.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://lnm.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kgd.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://krn.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wli.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rgn.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://vxe.cqqwz.cn

[E17] 首字母大写
来源：http://ddx.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://igx.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qzm.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://utm.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cee.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asy.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mqj.wangdashe.top

Ruby: s.capitalize
来源：http://otg.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://clv.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://wxf.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pui.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zsb.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aiu.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://osk.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qml.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kcr.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yyv.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nzc.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://opr.guannengcc.top

Py:   s.splitlines()
来源：http://dfc.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rjc.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://jsb.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://zxm.guannengcc.top

Java: s.lines().toList()
来源：http://wiy.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://zea.xuanzx.com

Ruby: s.lines
来源：http://gei.cqqwz.cn

C#:   s.Split('\n')
来源：http://bwk.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://evt.nanxuanxn.top

Py:   if not s:
来源：http://ykc.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nnj.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eix.jianghu66.top

TS:   if (s === "") {}
来源：http://ysg.sxryk.cn

Java: if (s.isEmpty()) {}
来源：http://die.vqdsnc.cn

Go:   if s == "" {}
来源：http://khy.uphjek.com

Ruby: if s.empty?
来源：http://rpu.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eji.xylfe.cn

[E21] 超长截断加省略号
来源：http://cei.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oom.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sqt.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://noj.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rmf.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tui.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://mgh.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gif.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aln.yonumen.top

[E22] 字节长度与字符长度
来源：http://mch.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xlo.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkc.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://woo.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcf.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eaa.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fge.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://kmd.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://stq.tian-w.cn

================================================================================
来源：http://ueq.hcnkem.com

F. 文件与目录
来源：http://jwh.yongpay.top

================================================================================
来源：http://pzc.yueranfly.top

[F01] 读取整个文件
来源：http://zhz.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uip.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://zpr.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ksx.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lri.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jxl.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://daq.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://hmx.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://tag.52xcode.cn

[F02] 逐行读取文件
来源：http://hqm.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lqr.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fap.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gau.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://haf.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yfh.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mxq.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocy.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zsd.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://pxj.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uau.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ixb.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://edq.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ntv.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kvf.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ydy.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://gnj.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrp.ivvv.top

[F04] 追加写入文件
来源：http://zum.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tud.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ses.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://usa.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbj.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dbs.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vyx.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zdo.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nvt.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://yzq.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yme.sweek.top

PHP:  file_exists("a.txt");
来源：http://nor.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://ict.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://hry.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://irr.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://flv.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://xlq.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://ckd.wangshuangyany.cn

[F06] 删除文件
来源：http://glq.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://wtv.tarul.cn

PHP:  unlink("a.txt");
来源：http://ujh.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://jkl.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://wro.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vem.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://zok.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://jby.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://sgo.redwolf501.top

[F07] 创建目录（含多级）
来源：http://pym.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kwt.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kzn.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lvd.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qaw.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rdo.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfj.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mwr.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sje.vehdjk.com

[F08] 遍历目录
来源：http://hym.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lqx.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nxm.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://pvy.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://xcy.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vue.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://clp.yongpay.top

Ruby: Dir.children("dir")
来源：http://iwf.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://eyo.cashguo.top

[F09] 获取文件大小
来源：http://jzk.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://ysw.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://msm.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://nxj.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://zdk.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://diy.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qxe.birdmap.top

Ruby: File.size("a.txt")
来源：http://dem.daria6918.cn


<!-- 参考信息 -->