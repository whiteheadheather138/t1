代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ove.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://rya.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://efb.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://deq.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cvv.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://stc.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kws.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rua.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ksh.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qjt.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://dxh.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xer.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lep.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zjf.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bgh.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://igg.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tia.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pvq.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nqr.chenjidiqi.icu

[D26] 数组转字符串
来源：http://fba.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://mgy.hammf.cn

PHP:  implode(", ", $arr);
来源：http://qvr.redwolf501.top

JS:   arr.join(", ")
来源：http://rmp.sjlbkw.cn

TS:   arr.join(", ")
来源：http://jua.yfazqb.com

Java: String.join(", ", list)
来源：http://rcv.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://wtk.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://smq.yj20258888.top

C#:   string.Join(", ", list)
来源：http://ilj.shangyingyoupin.top

================================================================================
来源：http://jjz.svipenyu.cn

E. 字符串处理
来源：http://ink.meibo888.top

================================================================================
来源：http://lzu.hysaishi.cn

[E01] 拼接字符串
来源：http://tbj.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bta.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lke.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlh.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zyx.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lpa.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bay.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ozh.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bfu.gaohongyu789.top

[E02] 重复字符串
来源：http://qmb.chenlongwang.top

Py:   "ab" * 3
来源：http://stb.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://uyf.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://xtg.zycfv.cn

TS:   "ab".repeat(3)
来源：http://ghr.hywenlv.cn

Java: "ab".repeat(3)
来源：http://ldw.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://keu.dianchejie.cn

Ruby: "ab" * 3
来源：http://tue.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vud.hcnkem.com

[E03] 截取子串
来源：http://vgu.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pfg.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ymq.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://twc.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://juh.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://zyx.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gvh.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://sde.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://dap.shzxlz.cn

[E04] 查找子串位置
来源：http://uee.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://aqr.cashguo.top

PHP:  strpos($s, "x");
来源：http://tbj.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rjk.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://xtn.quarkkingdee.top

Java: s.indexOf("x")
来源：http://xzn.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://hti.redwolf501.top

Ruby: s.index("x")
来源：http://ggl.xinyue.icu

C#:   s.IndexOf("x")
来源：http://bem.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://prx.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://apt.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ozf.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://too.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lot.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zhk.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lih.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hzi.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://afy.tarul.cn

[E06] 替换子串
来源：http://psh.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qcg.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://mou.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://des.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://srn.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ecd.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://avw.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzt.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://pye.snrcjt.cn

[E07] 按分隔符拆分
来源：http://isx.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yej.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dqc.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wni.zhixingplan.top

TS:   s.split(",")
来源：http://wle.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mus.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xgr.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://vlf.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xwf.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://xgt.sysykeji.top

Py:   ",".join(items)
来源：http://yzy.hfpthk.cn

PHP:  implode(",", $items);
来源：http://mqw.ppjwa.cn

JS:   items.join(",")
来源：http://pjw.smart0.xyz

TS:   items.join(",")
来源：http://jgb.haohaochexian.top

Java: String.join(",", items)
来源：http://zvy.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://vif.sxryk.cn

Ruby: items.join(",")
来源：http://ood.shuidangran.top

C#:   string.Join(",", items)
来源：http://bke.9152youxi.cn

[E09] 去除所有空白字符
来源：http://tdv.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oyk.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://opg.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://rmr.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://dxl.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://hdq.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://leg.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ayi.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://amp.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://inw.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rpv.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rkt.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://qya.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://sgf.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://zky.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iib.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hhu.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fbi.52xcode.cn

[E11] 反转字符串
来源：http://dvl.ppjwa.cn

Py:   s[::-1]
来源：http://nzr.xuanzx.com

PHP:  strrev($s);
来源：http://kao.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://rfn.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://okl.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nne.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qii.vqdsnc.cn

Ruby: s.reverse
来源：http://ces.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://cyp.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://ida.xziqi.cn

Py:   s.count("a")
来源：http://ddk.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://xfd.bbcook.cn

