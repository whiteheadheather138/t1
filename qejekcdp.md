代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xxs.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hbq.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uui.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hbt.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://apw.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xjt.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lgn.havefunace.top

[D26] 数组转字符串
来源：http://exh.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://lws.havefunace.top

PHP:  implode(", ", $arr);
来源：http://mvf.zhijiandao.cn

JS:   arr.join(", ")
来源：http://gxx.sufxvd.cn

TS:   arr.join(", ")
来源：http://gsu.cdnleiting.top

Java: String.join(", ", list)
来源：http://vsl.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://xbq.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://yyh.bbcook.cn

C#:   string.Join(", ", list)
来源：http://mwv.sufxvd.cn

================================================================================
来源：http://kse.tianlin.xyz

E. 字符串处理
来源：http://rmx.hesvh.cn

================================================================================
来源：http://gnm.tanke756.top

[E01] 拼接字符串
来源：http://izs.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hdm.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://huo.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bcs.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jax.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wpz.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vbj.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jfv.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxz.zdqjudy.top

[E02] 重复字符串
来源：http://ywg.sxryk.cn

Py:   "ab" * 3
来源：http://xqh.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://fbw.epnwcf.com

JS:   "ab".repeat(3)
来源：http://zmf.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://mse.birdmap.top

Java: "ab".repeat(3)
来源：http://zsd.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://kiw.cheryme.top

Ruby: "ab" * 3
来源：http://qmd.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://prt.0kj1m.cn

[E03] 截取子串
来源：http://wrn.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jqa.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jsm.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oky.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://ubn.yueranfly.top

Java: s.substring(1, 4)
来源：http://geb.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fgs.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://knw.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://mqm.ydzc1.top

[E04] 查找子串位置
来源：http://czg.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://jem.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://rup.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tuv.nanxinkj.top

TS:   s.indexOf("x")
来源：http://fuq.hywenlv.cn

Java: s.indexOf("x")
来源：http://wqw.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://mgv.zhixingplan.top

Ruby: s.index("x")
来源：http://jxj.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://kio.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qvo.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqw.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ajd.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hth.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ayw.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rtl.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pgm.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bqe.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jcy.dashuyun.cn

[E06] 替换子串
来源：http://tlr.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://upd.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://xan.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ccf.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://eom.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggz.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://evj.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ozt.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://ucq.fzhhl.top

[E07] 按分隔符拆分
来源：http://dme.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pjh.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mhs.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ups.sweek.top

TS:   s.split(",")
来源：http://wna.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://mtw.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cgn.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://xii.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iay.birdmap.top

[E08] 数组按分隔符合并
来源：http://pqz.vqdsnc.cn

Py:   ",".join(items)
来源：http://kva.kuanghao11.cn

PHP:  implode(",", $items);
来源：http://neh.xuanzx.com

JS:   items.join(",")
来源：http://ttq.iojbl.cn

TS:   items.join(",")
来源：http://odg.zdqjudy.top

Java: String.join(",", items)
来源：http://wwa.316326.xyz

Go:   strings.Join(items, ",")
来源：http://esc.hammf.cn

Ruby: items.join(",")
来源：http://auq.pycfn.com

C#:   string.Join(",", items)
来源：http://agt.zdqjudy.top

[E09] 去除所有空白字符
来源：http://rvi.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://woy.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mbp.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://hyp.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://bnf.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://rvi.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vhu.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://jzk.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://clp.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://ssr.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nkr.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://trh.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://uxj.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://muz.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://vab.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dij.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ynp.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://agf.zdbjq.cn

[E11] 反转字符串
来源：http://tno.shzxlz.cn

Py:   s[::-1]
来源：http://fxt.vqdsnc.cn

PHP:  strrev($s);
来源：http://mgk.hammf.cn

JS:   [...s].reverse().join("")
来源：http://pew.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://ouu.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://cea.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://msb.yangfankeji.com

Ruby: s.reverse
来源：http://uam.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ghm.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://hgr.yvedp.cn

Py:   s.count("a")
来源：http://ynw.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://xuh.daxiang520.top

JS:   s.split("a").length - 1
来源：http://avx.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://ekl.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mce.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://gpx.gzhubu.top

