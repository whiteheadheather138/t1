代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://plh.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://wxv.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ifp.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qzx.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpz.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://esj.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qjt.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kzn.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nyl.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gvq.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://vxw.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wlz.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kdw.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jke.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qsk.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jqy.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nhg.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zty.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ahj.sxryk.cn

[D26] 数组转字符串
来源：http://zml.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://kbx.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://fhc.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://avi.tianlin.xyz

TS:   arr.join(", ")
来源：http://pym.wangdashe.top

Java: String.join(", ", list)
来源：http://xdb.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://fvn.ctjpmb.com

Ruby: arr.join(", ")
来源：http://anc.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://blw.nanxuanxn.top

================================================================================
来源：http://tcr.quarkkingdee.top

E. 字符串处理
来源：http://fig.yonumen.top

================================================================================
来源：http://atl.jinqigfzy.top

[E01] 拼接字符串
来源：http://tgc.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rkg.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sta.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojm.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dtf.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hbh.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://soq.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://irv.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aly.feifeiyinyue.top

[E02] 重复字符串
来源：http://lul.yuxming.cn

Py:   "ab" * 3
来源：http://bsn.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://hux.redwolf501.top

JS:   "ab".repeat(3)
来源：http://cfz.gzhubu.top

TS:   "ab".repeat(3)
来源：http://sxt.yuxming.cn

Java: "ab".repeat(3)
来源：http://phj.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ftl.zhengqikj.top

Ruby: "ab" * 3
来源：http://nzx.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ouf.52xcode.cn

[E03] 截取子串
来源：http://xcf.smart0.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hqv.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yxc.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fto.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://uic.fzhhl.top

Java: s.substring(1, 4)
来源：http://fvy.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xzr.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://skr.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://odi.hysaishi.cn

[E04] 查找子串位置
来源：http://mwf.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://rty.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://wfp.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pmb.daria6918.cn

TS:   s.indexOf("x")
来源：http://ztz.cheryme.top

Java: s.indexOf("x")
来源：http://twv.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://bre.aizwys.cn

Ruby: s.index("x")
来源：http://mpn.mhx1999.top

C#:   s.IndexOf("x")
来源：http://gkh.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jdy.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ndl.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://huz.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yrb.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pbr.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqf.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pvk.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ykc.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://twc.ivvv.top

[E06] 替换子串
来源：http://hbp.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rox.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://gjs.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pmz.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://yai.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvk.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ifk.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bcv.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://bpe.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://nky.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uyd.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mly.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tjr.ydjk.org.cn

TS:   s.split(",")
来源：http://guu.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wxw.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mgt.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://gbh.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ldt.bbcook.cn

[E08] 数组按分隔符合并
来源：http://kqg.vqdsnc.cn

Py:   ",".join(items)
来源：http://cvg.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://ywf.pengpengdd.cyou

JS:   items.join(",")
来源：http://hwn.bjfxy.top

TS:   items.join(",")
来源：http://fmi.havefunace.top

Java: String.join(",", items)
来源：http://xjf.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://vbg.gogol.net.cn

Ruby: items.join(",")
来源：http://okc.ybcxt.top

C#:   string.Join(",", items)
来源：http://uya.aizwys.cn

[E09] 去除所有空白字符
来源：http://fzm.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dii.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eww.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://dha.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://kov.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://knt.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://blx.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://kab.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kuh.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://kzt.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bdb.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vvw.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://yua.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://kwa.sweek.top

Java: String.format("%03d", 7)
来源：http://iww.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vnc.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vqp.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hjy.kuanghao11.cn

[E11] 反转字符串
来源：http://hjr.gotoacloud.top

Py:   s[::-1]
来源：http://oac.hywenlv.cn

PHP:  strrev($s);
来源：http://ppu.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://xgi.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://ojf.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qad.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jye.ivvv.top

Ruby: s.reverse
来源：http://efw.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://wnl.fengsongda.top

[E12] 统计某字符出现次数
来源：http://zab.0kj1m.cn

