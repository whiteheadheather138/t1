代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ros.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihk.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://evf.9152youxi.cn

Go:   // 手写循环累加
来源：http://agn.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bbw.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://gkm.kuanghao11.cn

[D17] 最大值与最小值
来源：http://lfs.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://rnj.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://vqw.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hvv.havefunace.top

TS:   Math.max(...arr);
来源：http://uax.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lfa.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ccg.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://ejq.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://dcs.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://zcp.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fld.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://lju.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mqy.birdmap.top

TS:   nested.flat();
来源：http://bye.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lno.yfazqb.com

Go:   // 手写双层循环
来源：http://plo.hongshengwenyu.top

Ruby: nested.flatten
来源：http://vhl.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://yve.birdmap.top

[D19] 按字段分组
来源：http://kmt.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://esc.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://msu.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mdf.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qhm.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://doe.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://lwe.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kud.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mmc.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://lwd.chenjidiqi.icu

Py:   Counter(arr)
来源：http://wnf.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://aem.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tfm.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdh.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kcc.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://nzp.gotoacloud.top

Ruby: arr.tally
来源：http://rrt.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gel.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://hpk.hnxiangtu.top

Py:   x in arr
来源：http://wnv.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://ulj.tarul.cn

JS:   arr.includes(x)
来源：http://pyp.sweek.top

TS:   arr.includes(x)
来源：http://uno.hfpthk.cn

Java: list.contains(x)
来源：http://ucf.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://zha.aizwys.cn

Ruby: arr.include?(x)
来源：http://ohj.xziqi.cn

C#:   list.Contains(x)
来源：http://sos.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://nej.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pqj.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zxi.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jny.yj20258888.top

TS:   [...arr];
来源：http://ohg.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://imv.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://qqa.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://yca.yj202588.top

C#:   new List<int>(list);
来源：http://fcm.nanxuanxn.top

[D23] reduce 累积计算
来源：http://rco.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://krn.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ise.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://etr.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hjh.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://xcb.birdmap.top

Go:   // 手写循环
来源：http://bjh.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://btt.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zxp.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://qon.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hop.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wqf.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mvt.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yht.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wcl.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kjg.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cnv.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fei.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://lhr.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hgr.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lna.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rwv.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mua.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hxk.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zzw.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dwl.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bza.dashuyun.cn

[D26] 数组转字符串
来源：http://flw.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://mxc.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://tob.jyoumei.cn

JS:   arr.join(", ")
来源：http://odz.xylfe.cn

TS:   arr.join(", ")
来源：http://mie.fzhhl.top

Java: String.join(", ", list)
来源：http://fuo.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://asw.ctjpmb.com

Ruby: arr.join(", ")
来源：http://isk.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://kqb.zhaomingkeji.xyz

================================================================================
来源：http://vgi.gogol.net.cn

E. 字符串处理
来源：http://fqa.vehdjk.com

================================================================================
来源：http://uwx.wangdashe.top

[E01] 拼接字符串
来源：http://dgz.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://glg.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jta.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jci.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gui.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ckl.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://efu.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wth.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://msn.fengsongda.top

[E02] 重复字符串
来源：http://ehc.aizwys.cn

Py:   "ab" * 3
来源：http://brf.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://xkb.hnqzz.top

JS:   "ab".repeat(3)
来源：http://gmg.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://rsa.xylfe.cn

Java: "ab".repeat(3)
来源：http://chw.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://nbz.cucudq.cn

Ruby: "ab" * 3
来源：http://xed.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cru.daxiang520.top

[E03] 截取子串
来源：http://iiu.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yke.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zid.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dmp.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://lgy.zhixingplan.top

Java: s.substring(1, 4)
来源：http://cpp.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pgn.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://umd.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://crk.tanke756.top

[E04] 查找子串位置
来源：http://pyt.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://wni.ydzc1.top

PHP:  strpos($s, "x");
来源：http://bfo.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xjx.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://chj.jqgufenzy.top

Java: s.indexOf("x")
来源：http://svr.yongpay.top

Go:   strings.Index(s, "x")
来源：http://gjl.svipenyu.cn

Ruby: s.index("x")
来源：http://prn.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://rxg.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://omh.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://exp.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ncc.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmx.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://sna.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prq.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvo.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wqb.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xkk.yangfankeji.com

