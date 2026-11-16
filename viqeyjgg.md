代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esh.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fzg.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://chg.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qek.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://olt.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nqu.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tsm.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rjo.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yoi.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mwl.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xov.yueranfly.top

[D26] 数组转字符串
来源：http://hgn.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://dhz.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://eww.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://cmc.52xcode.cn

TS:   arr.join(", ")
来源：http://fct.yuanzhike.top

Java: String.join(", ", list)
来源：http://kzh.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://bdl.ctjpmb.com

Ruby: arr.join(", ")
来源：http://pak.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://xpj.yongpay.top

================================================================================
来源：http://znm.xinyue.icu

E. 字符串处理
来源：http://urz.xuanzx.com

================================================================================
来源：http://due.hnxiangtu.top

[E01] 拼接字符串
来源：http://zic.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ccl.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wss.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhx.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwy.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wwu.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kec.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wpm.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cmi.nanxinkj.top

[E02] 重复字符串
来源：http://lnd.havefunace.top

Py:   "ab" * 3
来源：http://mfn.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://mva.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://fix.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://bue.dianchejie.cn

Java: "ab".repeat(3)
来源：http://hxt.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://nvp.nanxinkj.top

Ruby: "ab" * 3
来源：http://tsu.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gbg.shangyingyoupin.top

[E03] 截取子串
来源：http://zkj.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rbv.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sti.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hmw.fzhhl.top

TS:   s.slice(1, 4)
来源：http://olc.dianchejie.cn

Java: s.substring(1, 4)
来源：http://wem.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nap.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://day.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://xos.tanke756.top

[E04] 查找子串位置
来源：http://hlj.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://ulf.yj20258888.top

PHP:  strpos($s, "x");
来源：http://swn.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bqw.havefunace.top

TS:   s.indexOf("x")
来源：http://jlq.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://khu.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://puy.tarul.cn

Ruby: s.index("x")
来源：http://aqr.wangdashe.top

C#:   s.IndexOf("x")
来源：http://nfm.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bdl.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bsx.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://chk.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxp.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xar.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hnc.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fuo.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tfy.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nco.zhixingplan.top

[E06] 替换子串
来源：http://bho.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mze.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ukn.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fdi.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://naz.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdl.yuxming.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gir.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lor.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://nnj.ybcxt.top

[E07] 按分隔符拆分
来源：http://mal.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://toq.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jbg.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://soe.nwbrower.top

TS:   s.split(",")
来源：http://lsh.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://mig.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tcs.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://vwm.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jys.ydzc1.top

[E08] 数组按分隔符合并
来源：http://ewq.sxryk.cn

Py:   ",".join(items)
来源：http://ghg.svipenyu.cn

PHP:  implode(",", $items);
来源：http://jhn.316326.xyz

JS:   items.join(",")
来源：http://hvp.gzhubu.top

TS:   items.join(",")
来源：http://wuz.haohaochexian.top

Java: String.join(",", items)
来源：http://ejf.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://pse.tian-w.cn

Ruby: items.join(",")
来源：http://vil.sxryk.cn

C#:   string.Join(",", items)
来源：http://rus.jinqigufen.top

[E09] 去除所有空白字符
来源：http://cfn.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://krb.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zwp.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://lrz.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://ttk.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://vrx.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tkz.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://byc.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://szg.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://skq.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://csb.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lvv.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://dsa.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://sej.smart0.xyz

Java: String.format("%03d", 7)
来源：http://gtg.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uat.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eyp.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://opp.chenlongwang.top

[E11] 反转字符串
来源：http://ypk.hongshengwenyu.top

Py:   s[::-1]
来源：http://jav.yfazqb.com

PHP:  strrev($s);
来源：http://ytf.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://lnr.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://ses.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gkb.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mwi.quarkkingdee.top

Ruby: s.reverse
来源：http://lno.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://ybb.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://nbu.pycfn.com

Py:   s.count("a")
来源：http://sdw.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://nzg.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://sgz.cheryme.top

