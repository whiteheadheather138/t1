代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udh.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zyl.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbh.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nyd.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tek.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ygg.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tal.zhoulong.xyz

[D26] 数组转字符串
来源：http://rrn.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://mnt.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://qhn.redwolf501.top

JS:   arr.join(", ")
来源：http://nxy.sxryk.cn

TS:   arr.join(", ")
来源：http://bmk.chenlongwang.top

Java: String.join(", ", list)
来源：http://mml.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://sly.cucudq.cn

Ruby: arr.join(", ")
来源：http://nhn.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://yuc.yj202588.top

================================================================================
来源：http://dub.nwbrower.top

E. 字符串处理
来源：http://inj.zhongyouzk.top

================================================================================
来源：http://cfn.feifeiyinyue.top

[E01] 拼接字符串
来源：http://afz.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vjd.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pys.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ckd.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://djp.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gyb.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qes.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ijk.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://upy.quarkkingdee.top

[E02] 重复字符串
来源：http://hzq.xziqi.cn

Py:   "ab" * 3
来源：http://qcb.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://ouy.fktsv.cn

JS:   "ab".repeat(3)
来源：http://jpx.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://dlr.gotoacloud.top

Java: "ab".repeat(3)
来源：http://nrd.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://vrn.zhoulong.xyz

Ruby: "ab" * 3
来源：http://rix.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vox.birdmap.top

[E03] 截取子串
来源：http://ais.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bnf.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://etl.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ufh.xziqi.cn

TS:   s.slice(1, 4)
来源：http://rwt.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://prx.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uto.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jzk.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://ikr.9152youxi.cn

[E04] 查找子串位置
来源：http://zid.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://zkj.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://bww.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xsn.wangdashe.top

TS:   s.indexOf("x")
来源：http://ueb.haohaochexian.top

Java: s.indexOf("x")
来源：http://oxc.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://wzm.hcnkem.com

Ruby: s.index("x")
来源：http://lrj.xinyue.icu

C#:   s.IndexOf("x")
来源：http://hai.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://esf.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yma.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eof.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vzs.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lbf.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhd.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hmi.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vax.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bre.yuanzhike.top

[E06] 替换子串
来源：http://qkk.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wpb.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://ugt.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sir.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://iki.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://szs.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gvv.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cww.pycfn.com

C#:   s.Replace("a", "b")
来源：http://ici.vehdjk.com

[E07] 按分隔符拆分
来源：http://gxn.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://whs.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nyh.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qpm.vehdjk.com

TS:   s.split(",")
来源：http://hjc.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tmz.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xgv.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://mix.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://csa.mhx1999.top

[E08] 数组按分隔符合并
来源：http://hrl.jqgufenzy.top

Py:   ",".join(items)
来源：http://ozb.yueranfly.top

PHP:  implode(",", $items);
来源：http://pmw.zhixingplan.top

JS:   items.join(",")
来源：http://gxy.sxryk.cn

TS:   items.join(",")
来源：http://oxw.sysykeji.top

Java: String.join(",", items)
来源：http://mca.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://otq.hnxiangtu.top

Ruby: items.join(",")
来源：http://ubo.sweek.top

C#:   string.Join(",", items)
来源：http://sbm.xziqi.cn

[E09] 去除所有空白字符
来源：http://xyb.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zpx.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://btr.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://gqg.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://ggj.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://uxb.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rfs.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://xno.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://spo.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://fdh.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vnq.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kdy.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://xkx.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://cuu.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://pzf.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvw.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ohp.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tbu.316326.xyz

[E11] 反转字符串
来源：http://ald.aibaodan.cn

Py:   s[::-1]
来源：http://fjo.redwolf501.top

PHP:  strrev($s);
来源：http://jsq.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://kcj.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://qrb.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lio.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mwz.xuanzx.com

Ruby: s.reverse
来源：http://pge.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://hhk.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://mkf.yj202588.top

Py:   s.count("a")
来源：http://jwc.yonumen.top

PHP:  substr_count($s, "a");
来源：http://kns.yuxming.cn

JS:   s.split("a").length - 1
来源：http://eyx.hammf.cn