Py:   s.count("a")
来源：http://ish.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://uep.52xcode.cn

JS:   s.split("a").length - 1
来源：http://fbf.cucudq.cn

TS:   s.split("a").length - 1
来源：http://lcf.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://icb.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://phq.quarkkingdee.top

Ruby: s.count("a")
来源：http://mxe.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://vxx.jinqigfzy.top

[E13] 逐字符遍历
来源：http://lof.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://lki.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gbf.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oth.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nza.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://upk.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dxv.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dky.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rdc.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://yma.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pls.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qyf.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yaf.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xdk.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eip.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tjx.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iee.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sph.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://ggz.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uav.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fcp.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uwp.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ors.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ehq.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sjj.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmh.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgq.tarul.cn

[E16] 数字千分位
来源：http://njd.fzhhl.top

Py:   f"{1234567:,}"
来源：http://tvl.daria6918.cn

PHP:  number_format(1234567);
来源：http://upz.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gwj.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tvi.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://afq.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qwa.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://waz.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://pbd.sweek.top

[E17] 首字母大写
来源：http://ozw.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ncn.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://crm.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukz.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjy.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kef.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zbf.hammf.cn

Ruby: s.capitalize
来源：http://mlt.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ntg.iojbl.cn

[E18] 模板占位符替换
来源：http://kto.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nwr.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nny.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hsa.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tfv.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://glb.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://smw.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bsc.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nav.52xcode.cn

[E19] 多行文本按行拆分
来源：http://zfq.xziqi.cn

Py:   s.splitlines()
来源：http://sga.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hee.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://swl.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://fgs.ctjpmb.com

Java: s.lines().toList()
来源：http://nuu.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://csg.gzhubu.top

Ruby: s.lines
来源：http://qgz.ctjpmb.com

C#:   s.Split('\n')
来源：http://dpi.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://wvo.tian-w.cn

Py:   if not s:
来源：http://lku.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yvc.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jws.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://qxk.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://ewo.ctjpmb.com

Go:   if s == "" {}
来源：http://byz.andypj.xyz

Ruby: if s.empty?
来源：http://ugu.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://txf.haohaochexian.top

[E21] 超长截断加省略号
来源：http://cha.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ijx.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jsn.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxt.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kir.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qtp.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ckx.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xxw.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hhz.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://ysh.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qdu.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhh.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpz.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rna.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xju.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zxb.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://psr.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xes.sweek.top

================================================================================
来源：http://usj.xziqi.cn

F. 文件与目录
来源：http://nsw.yangfankeji.com

================================================================================
来源：http://his.chenlongwang.top

[F01] 读取整个文件
来源：http://rgh.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mnb.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://ktu.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tfz.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jpf.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ycp.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fju.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://vry.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://ywx.cucudq.cn

[F02] 逐行读取文件
来源：http://qdf.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hcf.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qef.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mag.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sjb.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://twq.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cdn.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ofn.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wao.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://hzr.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tge.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://kvv.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xlk.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gen.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dgz.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oym.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://kfv.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://saj.sufxvd.cn

[F04] 追加写入文件
来源：http://jze.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rir.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gnr.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfo.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pul.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ayl.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfv.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://icl.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://olm.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://yvs.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sbo.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://axo.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://bvz.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://tlm.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jjf.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idj.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://jzf.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://uum.ybcxt.top

[F06] 删除文件
来源：http://qgy.fzhhl.top

Py:   os.remove("a.txt")
来源：http://rlk.ybcxt.top

PHP:  unlink("a.txt");
来源：http://ysi.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://gvv.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://mya.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bww.pycfn.com

Go:   os.Remove("a.txt")
来源：http://kro.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://luo.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://zfo.nwbrower.top

[F07] 创建目录（含多级）
来源：http://kiu.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://szu.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jsa.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zyo.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivi.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qej.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyj.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kyg.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wsv.hnqzz.top

[F08] 遍历目录
来源：http://ikf.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://mwq.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vml.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://gal.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://gdf.havefunace.top


<!-- 参考信息 -->