代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zlb.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qyv.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://opw.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://osh.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jxe.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rlo.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rzs.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://arm.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tcn.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vik.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtd.vqdsnc.cn

[D26] 数组转字符串
来源：http://vyg.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://tek.cheryme.top

PHP:  implode(", ", $arr);
来源：http://qai.xziqi.cn

JS:   arr.join(", ")
来源：http://mwi.cheryme.top

TS:   arr.join(", ")
来源：http://qdc.vqdsnc.cn

Java: String.join(", ", list)
来源：http://boa.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://sxa.xinyue.icu

Ruby: arr.join(", ")
来源：http://hdz.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://vzl.shzxlz.cn

================================================================================
来源：http://qzw.hnqzz.top

E. 字符串处理
来源：http://ewn.ywan-chungtsiang.top

================================================================================
来源：http://sfx.vqdsnc.cn

[E01] 拼接字符串
来源：http://ahs.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vnk.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yrn.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aoz.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqk.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cha.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qef.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eaf.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ywd.9152youxi.cn

[E02] 重复字符串
来源：http://dri.yanxiufei.cn

Py:   "ab" * 3
来源：http://qgw.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://nzp.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://imm.aizwys.cn

TS:   "ab".repeat(3)
来源：http://clb.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://sds.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://ycq.hywenlv.cn

Ruby: "ab" * 3
来源：http://hcp.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ent.jinyuanbaomall.cn

[E03] 截取子串
来源：http://fah.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jcb.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kbz.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://szi.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://yst.snrcjt.cn

Java: s.substring(1, 4)
来源：http://sxb.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://krs.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://fon.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://opa.cucudq.cn

[E04] 查找子串位置
来源：http://kwj.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://vua.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://nbj.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vli.ybcxt.top

TS:   s.indexOf("x")
来源：http://zhj.0kj1m.cn

Java: s.indexOf("x")
来源：http://fnq.yj20258.top

Go:   strings.Index(s, "x")
来源：http://mwm.vqdsnc.cn

Ruby: s.index("x")
来源：http://ujl.fengsongda.top

C#:   s.IndexOf("x")
来源：http://dvn.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iiv.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://csu.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ntv.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kur.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://dxj.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ymv.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iek.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kxw.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pcm.fehbvm.com

[E06] 替换子串
来源：http://ywv.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgo.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://mog.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yww.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://zzd.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jlt.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fqt.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kvr.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://owz.sufxvd.cn

[E07] 按分隔符拆分
来源：http://zqu.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zyu.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lwv.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eao.quarkkingdee.top

TS:   s.split(",")
来源：http://vwo.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kkl.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dsl.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://jsq.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ind.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://acv.jinqigfzy.top

Py:   ",".join(items)
来源：http://wbi.aizwys.cn

PHP:  implode(",", $items);
来源：http://gnj.ydjk.org.cn

JS:   items.join(",")
来源：http://eft.hongshengwenyu.top

TS:   items.join(",")
来源：http://dqw.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://xer.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://puk.gogol.net.cn

Ruby: items.join(",")
来源：http://nmm.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://pgp.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://xep.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xeh.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uce.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://bhg.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://ktr.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://rhs.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uag.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://aoh.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fnw.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://fqq.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gah.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vip.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://tzr.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://rfk.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://nvz.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddd.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ftl.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uwv.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://jyq.yj20258888.top

Py:   s[::-1]
来源：http://tzb.nanxuanxn.top

PHP:  strrev($s);
来源：http://liu.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://bsl.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://lae.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://olf.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxp.ctjpmb.com

Ruby: s.reverse
来源：http://gyk.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://kzw.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://lxi.cdnleiting.top

Py:   s.count("a")
来源：http://eua.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://wru.bbcook.cn

JS:   s.split("a").length - 1
来源：http://xdk.hesvh.cn

TS:   s.split("a").length - 1
来源：http://rzi.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjd.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://jas.sufxvd.cn

Ruby: s.count("a")
来源：http://bou.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://drj.yj20258.top

[E13] 逐字符遍历
来源：http://lux.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://dum.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bql.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhn.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qkr.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xar.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sco.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lqi.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hgg.tian-w.cn

[E14] URL 编码与 Base64
来源：http://ywd.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wlj.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sqp.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rru.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nrs.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wli.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fdb.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lnq.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wls.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://ofo.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mjn.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmq.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vym.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lgs.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lxp.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yka.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kjp.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jcn.cqqwz.cn

[E16] 数字千分位
来源：http://lez.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://pbn.yongpay.top

PHP:  number_format(1234567);
来源：http://rcn.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vbw.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tqq.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lia.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xik.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://usu.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://foc.xuetiantiany.cn

[E17] 首字母大写
来源：http://jih.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ipz.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dxg.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iho.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://itv.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oaq.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rpx.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://nnv.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lnp.gotoacloud.top

[E18] 模板占位符替换
来源：http://agk.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ajf.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jjk.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jgz.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ord.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rxh.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ujt.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lgh.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywv.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://mmi.wangshuangyany.cn

Py:   s.splitlines()
来源：http://vne.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jwk.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://krr.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://tfw.zhengqikj.top

Java: s.lines().toList()
来源：http://ide.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://kah.ivvv.top

Ruby: s.lines
来源：http://xbz.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://fre.sxryk.cn

[E20] 判断字符串是否为空
来源：http://ctl.yfazqb.com

Py:   if not s:
来源：http://mzt.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vuw.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://crb.hesvh.cn

TS:   if (s === "") {}
来源：http://qml.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://kxp.tian-w.cn

Go:   if s == "" {}
来源：http://yxy.yueranfly.top

Ruby: if s.empty?
来源：http://hfn.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://air.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://lui.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xbj.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jxb.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xkl.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lhe.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qbs.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://xkg.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://naf.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wbx.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://urj.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xgr.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxj.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xix.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwp.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ble.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fxv.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://qro.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pfb.zdbjq.cn

================================================================================
来源：http://aqn.hcnkem.com

F. 文件与目录
来源：http://lrf.ywan-chungtsiang.top

================================================================================
来源：http://due.yj202588.top

[F01] 读取整个文件
来源：http://dni.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kbb.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ays.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gbd.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fgf.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tze.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qvy.aizwys.cn

Ruby: File.read("a.txt")
来源：http://xbl.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://brf.ppjwa.cn

[F02] 逐行读取文件
来源：http://xxn.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ssr.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aoh.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ree.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyc.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zzf.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://djl.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cjb.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hmq.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://she.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://txd.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hbb.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hrn.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kam.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ymq.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fuc.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://tyt.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hjc.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://gio.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ecw.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vdl.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zcm.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imx.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xlk.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://stu.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eoj.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vos.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://wal.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wvg.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://fbe.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://cze.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://ikh.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tev.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jsp.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://iqh.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://kty.xylfe.cn

[F06] 删除文件
来源：http://ipt.sweek.top

Py:   os.remove("a.txt")
来源：http://fjt.daria6918.cn

PHP:  unlink("a.txt");
来源：http://pcx.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nvb.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fad.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wqd.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://yhd.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://wna.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://kvo.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://qfn.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aoi.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tot.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rwo.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ltv.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zac.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oya.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qhl.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yrq.yueranfly.top

[F08] 遍历目录
来源：http://yee.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://edz.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hdq.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://qcu.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://gxy.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zax.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://igo.xuanzx.com

Ruby: Dir.children("dir")
来源：http://llb.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://vuz.c1oappe.top

[F09] 获取文件大小
来源：http://wph.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://ywu.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://bhh.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://dmt.sjlbkw.cn


<!-- 参考信息 -->