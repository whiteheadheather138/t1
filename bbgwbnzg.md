代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tbq.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://auw.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://pjt.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vje.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wig.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://akx.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bwg.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pnq.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qnr.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hmm.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wlt.fktsv.cn

[D26] 数组转字符串
来源：http://vtt.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://xfe.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://oat.sweek.top

JS:   arr.join(", ")
来源：http://btz.svipenyu.cn

TS:   arr.join(", ")
来源：http://wjb.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://yza.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://lod.ivvv.top

Ruby: arr.join(", ")
来源：http://hga.xinyue.icu

C#:   string.Join(", ", list)
来源：http://bfr.haohaochexian.top

================================================================================
来源：http://hqa.gaohongyu789.top

E. 字符串处理
来源：http://dse.zdbjq.cn

================================================================================
来源：http://ulx.sxryk.cn

[E01] 拼接字符串
来源：http://zty.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zpn.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kny.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuu.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jbd.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mls.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xrb.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vxc.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cyi.feifeiyinyue.top

[E02] 重复字符串
来源：http://hoh.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://wtw.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://bek.ydzc1.top

JS:   "ab".repeat(3)
来源：http://ryt.ivvv.top

TS:   "ab".repeat(3)
来源：http://fxm.pycfn.com

Java: "ab".repeat(3)
来源：http://ynn.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://ceq.yanxiufei.cn

Ruby: "ab" * 3
来源：http://btn.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kro.zycfv.cn

[E03] 截取子串
来源：http://ohp.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ckd.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ktv.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ynd.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://esy.yj20258888.top

Java: s.substring(1, 4)
来源：http://wwe.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tbj.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://kjd.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://bik.yfazqb.com

[E04] 查找子串位置
来源：http://rru.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://ujc.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://gme.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://imp.ydzc1.top

TS:   s.indexOf("x")
来源：http://lzy.yj20258.top

Java: s.indexOf("x")
来源：http://wab.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://oqk.xylfe.cn

Ruby: s.index("x")
来源：http://adv.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://cld.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ebm.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tmq.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jno.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvy.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffw.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxi.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gzs.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://prl.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqt.chenlongwang.top

[E06] 替换子串
来源：http://teo.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xit.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://ers.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jug.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://brq.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mxm.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pho.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rug.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://gtr.yfazqb.com

[E07] 按分隔符拆分
来源：http://foh.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sqt.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dgy.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zzw.dashuyun.cn

TS:   s.split(",")
来源：http://lqz.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xoc.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oai.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://idy.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rlj.fzhhl.top

[E08] 数组按分隔符合并
来源：http://pew.cdnleiting.top

Py:   ",".join(items)
来源：http://ssr.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://kmo.fehbvm.com

JS:   items.join(",")
来源：http://jam.gogol.net.cn

TS:   items.join(",")
来源：http://wfb.ydjk.org.cn

Java: String.join(",", items)
来源：http://fkj.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://ewc.zhengqikj.top

Ruby: items.join(",")
来源：http://zxu.bbcook.cn

C#:   string.Join(",", items)
来源：http://mxt.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://uwy.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dvz.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://isv.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://gav.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://wxv.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://hxl.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nhr.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://gec.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bdy.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://uji.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://stp.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://egy.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://psw.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://zpv.jianghu66.top

Java: String.format("%03d", 7)
来源：http://skb.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bdd.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xck.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wuj.hammf.cn

[E11] 反转字符串
来源：http://vdr.hongshengwenyu.top

Py:   s[::-1]
来源：http://dfk.daxiang520.top

PHP:  strrev($s);
来源：http://rec.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://huf.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://uql.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cmq.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://kgx.sysykeji.top

Ruby: s.reverse
来源：http://cyx.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lfz.jianghu66.top

[E12] 统计某字符出现次数
来源：http://spn.wangshuangyany.cn

Py:   s.count("a")
来源：http://zta.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://vzo.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://jqz.yvedp.cn

TS:   s.split("a").length - 1
来源：http://lzr.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://krn.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://rax.yj20258888.top

