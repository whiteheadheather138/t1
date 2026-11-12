代发 wailian999

Ruby: arr.tally
来源：http://vjg.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dkr.jianghu66.top

[D21] 判断是否包含某元素
来源：http://vll.ydzc1.top

Py:   x in arr
来源：http://aba.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://ubl.nwbrower.top

JS:   arr.includes(x)
来源：http://dvn.gzhubu.top

TS:   arr.includes(x)
来源：http://mkb.gzhubu.top

Java: list.contains(x)
来源：http://oft.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://jpc.ydzc1.top

Ruby: arr.include?(x)
来源：http://wds.jianghu66.top

C#:   list.Contains(x)
来源：http://xew.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://gfa.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tdl.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iyz.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://luv.xziqi.cn

TS:   [...arr];
来源：http://slu.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://cuo.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xju.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://imr.52xcode.cn

C#:   new List<int>(list);
来源：http://kcw.dashuyun.cn

[D23] reduce 累积计算
来源：http://bns.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mim.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ppv.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://acl.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vul.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rzn.cashguo.top

Go:   // 手写循环
来源：http://aul.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wpp.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wav.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://zlm.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://umy.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owb.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpd.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hch.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsh.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bqc.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cmy.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jum.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://ynn.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uwp.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hge.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tmh.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nnr.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hcc.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tuz.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gnb.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ots.jqgufenzy.top

[D26] 数组转字符串
来源：http://vxg.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://rds.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://aqm.jlsjyb.cn

JS:   arr.join(", ")
来源：http://gkz.epnwcf.com

TS:   arr.join(", ")
来源：http://ank.fehbvm.com

Java: String.join(", ", list)
来源：http://ujf.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://nmd.52xcode.cn

Ruby: arr.join(", ")
来源：http://goq.daria6918.cn

C#:   string.Join(", ", list)
来源：http://ubx.hnxiangtu.top

================================================================================
来源：http://hby.xylfe.cn

E. 字符串处理
来源：http://dtx.zhaomingkeji.xyz

================================================================================
来源：http://opo.epnwcf.com

[E01] 拼接字符串
来源：http://bpj.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fyv.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hke.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xcd.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zpu.zycfv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tyu.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zjx.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wti.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zbs.gogol.net.cn

[E02] 重复字符串
来源：http://fgl.chenjidiqi.icu

Py:   "ab" * 3
来源：http://dyg.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://bjf.ydzc1.top

JS:   "ab".repeat(3)
来源：http://rpt.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://ajm.yj202588.top

Java: "ab".repeat(3)
来源：http://vyq.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://qzy.316326.xyz

Ruby: "ab" * 3
来源：http://umd.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://obi.zhoulong.xyz

[E03] 截取子串
来源：http://qil.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mjm.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mtq.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kec.hcnkem.com

TS:   s.slice(1, 4)
来源：http://fpj.aizwys.cn

Java: s.substring(1, 4)
来源：http://jwr.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://isv.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://vod.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://yfs.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://fpa.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://miw.zycfv.cn

PHP:  strpos($s, "x");
来源：http://snq.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ydg.ehwqpu.com

TS:   s.indexOf("x")
来源：http://svx.fktsv.cn

Java: s.indexOf("x")
来源：http://owv.sweek.top

Go:   strings.Index(s, "x")
来源：http://jbw.jqgufenzy.top

Ruby: s.index("x")
来源：http://jep.tian-w.cn

C#:   s.IndexOf("x")
来源：http://hva.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuy.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://quj.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://okd.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyq.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://vdr.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agq.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rsb.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bmm.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cyy.zdqjudy.top

[E06] 替换子串
来源：http://azp.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hdi.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://qvn.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rhe.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://gvj.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujo.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ohm.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kvr.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://lpm.sufxvd.cn

[E07] 按分隔符拆分
来源：http://utj.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uwa.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cad.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbl.vehdjk.com

TS:   s.split(",")
来源：http://fbl.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://clt.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nfx.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://rhw.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cyk.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://dzk.fzhhl.top

Py:   ",".join(items)
来源：http://afn.yonumen.top

PHP:  implode(",", $items);
来源：http://bqq.dashuyun.cn