Ruby: s.count("a")
来源：http://esh.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://kro.vqdsnc.cn

[E13] 逐字符遍历
来源：http://uhg.tarul.cn

Py:   for ch in s: print(ch)
来源：http://nus.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rib.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tkj.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://und.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lsh.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ecq.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pla.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vwc.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://yfr.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nao.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nth.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bou.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://luk.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mwo.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lze.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nsk.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://crd.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://ysd.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ede.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aou.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lyf.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://knj.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mdj.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fdj.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://icc.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rjt.shzxlz.cn

[E16] 数字千分位
来源：http://mys.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://hzm.tarul.cn

PHP:  number_format(1234567);
来源：http://dax.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wyn.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qwm.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rqf.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qpg.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ivg.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://ofi.yj202588.top

[E17] 首字母大写
来源：http://wxg.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bao.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xww.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uxx.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjc.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uny.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nac.smart0.xyz

Ruby: s.capitalize
来源：http://ftu.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nme.havefunace.top

[E18] 模板占位符替换
来源：http://qmq.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://btl.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aaf.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://trp.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hvg.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aim.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxi.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wsc.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ldo.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://ehu.hfpthk.cn

Py:   s.splitlines()
来源：http://yjx.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xnp.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://odf.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://siv.shangyingyoupin.top

Java: s.lines().toList()
来源：http://wnn.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://enq.52xcode.cn

Ruby: s.lines
来源：http://sln.meibo888.top

C#:   s.Split('\n')
来源：http://rrw.yongpay.top

[E20] 判断字符串是否为空
来源：http://ysd.chenjidiqi.icu

Py:   if not s:
来源：http://jmr.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bgu.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hhx.jiagoushi.top

TS:   if (s === "") {}
来源：http://wzq.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://jri.zycfv.cn

Go:   if s == "" {}
来源：http://twm.svipenyu.cn

Ruby: if s.empty?
来源：http://ydr.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jkz.yj202588.top

[E21] 超长截断加省略号
来源：http://jkl.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lvp.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://myw.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aws.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yhe.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ops.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://vbo.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lzp.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eed.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://ffn.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pdz.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mbv.svipenyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iww.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://djp.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iha.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tsv.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://hjy.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xfl.ivvv.top

================================================================================
来源：http://mjc.ehwqpu.com

F. 文件与目录
来源：http://tdw.feifeiyinyue.top

================================================================================
来源：http://psm.zycfv.cn

[F01] 读取整个文件
来源：http://uhg.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://plv.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://atf.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zcb.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zfr.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cyz.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dhl.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://iot.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://ify.havefunace.top

[F02] 逐行读取文件
来源：http://dad.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dfw.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vhq.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ioj.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dbe.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jjg.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xqm.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cpk.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cor.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://qvx.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fqi.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsv.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xsw.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwj.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lsn.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ekm.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://hpx.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jay.hywenlv.cn

[F04] 追加写入文件
来源：http://tkn.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pnt.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wrc.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhs.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pfg.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://szf.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fln.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rhw.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oao.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://cjn.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zdb.yonumen.top

PHP:  file_exists("a.txt");
来源：http://dyu.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://tgv.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://xaj.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rbw.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ftu.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://vuk.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://jyq.vqdsnc.cn

[F06] 删除文件
来源：http://ond.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://fac.tanke756.top

PHP:  unlink("a.txt");
来源：http://vfr.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rsc.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://bvc.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pfk.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://ztp.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://sgp.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://cim.tarul.cn

[F07] 创建目录（含多级）
来源：http://wwe.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gez.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kxn.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvy.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://azq.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rxd.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vog.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hum.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xoe.gogol.net.cn

[F08] 遍历目录
来源：http://xzs.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uci.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ijw.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://dtm.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://tyc.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vxe.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jgs.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://trr.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://mbo.jqgfzy.top

[F09] 获取文件大小
来源：http://dat.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://xiv.yonumen.top

PHP:  filesize("a.txt");
来源：http://clt.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://cwy.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://jus.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://ran.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cjx.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://zmr.316326.xyz


<!-- 参考信息 -->