Ruby: s.count("a")
来源：http://udw.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://nuh.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://jqk.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://sed.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tlr.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zzw.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxj.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dij.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://orc.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dyt.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xrq.zycfv.cn

[E14] URL 编码与 Base64
来源：http://ltd.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lsr.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ccd.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pgu.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pra.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qrb.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://miy.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oxy.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xtm.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://wwz.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bkx.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://glc.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ldj.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://vmj.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lic.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lmm.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sjd.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kzs.yangfankeji.com

[E16] 数字千分位
来源：http://evl.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://jaq.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://wms.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cnp.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ouh.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://acm.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pzp.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://twy.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://xbx.gogol.net.cn

[E17] 首字母大写
来源：http://tmo.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mbi.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ttk.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hnb.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guk.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://emm.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hcx.nwbrower.top

Ruby: s.capitalize
来源：http://ncx.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://usy.uphjek.com

[E18] 模板占位符替换
来源：http://pbd.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ptn.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yms.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mod.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dhr.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gww.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xwx.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tnb.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rgg.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://xje.svipenyu.cn

Py:   s.splitlines()
来源：http://ddw.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jbh.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://uok.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://cuz.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://qpz.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://ssq.pycfn.com

Ruby: s.lines
来源：http://exq.svipenyu.cn

C#:   s.Split('\n')
来源：http://chl.yj20258.top

[E20] 判断字符串是否为空
来源：http://czj.zhoulong.xyz

Py:   if not s:
来源：http://tfv.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yxq.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xlz.mhx1999.top

TS:   if (s === "") {}
来源：http://zeb.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://rzw.snrcjt.cn

Go:   if s == "" {}
来源：http://dlb.redwolf501.top

Ruby: if s.empty?
来源：http://wuu.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yan.cheryme.top

[E21] 超长截断加省略号
来源：http://oud.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vzu.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uyi.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rry.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://enr.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://frg.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wbr.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fgu.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://usr.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://kjk.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lme.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cvx.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksy.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://muy.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hot.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lnv.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://huj.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://clm.birdmap.top

================================================================================
来源：http://kjv.pycfn.com

F. 文件与目录
来源：http://iqi.tianlin.xyz

================================================================================
来源：http://uyv.hammf.cn

[F01] 读取整个文件
来源：http://gmc.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xfj.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://ogl.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cbi.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ugh.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pmt.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pby.sxryk.cn

Ruby: File.read("a.txt")
来源：http://wuy.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://yvt.zhongyouzk.top

[F02] 逐行读取文件
来源：http://tvr.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hss.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vnn.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpa.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jzu.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pnt.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jct.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aok.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgj.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://ika.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjm.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://omz.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zqz.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsa.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aia.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dpc.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://rpg.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pqb.9152youxi.cn

[F04] 追加写入文件
来源：http://qrd.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ayu.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jfc.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pjx.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://skt.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qmb.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nuh.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cxe.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bgr.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://fkl.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvq.yj202588.top

PHP:  file_exists("a.txt");
来源：http://axr.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://wkg.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://ojq.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://shr.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mca.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://wsm.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://bjd.sjlbkw.cn

[F06] 删除文件
来源：http://ois.yfazqb.com

Py:   os.remove("a.txt")
来源：http://srm.yj20258.top

PHP:  unlink("a.txt");
来源：http://nbz.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://lka.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://trt.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kkr.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://xgj.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://mxi.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://wwn.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://jsx.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cas.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vfy.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtn.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wen.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://max.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wuf.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fmg.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ofh.xuetiantiany.cn

[F08] 遍历目录
来源：http://kqb.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yqf.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bti.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://hvw.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://ybq.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zih.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tca.bjfxy.top

Ruby: Dir.children("dir")
来源：http://pxp.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://dcu.kuanghao11.cn

[F09] 获取文件大小
来源：http://ytc.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://bwo.c1oappe.top

PHP:  filesize("a.txt");
来源：http://mob.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://jdn.daria6918.cn


<!-- 参考信息 -->