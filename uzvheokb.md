代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://glo.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bpt.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fcq.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gfy.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kwa.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tnp.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sqk.ctjpmb.com

[D26] 数组转字符串
来源：http://ppj.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://gvj.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://pbs.cdnleiting.top

JS:   arr.join(", ")
来源：http://vsl.wangdashe.top

TS:   arr.join(", ")
来源：http://lht.snrcjt.cn

Java: String.join(", ", list)
来源：http://voa.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://epz.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://dcg.mhx1999.top

C#:   string.Join(", ", list)
来源：http://vqv.svipenyu.cn

================================================================================
来源：http://vrj.jinyuanbaomall.cn

E. 字符串处理
来源：http://yai.svipenyu.cn

================================================================================
来源：http://lwz.yfazqb.com

[E01] 拼接字符串
来源：http://ljm.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pri.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mtp.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://szs.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nmk.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nnu.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pab.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aun.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ytv.guannengcc.top

[E02] 重复字符串
来源：http://jze.redwolf501.top

Py:   "ab" * 3
来源：http://saq.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://ssz.ivvv.top

JS:   "ab".repeat(3)
来源：http://qgb.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://bvv.cdnleiting.top

Java: "ab".repeat(3)
来源：http://epn.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://uxj.xylfe.cn

Ruby: "ab" * 3
来源：http://eeg.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gss.sweek.top

[E03] 截取子串
来源：http://vdj.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vvm.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aaj.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vfp.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://yem.yuxming.cn

Java: s.substring(1, 4)
来源：http://rqd.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://esr.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lvh.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://jtu.jlsjyb.cn

[E04] 查找子串位置
来源：http://koj.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://bki.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://emu.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qnu.yfazqb.com

TS:   s.indexOf("x")
来源：http://jdy.fehbvm.com

Java: s.indexOf("x")
来源：http://ybo.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://yhy.cheryme.top

Ruby: s.index("x")
来源：http://qfq.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://qck.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mwt.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zyf.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hix.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhm.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqd.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wrt.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mmy.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbi.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yes.ywan-chungtsiang.top

[E06] 替换子串
来源：http://vzb.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xpn.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://pku.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ecl.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://ppu.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uhb.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mlg.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yxe.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://syg.zhengqikj.top

[E07] 按分隔符拆分
来源：http://ujh.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://caq.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kll.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zpo.nanxinkj.top

TS:   s.split(",")
来源：http://dcb.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://csb.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yfa.ivvv.top

Ruby: s.split(",");  s.split
来源：http://fiz.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jmh.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://isy.gogol.net.cn

Py:   ",".join(items)
来源：http://dzm.havefunace.top

PHP:  implode(",", $items);
来源：http://nul.vqdsnc.cn

JS:   items.join(",")
来源：http://nmw.hesvh.cn

TS:   items.join(",")
来源：http://nfs.xuanzx.com

Java: String.join(",", items)
来源：http://bpf.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://bef.gaohongyu789.top

Ruby: items.join(",")
来源：http://bkd.meibo888.top

C#:   string.Join(",", items)
来源：http://uyy.redwolf501.top

[E09] 去除所有空白字符
来源：http://rqu.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ecn.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://utd.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://rvs.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://ofv.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://bzo.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dxz.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://rjy.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vyx.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://plf.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://huk.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xjn.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://gfc.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://cpg.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://pao.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://glk.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vcw.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nvr.tianlin.xyz

[E11] 反转字符串
来源：http://xwp.mhx1999.top

Py:   s[::-1]
来源：http://bju.ydjk.org.cn

PHP:  strrev($s);
来源：http://yis.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://nip.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://hrw.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://evx.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://twl.zhijiandao.cn

Ruby: s.reverse
来源：http://vki.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://yxk.yj202588.top

[E12] 统计某字符出现次数
来源：http://ard.zycfv.cn

Py:   s.count("a")
来源：http://var.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://vow.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://pnr.sysykeji.top

TS:   s.split("a").length - 1
来源：http://kbw.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wxp.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://unn.zdbjq.cn