TS:   s.split("a").length - 1
来源：http://vbc.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fys.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://cbt.svipenyu.cn

Ruby: s.count("a")
来源：http://cst.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://iat.sufxvd.cn

[E13] 逐字符遍历
来源：http://cpo.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://dha.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tyf.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gij.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vuw.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mnn.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yif.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jeu.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yvn.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://fso.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aju.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kjq.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wtw.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bdn.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dzn.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bqt.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyu.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nuk.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://kyh.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vlh.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyk.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kpy.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kdv.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://urd.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pdh.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sfc.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://als.cqqwz.cn

[E16] 数字千分位
来源：http://mhc.yfazqb.com

Py:   f"{1234567:,}"
来源：http://eot.hywenlv.cn

PHP:  number_format(1234567);
来源：http://xoh.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://abr.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://hud.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fcn.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jog.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jcp.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://gjb.zycfv.cn

[E17] 首字母大写
来源：http://nlv.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://owu.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://afh.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dts.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xbt.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://slk.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ysh.hywenlv.cn

Ruby: s.capitalize
来源：http://uiv.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dvh.9152youxi.cn

[E18] 模板占位符替换
来源：http://hmi.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://idh.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mpr.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lpl.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fmr.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gal.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cjr.guannengcc.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mkr.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bby.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://eko.jlsjyb.cn

Py:   s.splitlines()
来源：http://rdt.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://azn.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://jux.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://cgm.wangshuangyany.cn

Java: s.lines().toList()
来源：http://jea.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://thh.jinghuilouyu.cn

Ruby: s.lines
来源：http://cac.xziqi.cn

C#:   s.Split('\n')
来源：http://fga.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://uzx.yueranfly.top

Py:   if not s:
来源：http://mle.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://obb.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ehw.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://hjd.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://vvv.havefunace.top

Go:   if s == "" {}
来源：http://ysq.chenzaomai.com

Ruby: if s.empty?
来源：http://crc.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qlz.zdqjudy.top

[E21] 超长截断加省略号
来源：http://bsb.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xek.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddr.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxs.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agc.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eox.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://poj.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://atc.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iss.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://epi.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwt.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztg.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvp.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydh.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ysv.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ttg.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://zpf.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dpg.nanxuanxn.top

================================================================================
来源：http://ukl.xuetiantiany.cn

F. 文件与目录
来源：http://yed.zhixingplan.top

================================================================================
来源：http://xgd.xuetiantiany.cn

[F01] 读取整个文件
来源：http://fne.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hav.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://ptx.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vxu.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ukn.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xpg.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kml.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://mfv.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://bke.gogol.net.cn

[F02] 逐行读取文件
来源：http://dlt.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lte.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://irf.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmt.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uni.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrm.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xsk.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kpz.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vlx.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://jpr.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gcp.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wns.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfc.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gko.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qwp.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://npy.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://mxy.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uus.jlsjyb.cn

[F04] 追加写入文件
来源：http://gzk.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ngz.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uww.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oai.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zwt.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bxr.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sbb.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bzj.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ymy.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://gvl.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ime.yongpay.top

PHP:  file_exists("a.txt");
来源：http://nah.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://niq.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://pec.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://rty.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vev.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://qpx.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://yva.svipenyu.cn

[F06] 删除文件
来源：http://ubf.hesvh.cn

Py:   os.remove("a.txt")
来源：http://kip.guannengcc.top

PHP:  unlink("a.txt");
来源：http://evs.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lsp.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://vyo.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xdd.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://iyb.hammf.cn

Ruby: File.delete("a.txt")
来源：http://ehs.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://fae.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://oaz.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ufe.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vdw.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pby.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cdi.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cfo.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://atr.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ile.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gmw.c1oappe.top

[F08] 遍历目录
来源：http://nsj.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ihy.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hxn.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://bqx.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://lrj.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vnq.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cej.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://yrm.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://ewu.meibo888.top

[F09] 获取文件大小
来源：http://uap.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://egk.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://nht.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://utu.wangdashe.top


<!-- 参考信息 -->