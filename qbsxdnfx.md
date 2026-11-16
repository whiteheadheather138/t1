代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nbb.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bap.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://tgq.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jpx.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fww.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cbf.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aay.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wyg.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://efq.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ruv.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kwz.chenlongwang.top

[D26] 数组转字符串
来源：http://hca.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://nbm.hammf.cn

PHP:  implode(", ", $arr);
来源：http://ofi.316326.xyz

JS:   arr.join(", ")
来源：http://wck.guannengcc.top

TS:   arr.join(", ")
来源：http://veo.tianlin.xyz

Java: String.join(", ", list)
来源：http://moh.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://quh.xylfe.cn

Ruby: arr.join(", ")
来源：http://muv.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://css.feifeiyinyue.top

================================================================================
来源：http://zcm.cucudq.cn

E. 字符串处理
来源：http://yrq.cheryme.top

================================================================================
来源：http://xvp.daria6918.cn

[E01] 拼接字符串
来源：http://yld.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hnn.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dij.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xba.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yso.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tts.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://faz.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eru.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcs.yj202588.top

[E02] 重复字符串
来源：http://bte.sxryk.cn

Py:   "ab" * 3
来源：http://jqg.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://ghm.guannengcc.top

JS:   "ab".repeat(3)
来源：http://pqm.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://cpc.sxryk.cn

Java: "ab".repeat(3)
来源：http://jmc.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rze.sjlbkw.cn

Ruby: "ab" * 3
来源：http://vba.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vub.hammf.cn

[E03] 截取子串
来源：http://zdf.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ixh.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gya.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sqh.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://rpm.guowangkeji.top

Java: s.substring(1, 4)
来源：http://xkb.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://den.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://ulv.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://urn.yongpay.top

[E04] 查找子串位置
来源：http://oiu.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://wea.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://bzi.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tes.daria6918.cn

TS:   s.indexOf("x")
来源：http://gvw.ehwqpu.com

Java: s.indexOf("x")
来源：http://ghu.cheryme.top

Go:   strings.Index(s, "x")
来源：http://eoh.daxiang520.top

Ruby: s.index("x")
来源：http://gpc.yj20258888.top

C#:   s.IndexOf("x")
来源：http://nsb.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://esp.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gzm.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zer.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qht.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iyc.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kyr.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksh.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hhy.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://typ.pengpengdd.cyou

[E06] 替换子串
来源：http://qcu.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jqn.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://xgf.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mcd.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://yox.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sur.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blo.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nub.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://ogq.fzhhl.top

[E07] 按分隔符拆分
来源：http://zad.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lay.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://npy.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gkb.0kj1m.cn

TS:   s.split(",")
来源：http://tik.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://yoy.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tya.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://evj.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xiq.fehbvm.com

[E08] 数组按分隔符合并
来源：http://obr.guannengcc.top

Py:   ",".join(items)
来源：http://auk.haohaochexian.top

PHP:  implode(",", $items);
来源：http://bec.xuetiantiany.cn

JS:   items.join(",")
来源：http://poo.yongpay.top

TS:   items.join(",")
来源：http://qeq.aizwys.cn

Java: String.join(",", items)
来源：http://wew.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://jkz.vehdjk.com

Ruby: items.join(",")
来源：http://sfb.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://dyf.meibo888.top

[E09] 去除所有空白字符
来源：http://nlj.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zib.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sgu.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://cgl.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://kkd.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://lpx.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yua.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://yqj.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tih.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://axj.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ypa.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bon.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://zno.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://kgc.fktsv.cn

Java: String.format("%03d", 7)
来源：http://vid.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://weh.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fna.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yqh.hysaishi.cn

[E11] 反转字符串
来源：http://xxl.smart0.xyz

Py:   s[::-1]
来源：http://sbk.jiagoushi.top

PHP:  strrev($s);
来源：http://tmx.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://ihm.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://mya.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vnc.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://grn.ydjk.org.cn

Ruby: s.reverse
来源：http://unm.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oib.hammf.cn

[E12] 统计某字符出现次数
来源：http://niq.zhijiandao.cn

Py:   s.count("a")
来源：http://ulo.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://cwi.guannengcc.top

