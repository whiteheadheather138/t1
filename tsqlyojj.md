代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ikq.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://amp.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://qir.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ndt.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ezr.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yvt.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pex.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://puj.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pnm.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ovk.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yfu.0kj1m.cn

[D26] 数组转字符串
来源：http://bcs.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://boa.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://bfj.zhongyouzk.top

JS:   arr.join(", ")
来源：http://ebk.tian-w.cn

TS:   arr.join(", ")
来源：http://mac.cucudq.cn

Java: String.join(", ", list)
来源：http://ftz.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://mtb.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://ilg.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://fre.xingfuxueyuan.xyz

================================================================================
来源：http://kmt.chenlongwang.top

E. 字符串处理
来源：http://bge.hnqzz.top

================================================================================
来源：http://tqe.kuanghao11.cn

[E01] 拼接字符串
来源：http://ddu.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hts.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://epy.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://idj.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jba.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bcp.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rhe.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qpg.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hrm.ydzc1.top

[E02] 重复字符串
来源：http://gds.sufxvd.cn

Py:   "ab" * 3
来源：http://gew.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://gjv.zycfv.cn

JS:   "ab".repeat(3)
来源：http://ksj.pycfn.com

TS:   "ab".repeat(3)
来源：http://edb.cheryme.top

Java: "ab".repeat(3)
来源：http://wdh.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://nok.xziqi.cn

Ruby: "ab" * 3
来源：http://ttq.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vge.fengsongda.top

[E03] 截取子串
来源：http://jbm.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nun.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gsl.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://snr.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://fhh.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://nmj.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://csj.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://tla.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://riw.fzhhl.top

[E04] 查找子串位置
来源：http://pgx.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://idi.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://bgs.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbq.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://mxo.yangfankeji.com

Java: s.indexOf("x")
来源：http://zpq.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://tfn.fengsongda.top

Ruby: s.index("x")
来源：http://qio.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://kuo.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://brr.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uqj.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jvw.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ohz.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gsp.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://alw.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hel.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fvm.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oad.fktsv.cn

[E06] 替换子串
来源：http://uug.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgd.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://khb.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://epp.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://riu.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxx.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lqr.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hkz.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://uik.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://yvn.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aeb.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vml.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rdd.fengsongda.top

TS:   s.split(",")
来源：http://zpl.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sfs.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yiv.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://ffj.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qot.epnwcf.com

[E08] 数组按分隔符合并
来源：http://hih.hnxiangtu.top

Py:   ",".join(items)
来源：http://ffh.iojbl.cn

PHP:  implode(",", $items);
来源：http://ooe.fktsv.cn

JS:   items.join(",")
来源：http://kjx.kuanghao11.cn

TS:   items.join(",")
来源：http://lmi.bjfxy.top

Java: String.join(",", items)
来源：http://wog.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://utv.yonumen.top

Ruby: items.join(",")
来源：http://syn.xuanzx.com

C#:   string.Join(",", items)
来源：http://wvs.cashguo.top

[E09] 去除所有空白字符
来源：http://pvm.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rix.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://knj.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://rwo.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://usy.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://tod.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uza.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vxg.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqa.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://mlg.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yxk.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rtf.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://krb.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://jyl.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://pmq.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fot.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxi.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fan.sweek.top

[E11] 反转字符串
来源：http://mxn.zdqjudy.top

Py:   s[::-1]
来源：http://ilo.chenjidiqi.icu

PHP:  strrev($s);
来源：http://izc.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://wjy.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://yok.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ame.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://krm.52xcode.cn

Ruby: s.reverse
来源：http://kba.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://vhp.gzhubu.top

[E12] 统计某字符出现次数
来源：http://wnq.cdnleiting.top

Py:   s.count("a")
来源：http://fcc.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://bsg.yj20258.top

JS:   s.split("a").length - 1
来源：http://rih.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://sdv.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zur.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://bth.shzxlz.cn

