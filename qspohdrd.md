代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wgl.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://axt.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://nlc.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://acg.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lcv.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://suf.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rdj.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qwi.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jol.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gaq.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://miq.ppjwa.cn

[D26] 数组转字符串
来源：http://kxu.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://nfq.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://uce.zhoulong.xyz

JS:   arr.join(", ")
来源：http://myq.uphjek.com

TS:   arr.join(", ")
来源：http://wpl.52xcode.cn

Java: String.join(", ", list)
来源：http://gbt.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://gjf.cdnleiting.top

Ruby: arr.join(", ")
来源：http://nch.tarul.cn

C#:   string.Join(", ", list)
来源：http://snx.xuetiantiany.cn

================================================================================
来源：http://mqi.yuanzhike.top

E. 字符串处理
来源：http://vyu.cdnleiting.top

================================================================================
来源：http://rnv.ivvv.top

[E01] 拼接字符串
来源：http://afz.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://khu.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wax.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exj.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kyf.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mrl.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yrt.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vza.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ocf.jiagoushi.top

[E02] 重复字符串
来源：http://ibz.meibo888.top

Py:   "ab" * 3
来源：http://vkf.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://and.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://vrv.cashguo.top

TS:   "ab".repeat(3)
来源：http://itl.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://inv.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://uzx.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://fnw.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uqc.wangshuangyany.cn

[E03] 截取子串
来源：http://nek.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ddp.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jhn.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pwk.fzhhl.top

TS:   s.slice(1, 4)
来源：http://wur.ehwqpu.com

Java: s.substring(1, 4)
来源：http://nzv.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gue.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://llc.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://xqe.gogol.net.cn

[E04] 查找子串位置
来源：http://hbw.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://wrc.daxiang520.top

PHP:  strpos($s, "x");
来源：http://rza.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bgx.ivvv.top

TS:   s.indexOf("x")
来源：http://rlx.hcnkem.com

Java: s.indexOf("x")
来源：http://jhr.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://tge.ctjpmb.com

Ruby: s.index("x")
来源：http://vco.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://qdz.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://csy.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://omk.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://luz.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lue.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://tql.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oal.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zhq.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xja.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kpm.smart0.xyz

[E06] 替换子串
来源：http://mgs.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://goq.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://fyl.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysv.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://csa.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amm.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ugb.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hcc.yongpay.top

C#:   s.Replace("a", "b")
来源：http://ibi.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://fww.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zyj.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ikr.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyp.52xcode.cn

TS:   s.split(",")
来源：http://khb.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://ehf.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uqx.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://ndl.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tth.hnqzz.top

[E08] 数组按分隔符合并
来源：http://ugi.vqdsnc.cn

Py:   ",".join(items)
来源：http://mms.aizwys.cn

PHP:  implode(",", $items);
来源：http://niq.hcnkem.com

JS:   items.join(",")
来源：http://ibd.yangfankeji.com

TS:   items.join(",")
来源：http://ntt.cashguo.top

Java: String.join(",", items)
来源：http://zux.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://sow.yj20258888.top

Ruby: items.join(",")
来源：http://kce.bbcook.cn

C#:   string.Join(",", items)
来源：http://hde.tian-w.cn

[E09] 去除所有空白字符
来源：http://mkn.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qdq.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ytp.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://zaz.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://ccq.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://efi.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ciw.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ope.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zih.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://erl.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vzz.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gzc.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://isc.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://bmk.meibo888.top

Java: String.format("%03d", 7)
来源：http://ucy.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bus.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ckp.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sfo.hammf.cn

[E11] 反转字符串
来源：http://soe.zhengqikj.top

Py:   s[::-1]
来源：http://wyx.sufxvd.cn

PHP:  strrev($s);
来源：http://njo.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://zbd.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://efd.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ljc.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vef.shzxlz.cn

Ruby: s.reverse
来源：http://cmg.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://uhy.bjfxy.top

[E12] 统计某字符出现次数
来源：http://xnk.jyoumei.cn

