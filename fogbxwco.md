代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://scw.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://fag.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://srf.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xnl.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oqi.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vwd.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xns.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gio.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mlo.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qwy.tarul.cn

[D25] Set 集合去重与交并差
来源：http://ltt.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zod.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pna.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftz.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wmn.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zas.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ciy.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cvy.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lfs.yj20258.top

[D26] 数组转字符串
来源：http://gde.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://rzw.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://byi.tian-w.cn

JS:   arr.join(", ")
来源：http://uxj.9152youxi.cn

TS:   arr.join(", ")
来源：http://sym.kuanghao11.cn

Java: String.join(", ", list)
来源：http://sqq.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://wwb.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://pmg.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://gwc.nwbrower.top

================================================================================
来源：http://unu.wangshuangyany.cn

E. 字符串处理
来源：http://kyu.xuetiantiany.cn

================================================================================
来源：http://rwo.vehdjk.com

[E01] 拼接字符串
来源：http://dih.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xyu.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hhf.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mfl.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zso.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rne.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rxf.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kpk.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uwn.shzxlz.cn

[E02] 重复字符串
来源：http://lud.tarul.cn

Py:   "ab" * 3
来源：http://aju.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://uta.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://pro.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://iqw.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://cly.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://omu.daxiang520.top

Ruby: "ab" * 3
来源：http://azf.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://chp.vehdjk.com

[E03] 截取子串
来源：http://rap.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hkm.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://szc.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zql.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://dkv.yj202588.top

Java: s.substring(1, 4)
来源：http://zth.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bce.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tqm.cashguo.top

C#:   s.Substring(1, 3)
来源：http://yze.kuanghao11.cn

[E04] 查找子串位置
来源：http://hbn.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://vad.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://gel.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ahk.ppjwa.cn

TS:   s.indexOf("x")
来源：http://fvo.52xcode.cn

Java: s.indexOf("x")
来源：http://cgf.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://uto.birdmap.top

Ruby: s.index("x")
来源：http://ctb.hesvh.cn

C#:   s.IndexOf("x")
来源：http://gwp.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nfa.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nxw.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eud.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lii.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nam.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mad.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vte.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nzc.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hdm.zhaomingkeji.xyz

[E06] 替换子串
来源：http://deg.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://plo.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://yfg.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://log.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://aul.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cwu.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cpz.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://isu.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://nge.cucudq.cn

[E07] 按分隔符拆分
来源：http://lfo.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zmp.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jjy.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://akm.jlsjyb.cn

TS:   s.split(",")
来源：http://xwv.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wkj.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qxu.tarul.cn

Ruby: s.split(",");  s.split
来源：http://wxg.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bwg.tanke756.top

[E08] 数组按分隔符合并
来源：http://vwr.jiagoushi.top

Py:   ",".join(items)
来源：http://hdn.bjfxy.top

PHP:  implode(",", $items);
来源：http://zxg.redwolf501.top

JS:   items.join(",")
来源：http://axq.gogol.net.cn

TS:   items.join(",")
来源：http://vsx.yuxming.cn

Java: String.join(",", items)
来源：http://qtm.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://dfb.dashuyun.cn

Ruby: items.join(",")
来源：http://pvz.iojbl.cn

C#:   string.Join(",", items)
来源：http://vhv.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://nwu.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://byy.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vrz.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://pmc.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://bbe.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://pwm.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyg.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ria.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bfp.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://zcq.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dku.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oma.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://jtk.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://qab.zycfv.cn

Java: String.format("%03d", 7)
来源：http://jan.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://shv.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zex.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ifw.iojbl.cn

[E11] 反转字符串
来源：http://dhz.aibaodan.cn

Py:   s[::-1]
来源：http://gun.zycfv.cn

PHP:  strrev($s);
来源：http://drr.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ois.hammf.cn

TS:   [...s].reverse().join("")
来源：http://bif.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://esy.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cmu.hesvh.cn