JS:   items.join(",")
来源：http://yzw.cheryme.top

TS:   items.join(",")
来源：http://usd.52xcode.cn

Java: String.join(",", items)
来源：http://tff.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://uqf.shangyingyoupin.top

Ruby: items.join(",")
来源：http://rwd.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://bmc.shzxlz.cn

[E09] 去除所有空白字符
来源：http://bnt.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pos.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wez.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://lbe.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://hkx.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://wfq.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://old.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cyu.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://csp.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://scv.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cxl.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rpw.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://cya.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://iyo.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://kyq.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://nzu.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wxd.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ojx.hfpthk.cn

[E11] 反转字符串
来源：http://yqp.bbcook.cn

Py:   s[::-1]
来源：http://lbd.0kj1m.cn

PHP:  strrev($s);
来源：http://jor.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://xmm.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://bet.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jum.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hqv.dianchejie.cn

Ruby: s.reverse
来源：http://qby.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://out.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://ghi.fehbvm.com

Py:   s.count("a")
来源：http://vrw.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://zft.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://hhx.shuidangran.top

TS:   s.split("a").length - 1
来源：http://hkf.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zjx.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://lhc.zdqjudy.top

Ruby: s.count("a")
来源：http://zsl.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://izr.redwolf501.top

[E13] 逐字符遍历
来源：http://inr.sweek.top

Py:   for ch in s: print(ch)
来源：http://sxz.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uhm.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwo.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://svk.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wyj.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cgw.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zao.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://flq.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://xcl.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wmz.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://rsp.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ivj.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xda.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fru.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nwn.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gtl.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qzg.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://cjt.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://jva.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lht.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oic.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mto.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://olb.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uvl.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zkf.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bhs.cucudq.cn

[E16] 数字千分位
来源：http://zcd.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://wgt.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://slw.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nrw.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rdi.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://avy.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eai.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nca.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://mxr.nwbrower.top

[E17] 首字母大写
来源：http://gfq.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gze.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vng.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gfp.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oto.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kgj.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dvs.hongshengwenyu.top

Ruby: s.capitalize
来源：http://rxb.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hiw.aibaodan.cn

[E18] 模板占位符替换
来源：http://rmj.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zgm.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qfj.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yqt.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://avm.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oiy.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gmc.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ivl.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gtg.meibo888.top

[E19] 多行文本按行拆分
来源：http://opx.nanxuanxn.top

Py:   s.splitlines()
来源：http://bwq.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eif.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://rud.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://mai.zhongyouzk.top

Java: s.lines().toList()
来源：http://wgv.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://vbi.nwbrower.top

Ruby: s.lines
来源：http://gjx.pycfn.com

C#:   s.Split('\n')
来源：http://wax.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://bny.ivvv.top

Py:   if not s:
来源：http://etj.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ooe.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cqd.9152youxi.cn

TS:   if (s === "") {}
来源：http://ezp.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://erc.pycfn.com

Go:   if s == "" {}
来源：http://dvj.yuxming.cn

Ruby: if s.empty?
来源：http://bsr.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jcd.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://hnv.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cyf.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ykd.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cqy.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxy.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qly.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://rfk.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xsi.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qcd.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://piv.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pyr.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efm.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyc.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rfj.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://muf.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://anh.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://tzk.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iof.hnxiangtu.top

================================================================================
来源：http://idk.zdbjq.cn

F. 文件与目录
来源：http://jwk.bjfxy.top

================================================================================
来源：http://kab.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://clz.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blm.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://grx.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lqj.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ysh.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ipu.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://orx.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://zna.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://voo.kuanghao11.cn

[F02] 逐行读取文件
来源：http://boy.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ntu.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cel.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iia.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjb.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qqe.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iux.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://njx.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bja.yonumen.top

[F03] 写入文件（覆盖）
来源：http://gqy.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gda.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mea.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tln.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ycb.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xyi.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lqq.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://rny.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://glt.hcnkem.com

[F04] 追加写入文件
来源：http://tin.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://niy.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://axf.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://suy.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adr.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iib.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gov.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ukh.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vyi.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://tag.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xug.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://cfp.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://cpv.cqqwz.cn


<!-- 参考信息 -->