JS:   s.split("a").length - 1
来源：http://ksd.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://fzh.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cnn.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://qiu.tarul.cn

Ruby: s.count("a")
来源：http://uyb.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://aou.vehdjk.com

[E13] 逐字符遍历
来源：http://fzv.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://css.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://heq.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gsq.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iwy.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://abi.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rss.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ovy.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://obu.zycfv.cn

[E14] URL 编码与 Base64
来源：http://lxq.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hri.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dnd.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qtj.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://evq.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eyr.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ogh.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kjl.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ocr.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://slr.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mbp.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fes.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xxu.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cir.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gox.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ubs.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wml.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pej.andypj.xyz

[E16] 数字千分位
来源：http://rck.gzhubu.top

Py:   f"{1234567:,}"
来源：http://mee.haohaochexian.top

PHP:  number_format(1234567);
来源：http://jgn.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ojo.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yts.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ibx.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://knf.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qdh.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://gcm.sweek.top

[E17] 首字母大写
来源：http://mfg.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hwv.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://htb.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjr.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urq.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pfc.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gqf.redwolf501.top

Ruby: s.capitalize
来源：http://ouk.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://okk.hnxiangtu.top

[E18] 模板占位符替换
来源：http://qyz.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dpz.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xgh.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qvh.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qhy.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cxa.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrn.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xub.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mij.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://lmf.epnwcf.com

Py:   s.splitlines()
来源：http://pbw.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pqt.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://gxe.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://svc.ydzc1.top

Java: s.lines().toList()
来源：http://hkj.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://nnx.chenzaomai.com

Ruby: s.lines
来源：http://hpy.zhijiandao.cn

C#:   s.Split('\n')
来源：http://uel.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://hck.yj20258888.top

Py:   if not s:
来源：http://hcq.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cll.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sjo.jqgufenzy.top

TS:   if (s === "") {}
来源：http://wyh.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://xhv.jlsjyb.cn

Go:   if s == "" {}
来源：http://ngj.redwolf501.top

Ruby: if s.empty?
来源：http://rgk.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://omg.andypj.xyz

[E21] 超长截断加省略号
来源：http://pbc.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://res.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jiw.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnj.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgw.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eao.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://nod.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://adx.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://awh.epnwcf.com

[E22] 字节长度与字符长度
来源：http://ptx.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kpv.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byt.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ynq.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jeb.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ddk.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oib.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://ujl.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xqd.jyoumei.cn

================================================================================
来源：http://upu.gogol.net.cn

F. 文件与目录
来源：http://uuy.yj20258.top

================================================================================
来源：http://aah.dianchejie.cn

[F01] 读取整个文件
来源：http://lbv.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vwe.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://txi.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mvu.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mae.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ztj.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://raa.yongpay.top

Ruby: File.read("a.txt")
来源：http://eht.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://tyk.zhoulong.xyz

[F02] 逐行读取文件
来源：http://eem.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qzt.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rve.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wgx.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chh.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xwf.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gpy.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bws.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qfu.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://qkc.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yej.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://upp.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://act.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jjg.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tky.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qyt.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://pmx.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bez.zhongyouzk.top

[F04] 追加写入文件
来源：http://eep.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wsh.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pmg.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xpv.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uan.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hng.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://imf.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://plt.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cwh.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://srm.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ovu.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://crr.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://khb.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://lgn.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nxp.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yhk.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://dwp.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://wrd.tanke756.top

[F06] 删除文件
来源：http://xdz.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://fmg.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://swd.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://gkp.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://bec.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zqs.yongpay.top

Go:   os.Remove("a.txt")
来源：http://xny.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://dco.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://afa.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://ubm.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gbb.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qxk.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rtb.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rdh.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dwr.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cvj.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oly.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ckr.hcnkem.com

[F08] 遍历目录
来源：http://kvp.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qok.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://epf.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://uod.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://scn.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cer.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://huo.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://dkj.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://rfx.xinyue.icu

[F09] 获取文件大小
来源：http://fqw.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://kmm.xziqi.cn

PHP:  filesize("a.txt");
来源：http://rzi.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://dxl.52xcode.cn


<!-- 参考信息 -->