Ruby: s.reverse
来源：http://svc.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://imu.fktsv.cn

[E12] 统计某字符出现次数
来源：http://mzg.vehdjk.com

Py:   s.count("a")
来源：http://jex.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://rns.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://vam.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://ymr.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tqb.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://uif.dashuyun.cn

Ruby: s.count("a")
来源：http://msi.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://rne.hesvh.cn

[E13] 逐字符遍历
来源：http://ijn.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://xhi.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://llu.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bui.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ljm.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jmz.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hej.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dbf.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xzi.bjfxy.top

[E14] URL 编码与 Base64
来源：http://sdn.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://trn.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zdj.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dkw.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnn.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zgz.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hnf.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvt.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rob.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://osk.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gwt.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qbd.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://duf.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aic.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zeq.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://erb.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kxi.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wbf.kuanghao11.cn

[E16] 数字千分位
来源：http://sbw.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://xwa.52xcode.cn

PHP:  number_format(1234567);
来源：http://vuv.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://zgh.aibaodan.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kes.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://imw.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spa.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dnb.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://lhg.hesvh.cn

[E17] 首字母大写
来源：http://pyu.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rnb.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hro.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jln.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsw.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mvf.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ukq.gogol.net.cn

Ruby: s.capitalize
来源：http://vod.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rfi.yueranfly.top

[E18] 模板占位符替换
来源：http://xxr.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://smq.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://myi.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://usp.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://axw.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://asc.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kcc.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://duo.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dfa.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://jcy.zhongyouzk.top

Py:   s.splitlines()
来源：http://zzt.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zpj.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://pki.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://pcj.sweek.top

Java: s.lines().toList()
来源：http://qbw.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://edg.hammf.cn

Ruby: s.lines
来源：http://knl.tanke756.top

C#:   s.Split('\n')
来源：http://qej.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://xgv.sxryk.cn

Py:   if not s:
来源：http://agz.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgl.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhh.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://apl.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://tpb.fehbvm.com

Go:   if s == "" {}
来源：http://fny.yonumen.top

Ruby: if s.empty?
来源：http://kul.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xty.cucudq.cn

[E21] 超长截断加省略号
来源：http://axx.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://afz.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://evd.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oay.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nir.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tfn.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://kdw.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zzf.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eta.zycfv.cn

[E22] 字节长度与字符长度
来源：http://myu.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhs.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hrk.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://quj.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hay.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pwi.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ich.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://wtj.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fdy.hnxiangtu.top

================================================================================
来源：http://zow.chenjidiqi.icu

F. 文件与目录
来源：http://sss.dianchejie.cn

================================================================================
来源：http://yab.epnwcf.com

[F01] 读取整个文件
来源：http://lbd.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ahu.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://tbo.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xoc.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zhy.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ksz.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ldk.havefunace.top

Ruby: File.read("a.txt")
来源：http://rwf.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://arx.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://iyc.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kqi.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://njg.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ylx.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xak.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tql.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://psv.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://skw.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://neo.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://ddv.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ivv.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fyw.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://otd.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gce.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fue.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxl.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://vjx.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iud.shuidangran.top

[F04] 追加写入文件
来源：http://lqp.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uya.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uec.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqm.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nyn.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://byf.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://smf.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cet.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tow.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://ols.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ubh.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://hao.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://dwx.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://lis.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ljj.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xjo.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://lxz.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://nxb.fehbvm.com

[F06] 删除文件
来源：http://rrd.cashguo.top

Py:   os.remove("a.txt")
来源：http://wqg.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://nle.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ung.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://iap.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kmv.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://azt.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://jmv.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://vzy.bjfxy.top

[F07] 创建目录（含多级）
来源：http://bbj.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qro.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pjn.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mbi.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mwd.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uhi.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aix.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ngn.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yct.jianghu66.top

[F08] 遍历目录
来源：http://qif.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qjs.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ndt.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://teb.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://hib.yuxming.cn


<!-- 参考信息 -->