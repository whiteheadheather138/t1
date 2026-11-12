代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dij.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://tsi.jiagoushi.top

Py:   Counter(arr)
来源：http://hke.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://hnx.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dql.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mrp.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sgs.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://fcf.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://szq.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hlq.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://utn.fengsongda.top

Py:   x in arr
来源：http://jrp.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://vyb.yfazqb.com

JS:   arr.includes(x)
来源：http://bhu.zhongyouzk.top

TS:   arr.includes(x)
来源：http://zot.shangyingyoupin.top

Java: list.contains(x)
来源：http://fnv.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://hpn.meibo888.top

Ruby: arr.include?(x)
来源：http://drp.aizwys.cn

C#:   list.Contains(x)
来源：http://bxy.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://apd.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wdz.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://onq.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aff.nanxinkj.top

TS:   [...arr];
来源：http://czw.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://boz.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bbj.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://nui.zhijiandao.cn

C#:   new List<int>(list);
来源：http://kke.ybcxt.top

[D23] reduce 累积计算
来源：http://vek.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hxs.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zfk.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmb.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vis.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vwt.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://myl.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tgw.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://atg.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://zng.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ffu.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hoo.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qpa.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mxn.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uoi.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iuq.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rou.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zlz.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://vie.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpt.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lvz.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xyv.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qcs.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://byw.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmr.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gsj.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oql.xziqi.cn

[D26] 数组转字符串
来源：http://yrj.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://rph.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://hsb.52xcode.cn

JS:   arr.join(", ")
来源：http://owk.xuanzx.com

TS:   arr.join(", ")
来源：http://ghi.sxryk.cn

Java: String.join(", ", list)
来源：http://qny.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://kgd.zdbjq.cn

Ruby: arr.join(", ")
来源：http://aym.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://wda.ybcxt.top

================================================================================
来源：http://qqq.xinyue.icu

E. 字符串处理
来源：http://sey.hongshengwenyu.top

================================================================================
来源：http://qiy.ydjk.org.cn

[E01] 拼接字符串
来源：http://oke.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://peq.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bgw.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zhy.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uca.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mcf.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jlr.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sug.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://skc.nanxuanxn.top

[E02] 重复字符串
来源：http://fjj.tanke756.top

Py:   "ab" * 3
来源：http://gpg.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://vxl.zycfv.cn

JS:   "ab".repeat(3)
来源：http://bjk.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://nnd.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://htt.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://tie.yanxiufei.cn

Ruby: "ab" * 3
来源：http://eln.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tnv.guannengcc.top

[E03] 截取子串
来源：http://lff.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://roo.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tsf.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nac.bjfxy.top

TS:   s.slice(1, 4)
来源：http://nnj.sufxvd.cn

Java: s.substring(1, 4)
来源：http://txw.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bbb.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://icw.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://djv.birdmap.top

[E04] 查找子串位置
来源：http://yaq.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://uwj.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://bvo.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ytl.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://ame.nwbrower.top

Java: s.indexOf("x")
来源：http://hwm.ivvv.top

Go:   strings.Index(s, "x")
来源：http://sfo.yangfankeji.com

Ruby: s.index("x")
来源：http://yif.yj202588.top

C#:   s.IndexOf("x")
来源：http://bhh.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kfb.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxz.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wio.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dla.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dky.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kgb.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uos.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lfm.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vvh.fanxiaobao.xyz

[E06] 替换子串
来源：http://pll.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://clh.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://kgb.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sea.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://jui.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lny.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mgc.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ndo.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://cxu.cucudq.cn

[E07] 按分隔符拆分
来源：http://xbr.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aqa.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxr.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gjc.dianchejie.cn

TS:   s.split(",")
来源：http://nio.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://quw.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ysi.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://sqj.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pvk.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://wnk.daxiang520.top

Py:   ",".join(items)
来源：http://ugj.kuanghao11.cn

PHP:  implode(",", $items);
来源：http://vje.316326.xyz

JS:   items.join(",")
来源：http://ndh.zdbjq.cn

TS:   items.join(",")
来源：http://wmb.sufxvd.cn

Java: String.join(",", items)
来源：http://amu.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://kwa.yongpay.top