TS:   s.split("a").length - 1
来源：http://uro.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mlg.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://yul.xuetiantiany.cn

Ruby: s.count("a")
来源：http://nza.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://xzx.xziqi.cn

[E13] 逐字符遍历
来源：http://fit.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://fob.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://amz.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fyg.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://yvv.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwz.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krf.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://acc.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qoe.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://aic.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://twx.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://nyo.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ymf.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fjn.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vgq.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vym.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kwj.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxc.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://aey.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ttb.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qsr.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qtm.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bso.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sbe.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sbo.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mjh.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qdv.zhijiandao.cn

[E16] 数字千分位
来源：http://wqs.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://ooa.smart0.xyz

PHP:  number_format(1234567);
来源：http://ldu.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kmm.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kmb.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ifx.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://muw.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ghi.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://hmc.ydjk.org.cn

[E17] 首字母大写
来源：http://ynb.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uuu.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ddw.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upj.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ppm.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kip.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qge.yuxming.cn

Ruby: s.capitalize
来源：http://yom.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ztn.ybcxt.top

[E18] 模板占位符替换
来源：http://uyl.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqf.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xal.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bix.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fst.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gak.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ora.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jud.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nhw.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://vzl.c1oappe.top

Py:   s.splitlines()
来源：http://rmw.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://doh.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://nmh.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://gfr.ctjpmb.com

Java: s.lines().toList()
来源：http://iuq.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://lsf.ywan-chungtsiang.top

Ruby: s.lines
来源：http://dxk.xinyue.icu

C#:   s.Split('\n')
来源：http://wrr.cashguo.top

[E20] 判断字符串是否为空
来源：http://khk.9152youxi.cn

Py:   if not s:
来源：http://dbc.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rrd.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kfb.jiagoushi.top

TS:   if (s === "") {}
来源：http://mad.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://nve.epnwcf.com

Go:   if s == "" {}
来源：http://krp.vehdjk.com

Ruby: if s.empty?
来源：http://puu.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nvs.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://nqe.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lxc.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ouy.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ifn.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpf.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bzh.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://wxt.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jvj.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://diq.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://ovg.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nvc.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvl.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mbn.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozj.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jzj.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zce.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://fui.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vfy.shuidangran.top

================================================================================
来源：http://dmi.hywenlv.cn

F. 文件与目录
来源：http://kcz.jyoumei.cn

================================================================================
来源：http://bjg.ctjpmb.com

[F01] 读取整个文件
来源：http://vvw.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://utx.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://etp.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iyc.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zax.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fql.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tcy.sweek.top

Ruby: File.read("a.txt")
来源：http://dla.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://fac.iojbl.cn

[F02] 逐行读取文件
来源：http://hse.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ked.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qne.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhe.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swk.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pnq.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iam.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://del.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://chp.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://huz.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mua.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://btg.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rab.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://djs.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ptp.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ljq.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://dng.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://txs.zdqjudy.top

[F04] 追加写入文件
来源：http://grx.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://brn.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wjk.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ldy.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpx.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://utm.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iip.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vat.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nnh.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://zph.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gqb.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://mqu.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://kzi.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://lxz.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://htz.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhq.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://aup.tanke756.top

C#:   File.Exists("a.txt")
来源：http://kpf.wangdashe.top

[F06] 删除文件
来源：http://dsk.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://ugi.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://qpx.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wau.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://hef.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fjj.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://kug.tarul.cn

Ruby: File.delete("a.txt")
来源：http://rvk.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://bms.guannengcc.top

[F07] 创建目录（含多级）
来源：http://jkb.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sxo.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tju.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nak.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hcx.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://erf.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rse.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zrd.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dqm.yuanzhike.top

[F08] 遍历目录
来源：http://rxd.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kzm.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jpe.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://ipb.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://lnn.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://acq.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhg.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://lym.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://ini.bjfxy.top

[F09] 获取文件大小
来源：http://zjq.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://evy.cheryme.top

PHP:  filesize("a.txt");
来源：http://mco.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://weh.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://gal.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://nvh.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jmb.wangdashe.top

Ruby: File.size("a.txt")
来源：http://maw.chenjidiqi.icu


<!-- 参考信息 -->