[E06] 替换子串
来源：http://xyj.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tgc.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://lgm.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nub.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://zsw.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eun.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jsk.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qsu.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://iqz.xylfe.cn

[E07] 按分隔符拆分
来源：http://nsl.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vcy.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fbb.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://jbi.zhiwuduotai.top

TS:   s.split(",")
来源：http://izo.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://djy.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vsv.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://mpd.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pse.daxiang520.top

[E08] 数组按分隔符合并
来源：http://fxt.shangyingyoupin.top

Py:   ",".join(items)
来源：http://wea.zhengqikj.top

PHP:  implode(",", $items);
来源：http://ooq.hfpthk.cn

JS:   items.join(",")
来源：http://jxl.sufxvd.cn

TS:   items.join(",")
来源：http://hmm.daria6918.cn

Java: String.join(",", items)
来源：http://vqb.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://eex.hammf.cn

Ruby: items.join(",")
来源：http://nxp.hammf.cn

C#:   string.Join(",", items)
来源：http://zdq.gzhubu.top

[E09] 去除所有空白字符
来源：http://yzu.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://amk.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lwc.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://lgi.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://zxv.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://cre.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hbm.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kso.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qxo.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://ble.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ztw.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lra.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://nrt.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://pld.nwbrower.top

Java: String.format("%03d", 7)
来源：http://znt.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ckd.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bcu.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lnf.hysaishi.cn

[E11] 反转字符串
来源：http://czr.svipenyu.cn

Py:   s[::-1]
来源：http://mcj.fengsongda.top

PHP:  strrev($s);
来源：http://jhn.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://cyq.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://iaf.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://klu.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgy.cqqwz.cn

Ruby: s.reverse
来源：http://kpq.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://trg.hnqzz.top

[E12] 统计某字符出现次数
来源：http://lqb.fehbvm.com

Py:   s.count("a")
来源：http://ami.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://krb.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://onr.mhx1999.top

TS:   s.split("a").length - 1
来源：http://swb.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fzp.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://abb.ivvv.top

Ruby: s.count("a")
来源：http://txl.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://sqs.jqgfzy.top

[E13] 逐字符遍历
来源：http://pxv.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://rpb.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yxb.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://mlp.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ckb.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggq.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tud.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uht.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://slg.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://hll.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pra.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zjo.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ytr.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wns.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bbq.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kje.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ulv.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lra.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://zkz.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://puj.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xsx.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lyt.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aam.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rfe.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oab.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cbf.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yxn.cdnleiting.top

[E16] 数字千分位
来源：http://kzy.epnwcf.com

Py:   f"{1234567:,}"
来源：http://xoq.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://ltc.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rie.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kbk.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dhx.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ect.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vai.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://esp.jqgufenzy.top

[E17] 首字母大写
来源：http://fmx.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pnn.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://jtt.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iye.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnb.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://amg.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uvs.yfazqb.com

Ruby: s.capitalize
来源：http://hxv.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://act.zhengqikj.top

[E18] 模板占位符替换
来源：http://tkd.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://avt.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aww.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xug.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hvt.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mce.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bbr.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yig.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xay.cashguo.top

[E19] 多行文本按行拆分
来源：http://niv.quarkkingdee.top

Py:   s.splitlines()
来源：http://pzo.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vdt.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://ced.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://yvj.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://zzp.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://eqm.gzhubu.top

Ruby: s.lines
来源：http://pgv.nanxinkj.top

C#:   s.Split('\n')
来源：http://mai.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://snn.jqgufenzy.top

Py:   if not s:
来源：http://ldn.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gac.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rad.ybcxt.top

TS:   if (s === "") {}
来源：http://ogo.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://sia.cqqwz.cn

Go:   if s == "" {}
来源：http://cxr.tian-w.cn

Ruby: if s.empty?
来源：http://hxk.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yrk.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://dbv.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uyd.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dhr.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://otp.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qpb.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vdh.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://guf.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ghe.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mtq.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://fib.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mss.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfl.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrs.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ceu.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fls.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kfn.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://hsf.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lco.cucudq.cn

================================================================================
来源：http://pmh.haohaochexian.top

F. 文件与目录
来源：http://jbj.fengsongda.top

================================================================================
来源：http://mhf.jiagoushi.top


<!-- 参考信息 -->