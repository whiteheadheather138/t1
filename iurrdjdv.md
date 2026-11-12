代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bay.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://twb.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://wdu.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://usv.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwz.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cfr.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqf.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://guw.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sas.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hjk.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nuh.52xcode.cn

[D26] 数组转字符串
来源：http://cpb.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://wzn.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://afx.bjfxy.top

JS:   arr.join(", ")
来源：http://pyv.fehbvm.com

TS:   arr.join(", ")
来源：http://cjh.sjlbkw.cn

Java: String.join(", ", list)
来源：http://sro.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://wdd.zhengqikj.top

Ruby: arr.join(", ")
来源：http://tmg.hnqzz.top

C#:   string.Join(", ", list)
来源：http://bua.snrcjt.cn

================================================================================
来源：http://gvs.guannengcc.top

E. 字符串处理
来源：http://cvv.jqgufenzy.top

================================================================================
来源：http://mic.nwbrower.top

[E01] 拼接字符串
来源：http://mzi.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nxa.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://env.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mwp.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://utf.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gym.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ohh.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nzq.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gqx.xuetiantiany.cn

[E02] 重复字符串
来源：http://yiv.redwolf501.top

Py:   "ab" * 3
来源：http://unu.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://zng.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://gci.daxiang520.top

TS:   "ab".repeat(3)
来源：http://mxd.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://tbo.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://qgm.pycfn.com

Ruby: "ab" * 3
来源：http://jbj.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kki.kuanghao11.cn

[E03] 截取子串
来源：http://ghe.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nbo.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uyd.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://siy.tian-w.cn

TS:   s.slice(1, 4)
来源：http://oij.sweek.top

Java: s.substring(1, 4)
来源：http://wgi.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cjn.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://sct.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://thd.xylfe.cn

[E04] 查找子串位置
来源：http://fgd.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://guq.tian-w.cn

PHP:  strpos($s, "x");
来源：http://kav.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khy.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://ioi.hnqzz.top

Java: s.indexOf("x")
来源：http://egh.sweek.top

Go:   strings.Index(s, "x")
来源：http://kws.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://tzg.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://sib.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://mku.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wyv.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://spg.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://suk.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://boa.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://roi.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uuo.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://otx.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvy.jyoumei.cn

[E06] 替换子串
来源：http://phk.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rfk.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://bbr.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brm.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://jqb.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tmo.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bni.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ogf.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://ehw.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://fdb.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xox.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gas.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xie.jlsjyb.cn

TS:   s.split(",")
来源：http://bbp.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://hzj.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bda.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://nqb.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lds.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://mce.zhiwuduotai.top

Py:   ",".join(items)
来源：http://xyw.svipenyu.cn

PHP:  implode(",", $items);
来源：http://egv.dashuyun.cn

JS:   items.join(",")
来源：http://yxf.zhengqikj.top

TS:   items.join(",")
来源：http://krs.sysykeji.top

Java: String.join(",", items)
来源：http://gjc.pycfn.com

Go:   strings.Join(items, ",")
来源：http://ivx.0kj1m.cn

Ruby: items.join(",")
来源：http://wog.yuanzhike.top

C#:   string.Join(",", items)
来源：http://pun.yvedp.cn

[E09] 去除所有空白字符
来源：http://ylf.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uqf.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://igo.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://duv.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://nrn.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://sfd.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yrn.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://tgw.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ywj.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://gta.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ayt.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://guu.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://iiw.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://aia.52xcode.cn

Java: String.format("%03d", 7)
来源：http://uiv.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahi.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sok.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ubh.yj20258.top

[E11] 反转字符串
来源：http://wsa.guowangkeji.top

Py:   s[::-1]
来源：http://hbx.xuanzx.com

PHP:  strrev($s);
来源：http://gbb.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://xab.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://msa.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lnz.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fbp.fktsv.cn

Ruby: s.reverse
来源：http://itv.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://beo.meibo888.top

[E12] 统计某字符出现次数
来源：http://xwk.guannengcc.top

Py:   s.count("a")
来源：http://lxp.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://ohv.gzhubu.top

JS:   s.split("a").length - 1
来源：http://qib.andypj.xyz

TS:   s.split("a").length - 1
来源：http://exz.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qqj.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://dil.zycfv.cn