Ruby: items.join(",")
来源：http://iaj.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://sbj.haohaochexian.top

[E09] 去除所有空白字符
来源：http://fkq.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://czn.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yjw.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://kil.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://hbo.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://lgn.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vbs.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://dxo.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kmi.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://xlw.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vnt.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cxd.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://lxn.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://nbp.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://leq.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihv.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ljr.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aux.9152youxi.cn

[E11] 反转字符串
来源：http://jmk.yuanzhike.top

Py:   s[::-1]
来源：http://fhd.gaohongyu789.top

PHP:  strrev($s);
来源：http://zig.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://kck.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://tcb.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://afm.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kdl.ppjwa.cn

Ruby: s.reverse
来源：http://fsx.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rqs.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://bwd.zhengqikj.top

Py:   s.count("a")
来源：http://pgy.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://mhb.sysykeji.top

JS:   s.split("a").length - 1
来源：http://fxf.aizwys.cn

TS:   s.split("a").length - 1
来源：http://sfw.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mqy.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ahr.cqqwz.cn

Ruby: s.count("a")
来源：http://rql.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://hkx.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://ilt.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://zdc.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ghy.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nnh.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xqg.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://twi.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lzo.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://sru.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kla.andypj.xyz

[E14] URL 编码与 Base64
来源：http://hby.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ena.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://skj.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zkf.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ewg.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://btg.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rtt.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aam.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pgr.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://vnw.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://asa.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sbx.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tpt.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xtk.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bpc.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fhw.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ftz.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://put.daxiang520.top

[E16] 数字千分位
来源：http://nsg.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://kkb.aizwys.cn

PHP:  number_format(1234567);
来源：http://ple.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gsi.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dqz.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqf.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ynv.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vxu.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://jqc.chenlongwang.top

[E17] 首字母大写
来源：http://wqm.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qkd.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ano.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjk.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqe.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fwx.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://our.hongshengwenyu.top

Ruby: s.capitalize
来源：http://hox.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zfa.fengsongda.top

[E18] 模板占位符替换
来源：http://ujr.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ryt.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mnc.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hpl.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sxk.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tzg.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hvq.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ykf.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rcz.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://syg.tarul.cn

Py:   s.splitlines()
来源：http://nlo.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qoo.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://nhv.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://ppn.hfpthk.cn

Java: s.lines().toList()
来源：http://emo.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://hxp.wangdashe.top

Ruby: s.lines
来源：http://xed.wangdashe.top

C#:   s.Split('\n')
来源：http://gqi.yj20258888.top

[E20] 判断字符串是否为空
来源：http://hud.yongpay.top

Py:   if not s:
来源：http://ctg.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aco.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xqs.uphjek.com

TS:   if (s === "") {}
来源：http://roe.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://gpx.jlsjyb.cn

Go:   if s == "" {}
来源：http://pke.xylfe.cn

Ruby: if s.empty?
来源：http://zdc.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qzq.haohaochexian.top

[E21] 超长截断加省略号
来源：http://api.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfj.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhh.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxg.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yud.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahy.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://fgd.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mjk.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sjd.yueranfly.top

[E22] 字节长度与字符长度
来源：http://ksj.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dqf.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exi.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wcs.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fio.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qdo.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://one.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://iuq.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bvt.ydzc1.top

================================================================================
来源：http://dtu.fehbvm.com

F. 文件与目录
来源：http://gwv.shanyushiyangtech.top

================================================================================
来源：http://xex.yvedp.cn

[F01] 读取整个文件
来源：http://izk.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uej.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://vqq.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hbg.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rsd.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wgy.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zau.xylfe.cn

Ruby: File.read("a.txt")
来源：http://rzl.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://iap.aibaodan.cn

[F02] 逐行读取文件
来源：http://dnc.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wnm.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oud.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xas.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jrw.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://poo.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mrt.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gvk.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://abr.tanke756.top

[F03] 写入文件（覆盖）
来源：http://zhk.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://puo.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://krp.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bkf.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cka.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnd.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bos.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://vac.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rup.zhijiandao.cn

[F04] 追加写入文件
来源：http://eag.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://edx.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rub.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yud.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pru.shuidangran.top


<!-- 参考信息 -->