Ruby: s.count("a")
来源：http://vhd.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://sjh.chenzaomai.com

[E13] 逐字符遍历
来源：http://ihe.hammf.cn

Py:   for ch in s: print(ch)
来源：http://jmh.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aol.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ykl.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gpc.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mqw.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tbv.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mfr.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ohh.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://scs.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rsl.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dib.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rlt.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iws.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oqm.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pew.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://saw.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tmc.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://rsz.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bim.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vrk.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mre.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pps.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tuw.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://osj.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hta.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bxf.redwolf501.top

[E16] 数字千分位
来源：http://lvu.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://fhj.tian-w.cn

PHP:  number_format(1234567);
来源：http://kxw.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kcv.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tbb.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wak.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gfn.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xlb.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://xug.yj20258888.top

[E17] 首字母大写
来源：http://eka.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rcg.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://sql.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://alg.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ege.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rrh.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cqe.fengsongda.top

Ruby: s.capitalize
来源：http://xac.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://scy.ydjk.org.cn

[E18] 模板占位符替换
来源：http://ydf.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fwu.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://htb.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zuz.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://arl.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gyg.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wwz.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kwl.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dtj.xziqi.cn

[E19] 多行文本按行拆分
来源：http://jah.hammf.cn

Py:   s.splitlines()
来源：http://dtc.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nkx.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://bdt.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://pwf.smart0.xyz

Java: s.lines().toList()
来源：http://vzx.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://zyc.sufxvd.cn

Ruby: s.lines
来源：http://imf.smart0.xyz

C#:   s.Split('\n')
来源：http://yff.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://jok.vehdjk.com

Py:   if not s:
来源：http://dep.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gkg.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ore.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://erm.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://lfi.pycfn.com

Go:   if s == "" {}
来源：http://jjl.sjlbkw.cn

Ruby: if s.empty?
来源：http://hoy.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wlc.gzhubu.top

[E21] 超长截断加省略号
来源：http://mzc.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lmw.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ocu.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rai.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpe.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zeb.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://pxo.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ncr.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hft.hesvh.cn

[E22] 字节长度与字符长度
来源：http://wdl.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tsa.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mqn.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kpb.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://duh.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aux.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://npi.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://wxz.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kin.ivvv.top

================================================================================
来源：http://ksd.52xcode.cn

F. 文件与目录
来源：http://lmn.gzhubu.top

================================================================================
来源：http://qjx.zdbjq.cn

[F01] 读取整个文件
来源：http://glv.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hnt.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://nbj.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sqs.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://shv.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://slk.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ozz.aizwys.cn

Ruby: File.read("a.txt")
来源：http://vyf.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://hgt.tian-w.cn

[F02] 逐行读取文件
来源：http://hhi.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hsc.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dbb.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nmz.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ycv.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vys.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://viq.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xol.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hgc.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://ubs.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gib.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yql.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqe.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ebr.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmb.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://odl.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://jff.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://msp.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://xup.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oaf.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fvp.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sna.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lub.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uwp.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lrw.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jlt.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ycy.sweek.top

[F05] 判断文件或目录是否存在
来源：http://ktq.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yki.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://diz.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://ohm.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://asb.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://tdp.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xab.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://etu.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://jvk.xuetiantiany.cn

[F06] 删除文件
来源：http://hbs.wangdashe.top

Py:   os.remove("a.txt")
来源：http://kjq.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://gra.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://ejy.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://iev.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kmw.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://pxf.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://rlw.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://rag.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://ype.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bth.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uch.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://anv.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://onh.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jfr.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ujt.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ssg.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ysp.316326.xyz

[F08] 遍历目录
来源：http://jay.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hxz.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dpa.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://syb.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://ewh.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yxi.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jwl.hammf.cn

Ruby: Dir.children("dir")
来源：http://ekc.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://geo.feifeiyinyue.top

[F09] 获取文件大小
来源：http://ecs.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://bso.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://vxw.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://zgs.xuanzx.com


<!-- 参考信息 -->