Py:   s.count("a")
来源：http://mba.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://otk.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://kae.guannengcc.top

TS:   s.split("a").length - 1
来源：http://rdg.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://try.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://rhj.ybcxt.top

Ruby: s.count("a")
来源：http://iyl.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://fhr.gotoacloud.top

[E13] 逐字符遍历
来源：http://ova.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://mqy.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://igl.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mno.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dki.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fhb.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kqv.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://krt.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://agx.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://soz.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vcv.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kfy.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cvb.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://frk.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iqc.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rsk.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bpn.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nhd.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://xaz.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pdv.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bpk.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dpc.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://era.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fyp.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://umz.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://prh.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hir.gogol.net.cn

[E16] 数字千分位
来源：http://xhx.shuidangran.top

Py:   f"{1234567:,}"
来源：http://sts.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://gdd.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nju.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://heh.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qqu.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ljf.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bfg.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://wnh.chenjidiqi.icu

[E17] 首字母大写
来源：http://tfc.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jdc.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xhe.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nfu.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtc.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://did.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rds.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://ziz.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xto.birdmap.top

[E18] 模板占位符替换
来源：http://cit.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gfh.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eba.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wgi.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cln.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ohm.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mpn.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yxi.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yyu.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://thl.yangfankeji.com

Py:   s.splitlines()
来源：http://ewl.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kvf.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://tsj.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://wgf.gaohongyu789.top

Java: s.lines().toList()
来源：http://qsp.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://ojx.gogol.net.cn

Ruby: s.lines
来源：http://rkl.fzhhl.top

C#:   s.Split('\n')
来源：http://zle.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://asc.bbcook.cn

Py:   if not s:
来源：http://mrh.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uwj.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jsw.sxryk.cn

TS:   if (s === "") {}
来源：http://wfg.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://hsq.jqgfzy.top

Go:   if s == "" {}
来源：http://ici.cashguo.top

Ruby: if s.empty?
来源：http://oqp.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oxs.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://wok.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dms.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xlk.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izq.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kol.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uli.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://pep.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yel.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cek.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://cdv.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ytj.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gqy.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mti.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpn.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hrn.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://brq.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://qmt.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czd.fktsv.cn

================================================================================
来源：http://lww.zhongyouzk.top

F. 文件与目录
来源：http://hkv.ehwqpu.com

================================================================================
来源：http://bkp.hnqzz.top

[F01] 读取整个文件
来源：http://mnf.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iqy.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://fqu.ybcxt.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tuh.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rwh.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fez.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://asd.sxryk.cn

Ruby: File.read("a.txt")
来源：http://pyv.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://hkc.mhx1999.top

[F02] 逐行读取文件
来源：http://uku.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hha.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://guu.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sfn.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrv.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qwv.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qsy.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukr.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jdq.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://qja.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sik.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kdk.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwe.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wue.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ypi.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wmu.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://ckz.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mfj.fengsongda.top

[F04] 追加写入文件
来源：http://atj.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bkj.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gsq.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucx.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://atv.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eyq.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xkj.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://udc.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rjt.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://zwq.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://doj.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://wja.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://tab.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://wsq.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ubz.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jru.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://bbl.birdmap.top

C#:   File.Exists("a.txt")
来源：http://lhq.hnxiangtu.top

[F06] 删除文件
来源：http://opc.zycfv.cn

Py:   os.remove("a.txt")
来源：http://ivz.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://htb.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://djt.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://lga.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ynj.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://rfw.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://vfl.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://jci.tanke756.top

[F07] 创建目录（含多级）
来源：http://qnx.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdy.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://riu.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twe.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jkf.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nql.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bel.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sbi.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dbz.ppjwa.cn

[F08] 遍历目录
来源：http://tnw.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgk.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tmg.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://isa.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://ext.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gka.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nsa.sweek.top

Ruby: Dir.children("dir")
来源：http://qww.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://srr.mhx1999.top

[F09] 获取文件大小
来源：http://wqx.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://qii.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://gvl.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://eqy.ehwqpu.com


<!-- 参考信息 -->