Ruby: s.count("a")
来源：http://rng.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://yqc.jinqigufen.top

[E13] 逐字符遍历
来源：http://wuy.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://tsv.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kzw.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxn.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qdb.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pxf.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://syl.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qcw.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ztu.xziqi.cn

[E14] URL 编码与 Base64
来源：http://qsq.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jge.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qqz.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hmu.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nxv.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rtm.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tln.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://idx.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://itt.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://bpe.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hqi.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://krn.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mel.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ccu.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fmq.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sfu.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iec.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jcp.zhijiandao.cn

[E16] 数字千分位
来源：http://jhj.yj202588.top

Py:   f"{1234567:,}"
来源：http://ebd.jqgfzy.top

PHP:  number_format(1234567);
来源：http://vvi.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ekk.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://gxq.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hwa.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://upt.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gtp.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://yci.mhx1999.top

[E17] 首字母大写
来源：http://mzi.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ciq.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://guh.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qrw.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xan.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://edo.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://btf.fengsongda.top

Ruby: s.capitalize
来源：http://lgb.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://plt.aibaodan.cn

[E18] 模板占位符替换
来源：http://kss.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fyo.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://imq.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://cme.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qnf.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmx.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wfz.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xfs.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ich.guannengcc.top

[E19] 多行文本按行拆分
来源：http://nqz.chenlongwang.top

Py:   s.splitlines()
来源：http://gni.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://emv.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://rlh.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://vky.wangshuangyany.cn

Java: s.lines().toList()
来源：http://rlz.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://fjc.cheryme.top

Ruby: s.lines
来源：http://pep.ctjpmb.com

C#:   s.Split('\n')
来源：http://pbq.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://kqh.zhixingplan.top

Py:   if not s:
来源：http://dmz.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jit.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kez.hcnkem.com

TS:   if (s === "") {}
来源：http://spq.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://ozc.yfazqb.com

Go:   if s == "" {}
来源：http://fzq.svipenyu.cn

Ruby: if s.empty?
来源：http://ukr.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tyy.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://oil.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ywb.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jew.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxe.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tus.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vta.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://mjp.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tkd.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmc.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://hwc.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lal.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvw.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyv.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkc.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vxi.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dcv.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://xbm.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://azb.ywan-chungtsiang.top

================================================================================
来源：http://ijl.sufxvd.cn

F. 文件与目录
来源：http://vmk.birdmap.top

================================================================================
来源：http://ejb.xuanzx.com

[F01] 读取整个文件
来源：http://qri.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dfp.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://cfe.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lqm.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwy.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://gks.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hdy.bjfxy.top

Ruby: File.read("a.txt")
来源：http://enj.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://ghq.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://wib.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://trg.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dxm.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mel.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pye.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fnr.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kzh.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ual.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://djm.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://ouc.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sqf.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://osp.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jxn.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://czd.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ntm.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://npt.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://hjg.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hfg.ivvv.top

[F04] 追加写入文件
来源：http://ist.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hzz.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gwz.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bra.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cdf.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lwi.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jgj.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gvp.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://akk.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://xvg.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxe.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://uyk.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://xys.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://rnu.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rdb.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xxo.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://gmy.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://fag.zdqjudy.top

[F06] 删除文件
来源：http://rmo.smart0.xyz

Py:   os.remove("a.txt")
来源：http://urv.shuidangran.top

PHP:  unlink("a.txt");
来源：http://fxw.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://paw.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://glf.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pbu.tarul.cn

Go:   os.Remove("a.txt")
来源：http://upq.ivvv.top

Ruby: File.delete("a.txt")
来源：http://xlz.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://ixq.guannengcc.top

[F07] 创建目录（含多级）
来源：http://tpe.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bde.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fqy.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uic.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvz.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hrl.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fvb.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lwq.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tmy.dianchejie.cn

[F08] 遍历目录
来源：http://vuj.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://azk.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://flo.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://bog.nanxuanxn.top

TS:   fs.readdirSync("dir")
来源：http://cpn.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yph.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lig.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://pck.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://cud.hnqzz.top

[F09] 获取文件大小
来源：http://era.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://bpp.vehdjk.com

PHP:  filesize("a.txt");
来源：http://gwa.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://vwk.zhixingplan.top


<!-- 参考信息 -->