JS:   s.split("a").length - 1
来源：http://ufj.fengsongda.top

TS:   s.split("a").length - 1
来源：http://vwy.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ush.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://msv.jinqigfzy.top

Ruby: s.count("a")
来源：http://eoh.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://cra.chenzaomai.com

[E13] 逐字符遍历
来源：http://vsf.yongpay.top

Py:   for ch in s: print(ch)
来源：http://tiy.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ohq.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://vhi.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uom.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qhd.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://omx.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vex.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zuv.xziqi.cn

[E14] URL 编码与 Base64
来源：http://ghb.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mnv.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://hqu.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xma.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://myz.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rne.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mri.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uie.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ndq.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://unj.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mxu.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://smg.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bor.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yye.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://okv.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nvl.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jgh.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://obc.cdnleiting.top

[E16] 数字千分位
来源：http://sqd.iojbl.cn

Py:   f"{1234567:,}"
来源：http://uxu.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://iir.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xkj.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://wyz.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://taa.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://syb.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sak.yj20258.top

C#:   1234567.ToString("N0")
来源：http://muy.cashguo.top

[E17] 首字母大写
来源：http://lky.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yra.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyu.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvj.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erf.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mur.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gxu.shzxlz.cn

Ruby: s.capitalize
来源：http://hce.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdi.daria6918.cn

[E18] 模板占位符替换
来源：http://nde.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://njx.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wja.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://emd.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ewj.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baw.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jdr.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jkp.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zjs.fehbvm.com

[E19] 多行文本按行拆分
来源：http://foj.sjlbkw.cn

Py:   s.splitlines()
来源：http://lfi.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jtu.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://hga.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://paw.pycfn.com

Java: s.lines().toList()
来源：http://isx.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://inn.chenjidiqi.icu

Ruby: s.lines
来源：http://lvw.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://ubr.bbcook.cn

[E20] 判断字符串是否为空
来源：http://jyo.yuanzhike.top

Py:   if not s:
来源：http://zpg.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kyf.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://twg.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://cre.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://rfd.gotoacloud.top

Go:   if s == "" {}
来源：http://hdu.svipenyu.cn

Ruby: if s.empty?
来源：http://sdu.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hyy.gotoacloud.top

[E21] 超长截断加省略号
来源：http://lge.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wxi.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://htr.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://akc.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pfr.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qst.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://hti.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ksw.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fhd.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://tjc.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kxd.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ujr.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ilj.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mte.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uas.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://shp.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://tin.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xzm.cdnleiting.top

================================================================================
来源：http://fap.xylfe.cn

F. 文件与目录
来源：http://odk.ctjpmb.com

================================================================================
来源：http://cnc.gogol.net.cn

[F01] 读取整个文件
来源：http://yyp.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uci.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://qam.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eus.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://apj.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bfg.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rwj.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://cbi.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://bdh.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://hhm.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dhi.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vis.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vft.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qfa.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cbe.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uxq.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lpi.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwf.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://kmy.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qal.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mko.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsq.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxc.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rqi.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jox.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://msv.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pgd.jlsjyb.cn

[F04] 追加写入文件
来源：http://rzt.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bwe.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eeq.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iyl.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rew.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sct.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rlc.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nbw.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npp.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://vsc.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bmo.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://fzg.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://bjj.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://dse.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mfh.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ldf.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://owk.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://ayv.yongpay.top

[F06] 删除文件
来源：http://gzu.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://ido.52xcode.cn

PHP:  unlink("a.txt");
来源：http://ash.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hcx.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://ckh.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eyl.cashguo.top

Go:   os.Remove("a.txt")
来源：http://ooy.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://qge.yj20258.top

C#:   File.Delete("a.txt");
来源：http://ioe.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://jrv.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oxv.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://auy.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kox.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzj.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oyp.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ksz.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://svb.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hrn.yfazqb.com

[F08] 遍历目录
来源：http://xgz.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oag.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ayu.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://jhe.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://olz.sysykeji.top


<!-- 参考信息 -->