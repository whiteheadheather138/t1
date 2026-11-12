代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sxq.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://csk.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dtj.nanxinkj.top

[D26] 数组转字符串
来源：http://iwm.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://ghz.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://hor.yueranfly.top

JS:   arr.join(", ")
来源：http://kls.cashguo.top

TS:   arr.join(", ")
来源：http://qfy.gzhubu.top

Java: String.join(", ", list)
来源：http://eai.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://cof.52xcode.cn

Ruby: arr.join(", ")
来源：http://oxi.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://ifl.xinyue.icu

================================================================================
来源：http://iqu.yvedp.cn

E. 字符串处理
来源：http://wrd.jlsjyb.cn

================================================================================
来源：http://iwp.redwolf501.top

[E01] 拼接字符串
来源：http://eif.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ekc.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wof.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgf.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cly.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hnx.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vau.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://inn.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vjf.xuetiantiany.cn

[E02] 重复字符串
来源：http://wmn.jianghu66.top

Py:   "ab" * 3
来源：http://kos.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://ryy.fehbvm.com

JS:   "ab".repeat(3)
来源：http://hem.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://xar.0kj1m.cn

Java: "ab".repeat(3)
来源：http://jmf.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://lgl.daria6918.cn

Ruby: "ab" * 3
来源：http://duz.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rqm.pengpengdd.cyou

[E03] 截取子串
来源：http://ynd.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fmf.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://opo.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dbz.316326.xyz

TS:   s.slice(1, 4)
来源：http://ugn.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://nrh.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vid.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://sqb.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://sfe.sufxvd.cn

[E04] 查找子串位置
来源：http://cfq.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://zjr.316326.xyz

PHP:  strpos($s, "x");
来源：http://fan.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ifj.sysykeji.top

TS:   s.indexOf("x")
来源：http://zzk.iojbl.cn

Java: s.indexOf("x")
来源：http://lvi.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://loj.guowangkeji.top

Ruby: s.index("x")
来源：http://nzd.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://rll.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pvg.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lnc.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xdv.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpw.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ddt.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tai.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://een.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sgl.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uwo.chenjidiqi.icu

[E06] 替换子串
来源：http://nfh.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://utw.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://uyq.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfk.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://dmd.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tmb.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zzg.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ndq.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://vni.dashuyun.cn

[E07] 按分隔符拆分
来源：http://ckw.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tyl.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yqb.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxy.havefunace.top

TS:   s.split(",")
来源：http://dsa.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://yxh.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vjf.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://hdz.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cvy.havefunace.top

[E08] 数组按分隔符合并
来源：http://gkr.tarul.cn

Py:   ",".join(items)
来源：http://mzm.jyoumei.cn

PHP:  implode(",", $items);
来源：http://wvy.quarkkingdee.top

JS:   items.join(",")
来源：http://ukc.yonumen.top

TS:   items.join(",")
来源：http://yws.uphjek.com

Java: String.join(",", items)
来源：http://cdv.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://igf.iojbl.cn

Ruby: items.join(",")
来源：http://yuf.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://cxq.birdmap.top

[E09] 去除所有空白字符
来源：http://kxk.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dwb.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nay.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://ahz.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://hew.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://qgw.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tfw.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rgm.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yqv.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://iyb.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tdk.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://esy.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://eoi.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://gua.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://heu.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ckw.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nfu.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oki.shuidangran.top

[E11] 反转字符串
来源：http://imf.smart0.xyz

Py:   s[::-1]
来源：http://ora.chenjidiqi.icu

PHP:  strrev($s);
来源：http://juu.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://cwv.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://vok.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zsp.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eov.tian-w.cn

Ruby: s.reverse
来源：http://tdy.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://slw.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://iiu.hammf.cn

Py:   s.count("a")
来源：http://ocl.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://ryf.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://swp.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://ubm.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jnn.ivvv.top

Go:   strings.Count(s, "a")
来源：http://nui.tanke756.top

