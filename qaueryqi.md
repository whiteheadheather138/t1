代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bpa.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rvm.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tva.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tdt.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uif.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltz.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vwo.zycfv.cn

[D26] 数组转字符串
来源：http://uaj.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://shv.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://vgd.hcnkem.com

JS:   arr.join(", ")
来源：http://tbl.pycfn.com

TS:   arr.join(", ")
来源：http://xkd.jyoumei.cn

Java: String.join(", ", list)
来源：http://iza.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://awk.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://onp.yj20258.top

C#:   string.Join(", ", list)
来源：http://vir.epnwcf.com

================================================================================
来源：http://fgl.pycfn.com

E. 字符串处理
来源：http://uar.cqqwz.cn

================================================================================
来源：http://kez.jqgfzy.top

[E01] 拼接字符串
来源：http://cuz.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mcf.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ykt.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gfy.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lws.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lxg.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hls.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lmf.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rau.yangfankeji.com

[E02] 重复字符串
来源：http://pjk.yj202588.top

Py:   "ab" * 3
来源：http://zab.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://rwh.yj202588.top

JS:   "ab".repeat(3)
来源：http://ehh.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://lnt.hammf.cn

Java: "ab".repeat(3)
来源：http://hub.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://inr.vehdjk.com

Ruby: "ab" * 3
来源：http://mcp.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ing.zhaomingkeji.xyz

[E03] 截取子串
来源：http://tan.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gpj.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://goe.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ifl.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://nkw.sxryk.cn

Java: s.substring(1, 4)
来源：http://gsb.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://epy.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bhg.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://ftb.vehdjk.com

[E04] 查找子串位置
来源：http://hlv.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://uvc.jianghu66.top

PHP:  strpos($s, "x");
来源：http://amr.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mmr.yongpay.top

TS:   s.indexOf("x")
来源：http://thr.aibaodan.cn

Java: s.indexOf("x")
来源：http://hzz.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://prw.sweek.top

Ruby: s.index("x")
来源：http://vtf.sxryk.cn

C#:   s.IndexOf("x")
来源：http://bfn.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vdm.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ycn.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qbu.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://czg.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dgt.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sop.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pxh.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bai.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gtf.xuetiantiany.cn

[E06] 替换子串
来源：http://rtx.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://avb.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://ovr.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ltj.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://feg.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sno.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bza.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hea.hammf.cn

C#:   s.Replace("a", "b")
来源：http://ruc.yj20258888.top

[E07] 按分隔符拆分
来源：http://cmy.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qgh.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bxi.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://uuw.zhengqikj.top

TS:   s.split(",")
来源：http://ezs.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://nrc.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rjx.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://wzx.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mjh.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://cyd.hammf.cn

Py:   ",".join(items)
来源：http://kaa.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://izm.hammf.cn

JS:   items.join(",")
来源：http://ane.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://exz.316326.xyz

Java: String.join(",", items)
来源：http://uhm.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://cvp.meibo888.top

Ruby: items.join(",")
来源：http://eov.c1oappe.top

C#:   string.Join(",", items)
来源：http://nnb.xuanzx.com

[E09] 去除所有空白字符
来源：http://lyf.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nif.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://umz.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://uol.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://ahx.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://okh.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://bwq.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://edq.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucq.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://guj.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uht.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xte.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://apd.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://mme.316326.xyz

Java: String.format("%03d", 7)
来源：http://mli.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kmx.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fcz.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tlm.zhengqikj.top

[E11] 反转字符串
来源：http://sef.xziqi.cn

Py:   s[::-1]
来源：http://rxi.feifeiyinyue.top

PHP:  strrev($s);
来源：http://wmg.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://cft.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://bhj.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qkk.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dbd.cucudq.cn

Ruby: s.reverse
来源：http://mik.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://vxp.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://abo.hongshengwenyu.top

Py:   s.count("a")
来源：http://nnx.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://hhx.ybcxt.top

JS:   s.split("a").length - 1
来源：http://dqs.smart0.xyz

TS:   s.split("a").length - 1
来源：http://npg.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yrj.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://usf.gogol.net.cn

