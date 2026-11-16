代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nrg.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pmt.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://nte.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sdp.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vyf.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wxe.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vtk.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://crf.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xds.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mfr.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hhb.cheryme.top

[D26] 数组转字符串
来源：http://mok.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://scq.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://ziq.yongpay.top

JS:   arr.join(", ")
来源：http://ecm.jiagoushi.top

TS:   arr.join(", ")
来源：http://rkn.gaohongyu789.top

Java: String.join(", ", list)
来源：http://xht.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://cle.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://orb.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://syi.haohaochexian.top

================================================================================
来源：http://dan.hywenlv.cn

E. 字符串处理
来源：http://ths.guowangkeji.top

================================================================================
来源：http://avd.yvedp.cn

[E01] 拼接字符串
来源：http://dur.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdf.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsm.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvq.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ylf.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cpr.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tmc.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sxr.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://avy.jyoumei.cn

[E02] 重复字符串
来源：http://nee.dianchejie.cn

Py:   "ab" * 3
来源：http://xar.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://tuy.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://hde.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://xzz.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://lcm.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://hta.bjfxy.top

Ruby: "ab" * 3
来源：http://apt.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vfm.andypj.xyz

[E03] 截取子串
来源：http://pps.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xda.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cep.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xwt.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://hhw.shzxlz.cn

Java: s.substring(1, 4)
来源：http://jmq.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhm.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fuq.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://sus.yj20258.top

[E04] 查找子串位置
来源：http://tmk.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://zke.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://efx.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ieo.yuanzhike.top

TS:   s.indexOf("x")
来源：http://ijy.yanxiufei.cn

Java: s.indexOf("x")
来源：http://sxv.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://usv.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://xzj.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://mrf.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tge.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qqi.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qqq.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://loj.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekh.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gov.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yhq.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jvo.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kka.shangyingyoupin.top

[E06] 替换子串
来源：http://wpl.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yql.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://beb.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnu.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://rnj.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjs.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lxq.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://trs.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://jor.cqqwz.cn

[E07] 按分隔符拆分
来源：http://izq.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://phq.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cvd.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kdg.fanxiaobao.xyz

TS:   s.split(",")
来源：http://tuz.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nyb.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qmy.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://udq.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xft.sysykeji.top

[E08] 数组按分隔符合并
来源：http://yny.redwolf501.top

Py:   ",".join(items)
来源：http://fqi.9152youxi.cn

PHP:  implode(",", $items);
来源：http://mvd.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://klb.sweek.top

TS:   items.join(",")
来源：http://fvy.guannengcc.top

Java: String.join(",", items)
来源：http://lmv.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://tsr.jqgufenzy.top

Ruby: items.join(",")
来源：http://lqi.bjfxy.top

C#:   string.Join(",", items)
来源：http://jqk.cashguo.top

[E09] 去除所有空白字符
来源：http://ush.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fqk.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypv.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://pxs.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://coj.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://iir.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://whr.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://tes.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jdx.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://exb.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lta.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://anb.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://sdj.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://cvb.sweek.top

Java: String.format("%03d", 7)
来源：http://tjw.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://okh.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mog.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wez.redwolf501.top

[E11] 反转字符串
来源：http://dpm.9152youxi.cn

Py:   s[::-1]
来源：http://qqc.ivvv.top

PHP:  strrev($s);
来源：http://ilc.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://ixx.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://sja.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://scb.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ffi.wangshuangyany.cn

Ruby: s.reverse
来源：http://vxp.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://naw.xinyue.icu

[E12] 统计某字符出现次数
来源：http://tgy.c1oappe.top

Py:   s.count("a")
来源：http://ojr.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://apf.shuidangran.top

JS:   s.split("a").length - 1
来源：http://pvz.yfazqb.com

TS:   s.split("a").length - 1
来源：http://zod.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lts.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://gcu.yvedp.cn

Ruby: s.count("a")
来源：http://fco.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://krl.sjlbkw.cn