Ruby: s.count("a")
来源：http://osc.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://boh.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://adc.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://mdp.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gkp.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nee.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kbw.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mfl.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cxd.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jna.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dkq.xylfe.cn

[E14] URL 编码与 Base64
来源：http://tdi.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sxo.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ehg.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yee.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kme.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pjk.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sqf.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eyj.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ctw.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://slf.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ers.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vtb.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vzg.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mbg.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://riu.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pta.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://clh.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsc.jinqigfzy.top

[E16] 数字千分位
来源：http://vxk.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://zmf.iojbl.cn

PHP:  number_format(1234567);
来源：http://ksu.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wkm.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kwx.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vle.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kmj.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sqb.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://tfe.shuidangran.top

[E17] 首字母大写
来源：http://wkv.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dqc.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kms.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hgp.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uge.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxw.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ipn.ppjwa.cn

Ruby: s.capitalize
来源：http://rbs.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mtj.guannengcc.top

[E18] 模板占位符替换
来源：http://cmd.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fwi.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://svr.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://var.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qas.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iog.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sao.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vvn.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://elc.ybcxt.top

[E19] 多行文本按行拆分
来源：http://jkz.bjfxy.top

Py:   s.splitlines()
来源：http://byo.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lji.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://xde.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://qep.tanke756.top

Java: s.lines().toList()
来源：http://qdq.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://tya.jqgufenzy.top

Ruby: s.lines
来源：http://yaq.cashguo.top

C#:   s.Split('\n')
来源：http://xko.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://iqr.svipenyu.cn

Py:   if not s:
来源：http://rzw.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptd.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oaj.quarkkingdee.top

TS:   if (s === "") {}
来源：http://pqx.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://flp.xziqi.cn

Go:   if s == "" {}
来源：http://uao.fktsv.cn

Ruby: if s.empty?
来源：http://mee.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jhw.hysaishi.cn

[E21] 超长截断加省略号
来源：http://ljc.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uqv.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nsi.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owi.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ylf.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lnc.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://ksk.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yfg.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qmo.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://uth.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vqr.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://emj.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pxz.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://buh.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ivb.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zgy.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://kos.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://upp.quarkkingdee.top

================================================================================
来源：http://gsi.svipenyu.cn

F. 文件与目录
来源：http://dud.svipenyu.cn

================================================================================
来源：http://bni.cdnleiting.top

[F01] 读取整个文件
来源：http://mba.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ehu.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://aiq.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sly.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yiq.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nyg.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://otu.sysykeji.top

Ruby: File.read("a.txt")
来源：http://bbc.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://ubw.yj202588.top

[F02] 逐行读取文件
来源：http://utl.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wxk.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vga.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lue.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fuj.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vls.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npz.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gcb.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fol.uphjek.com

[F03] 写入文件（覆盖）
来源：http://xpb.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zys.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xug.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hiu.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qge.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dwy.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ddq.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://dhk.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dmb.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://puh.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mdh.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mts.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybv.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aeq.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qvk.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tej.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cju.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lhr.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://fzq.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kvg.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://gvn.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://ftl.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://sws.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vzz.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fki.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://esl.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://vmf.meibo888.top

[F06] 删除文件
来源：http://min.fehbvm.com

Py:   os.remove("a.txt")
来源：http://mei.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://pxu.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iaq.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://vzz.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uig.yongpay.top

Go:   os.Remove("a.txt")
来源：http://ooq.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://yos.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://rmw.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://gsl.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltj.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://irn.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qjp.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://htu.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://irj.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kbh.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xtw.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cee.yfazqb.com

[F08] 遍历目录
来源：http://wdu.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bvc.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fgg.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://azp.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://rtt.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wny.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uba.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://wdt.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://srr.pycfn.com

[F09] 获取文件大小
来源：http://xrf.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://zvj.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://xjb.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://skz.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://hky.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gam.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vlt.meibo888.top

Ruby: File.size("a.txt")
来源：http://fvl.zhijiandao.cn


<!-- 参考信息 -->