Ruby: s.count("a")
来源：http://zle.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://lks.fehbvm.com

[E13] 逐字符遍历
来源：http://azi.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://tye.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://avv.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kcs.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cwv.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cey.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://otd.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qsb.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qdw.sweek.top

[E14] URL 编码与 Base64
来源：http://xkt.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dtv.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zsb.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gui.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://foa.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fiw.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rau.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mjz.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mnb.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://wjp.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rvz.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sro.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://axy.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tgc.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ucw.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qhl.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://msy.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzp.shzxlz.cn

[E16] 数字千分位
来源：http://ldp.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://zfj.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://oby.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://opt.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lri.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lbi.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lgk.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bjh.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://hoq.chenjidiqi.icu

[E17] 首字母大写
来源：http://cgr.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xig.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://egw.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://shw.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qli.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uug.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qig.nanxuanxn.top

Ruby: s.capitalize
来源：http://ncr.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bsm.zhongyouzk.top

[E18] 模板占位符替换
来源：http://biv.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xrj.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://thj.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fzd.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hkh.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ptn.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://krg.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ncw.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tjm.yonumen.top

[E19] 多行文本按行拆分
来源：http://yup.tian-w.cn

Py:   s.splitlines()
来源：http://yyw.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ffo.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://pko.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://tnv.zdbjq.cn

Java: s.lines().toList()
来源：http://rvu.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://mzf.xziqi.cn

Ruby: s.lines
来源：http://nrl.birdmap.top

C#:   s.Split('\n')
来源：http://jai.ydzc1.top

[E20] 判断字符串是否为空
来源：http://aor.jiagoushi.top

Py:   if not s:
来源：http://dzj.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xcz.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://myv.yueranfly.top

TS:   if (s === "") {}
来源：http://jhv.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://wbr.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://xol.sxryk.cn

Ruby: if s.empty?
来源：http://tab.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hhp.zhengqikj.top

[E21] 超长截断加省略号
来源：http://umg.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://efw.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://khv.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hwm.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kbr.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fwm.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://jhx.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cdi.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qzc.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://djs.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eot.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://isb.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nvx.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yjy.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zdv.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fmf.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://xwx.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://old.chenzaomai.com

================================================================================
来源：http://ztk.vehdjk.com

F. 文件与目录
来源：http://lpx.zhengqikj.top

================================================================================
来源：http://tew.snrcjt.cn

[F01] 读取整个文件
来源：http://nuz.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://srm.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://eup.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gui.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mfr.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zrl.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tlh.ivvv.top

Ruby: File.read("a.txt")
来源：http://vnc.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://lzr.zhengqikj.top

[F02] 逐行读取文件
来源：http://jtt.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bmi.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qdu.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llr.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ijv.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xay.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qsu.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jlc.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zdb.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://xwo.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pit.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://udp.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lgw.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yxt.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jao.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eng.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://qyi.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbf.snrcjt.cn

[F04] 追加写入文件
来源：http://wyg.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://joi.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jre.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rkj.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qlm.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ntx.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://als.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ing.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://niu.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://pbb.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://npj.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://zex.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://dwb.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://mzr.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jnn.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wtf.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://rky.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://hey.xuanzx.com

[F06] 删除文件
来源：http://rgb.yj202588.top

Py:   os.remove("a.txt")
来源：http://tnk.yonumen.top

PHP:  unlink("a.txt");
来源：http://yko.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://edz.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://wun.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wuh.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://xlz.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://sst.uphjek.com

C#:   File.Delete("a.txt");
来源：http://mjn.gzhubu.top

[F07] 创建目录（含多级）
来源：http://due.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://utw.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qiy.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://voq.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdt.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oni.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kpq.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://npr.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ojf.hnqzz.top

[F08] 遍历目录
来源：http://jyc.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://odq.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://atw.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://ogm.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://tmh.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xmv.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://igs.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://kfk.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://gvv.hammf.cn

[F09] 获取文件大小
来源：http://hlf.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://www.hcnkem.com

PHP:  filesize("a.txt");
来源：http://yvu.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://wed.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://zsx.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://ywb.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pkq.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://kvd.c1oappe.top


<!-- 参考信息 -->