Ruby: s.count("a")
来源：http://mig.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://qro.aibaodan.cn

[E13] 逐字符遍历
来源：http://cdp.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://uoj.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ckv.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnd.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vdy.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://stx.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qjl.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://hxo.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hak.yongpay.top

[E14] URL 编码与 Base64
来源：http://yhi.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddd.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xnd.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cho.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ocp.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zjc.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ock.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hob.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fph.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://iie.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tev.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yoo.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nea.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jyj.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tdo.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hfk.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nka.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vma.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://moq.redwolf501.top

Py:   f"{1234567:,}"
来源：http://agt.iojbl.cn

PHP:  number_format(1234567);
来源：http://cpm.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lxf.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fak.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ong.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uav.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rjl.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://yzl.yonumen.top

[E17] 首字母大写
来源：http://jpr.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yvt.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://gni.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wjq.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dlh.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ynv.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cyz.fktsv.cn

Ruby: s.capitalize
来源：http://rnw.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hmn.hywenlv.cn

[E18] 模板占位符替换
来源：http://iej.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dnj.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://slx.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lkb.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zrj.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qto.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xig.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kof.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kje.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://ler.aizwys.cn

Py:   s.splitlines()
来源：http://mwi.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wrq.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://aqr.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://wai.zhijiandao.cn

Java: s.lines().toList()
来源：http://qde.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://wnv.jiagoushi.top

Ruby: s.lines
来源：http://btl.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://rzm.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://ona.guowangkeji.top

Py:   if not s:
来源：http://vup.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fvh.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://grm.jlsjyb.cn

TS:   if (s === "") {}
来源：http://dzf.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://ogg.xuanzx.com

Go:   if s == "" {}
来源：http://kfn.hysaishi.cn

Ruby: if s.empty?
来源：http://frj.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dgh.yangfankeji.com

[E21] 超长截断加省略号
来源：http://jrk.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eof.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ckk.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckc.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://anq.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sto.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://nry.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://imo.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zhx.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://twi.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pey.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhp.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cbp.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibu.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mwh.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qgv.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://hva.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rwm.zdqjudy.top

================================================================================
来源：http://odm.sjlbkw.cn

F. 文件与目录
来源：http://idh.c1oappe.top

================================================================================
来源：http://jpt.nwbrower.top

[F01] 读取整个文件
来源：http://epm.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lqm.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://npg.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xqr.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gji.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xts.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wzt.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://cei.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://aea.cashguo.top

[F02] 逐行读取文件
来源：http://eai.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lpi.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjt.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tct.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cct.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uub.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zjl.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tut.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xzs.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://eqf.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gxo.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rad.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lvw.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwc.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ais.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vsp.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://oil.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uqb.fengsongda.top

[F04] 追加写入文件
来源：http://yuv.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkc.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hht.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vtm.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sra.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mok.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tla.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uay.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ave.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://cbo.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tsi.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://ajw.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://hsw.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://ewh.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ldi.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tka.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://ysb.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://afy.gaohongyu789.top

[F06] 删除文件
来源：http://hpq.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://riz.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://uob.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qny.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zgl.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://odj.meibo888.top

Go:   os.Remove("a.txt")
来源：http://csm.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://lxb.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://nmp.tian-w.cn

[F07] 创建目录（含多级）
来源：http://ptn.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dlq.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sut.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvx.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtm.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sgx.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xzl.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rgv.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://owz.zhongyouzk.top

[F08] 遍历目录
来源：http://xzj.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yua.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zam.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://bff.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://gcl.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fya.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gxt.hnqzz.top

Ruby: Dir.children("dir")
来源：http://cxu.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://fxk.yvedp.cn

[F09] 获取文件大小
来源：http://olj.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://vdf.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://iji.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://pii.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://xmm.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://jfj.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbn.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://vbv.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://fze.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://dyu.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gai.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://enm.hesvh.cn


<!-- 参考信息 -->