[E13] 逐字符遍历
来源：http://dpc.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://rxy.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hgz.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jfx.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bfv.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wza.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://foa.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://wkg.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zbn.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://jsj.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lxl.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://kal.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpo.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nzb.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://prc.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xou.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yfz.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ylf.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://puj.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sqi.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nep.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mdc.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gpm.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ujm.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://auy.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xrx.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hcm.ydjk.org.cn

[E16] 数字千分位
来源：http://zjn.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://wlb.gogol.net.cn

PHP:  number_format(1234567);
来源：http://znm.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xbn.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yfd.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gyu.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mju.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://btp.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://nrw.hesvh.cn

[E17] 首字母大写
来源：http://uzf.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uad.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vdy.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jar.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mdh.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fxt.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sbz.yangfankeji.com

Ruby: s.capitalize
来源：http://hwn.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ozh.uphjek.com

[E18] 模板占位符替换
来源：http://lcs.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lmn.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://itd.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ycg.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wyz.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ffc.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wgd.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zgq.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pof.havefunace.top

[E19] 多行文本按行拆分
来源：http://xis.dianchejie.cn

Py:   s.splitlines()
来源：http://dev.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uvg.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://nua.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://xje.mhx1999.top

Java: s.lines().toList()
来源：http://kqi.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://pqo.jqgfzy.top

Ruby: s.lines
来源：http://wxj.jqgufenzy.top

C#:   s.Split('\n')
来源：http://mzq.sweek.top

[E20] 判断字符串是否为空
来源：http://iny.zdqjudy.top

Py:   if not s:
来源：http://vob.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vrk.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uih.jianghu66.top

TS:   if (s === "") {}
来源：http://byt.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://jmp.nanxinkj.top

Go:   if s == "" {}
来源：http://atl.daxiang520.top

Ruby: if s.empty?
来源：http://sor.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://few.yonumen.top

[E21] 超长截断加省略号
来源：http://kfd.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ndq.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jcp.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfm.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hte.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yip.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://cwu.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipm.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kis.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://cuu.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nbg.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://guh.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmt.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fgv.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pnx.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://orv.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://gqa.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ano.yj20258888.top

================================================================================
来源：http://yce.sufxvd.cn

F. 文件与目录
来源：http://oul.sxryk.cn

================================================================================
来源：http://xih.vqdsnc.cn

[F01] 读取整个文件
来源：http://gvq.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://izz.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://cpo.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gyq.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eek.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://gzy.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yjp.yj20258.top

Ruby: File.read("a.txt")
来源：http://agw.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://yud.epnwcf.com

[F02] 逐行读取文件
来源：http://rio.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ccd.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sic.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://krx.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqw.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ytk.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://esw.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qhr.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vvu.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://xma.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rxs.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kax.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qmx.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bgf.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sqj.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqg.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://fxx.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://akr.shzxlz.cn

[F04] 追加写入文件
来源：http://srn.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gyv.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sut.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfa.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvx.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mgr.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bwz.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zfo.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nsi.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://amy.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://adv.cashguo.top

PHP:  file_exists("a.txt");
来源：http://fvr.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://urw.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://uqu.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://diu.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iif.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://wcw.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://opc.zhaomingkeji.xyz

[F06] 删除文件
来源：http://alq.yfazqb.com

Py:   os.remove("a.txt")
来源：http://alj.xylfe.cn

PHP:  unlink("a.txt");
来源：http://rgz.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rum.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://efn.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cbn.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://tkq.uphjek.com

Ruby: File.delete("a.txt")
来源：http://bdy.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://zxd.yj20258.top

[F07] 创建目录（含多级）
来源：http://axn.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://euv.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fjl.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzp.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xri.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kii.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zdl.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yew.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bnb.hammf.cn

[F08] 遍历目录
来源：http://kem.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ovc.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://new.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://uuj.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://hzk.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kbp.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://tso.yuxming.cn

Ruby: Dir.children("dir")
来源：http://gmy.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://qqm.bbcook.cn

[F09] 获取文件大小
来源：http://xnw.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://jip.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://ljn.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://yhh.zhiwuduotai.top


<!-- 参考信息 -->