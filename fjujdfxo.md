代发 wailian999

C#:   list.Distinct().ToList()
来源：http://xrm.yueranfly.top

[D16] 求和与平均值
来源：http://wam.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xrx.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmf.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vkl.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsm.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://opq.tian-w.cn

Go:   // 手写循环累加
来源：http://fik.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ifh.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://bea.ydjk.org.cn

[D17] 最大值与最小值
来源：http://ohm.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://zom.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://sqf.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nys.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://cnv.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://veh.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hdp.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://ppn.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://usw.birdmap.top

[D18] 扁平化嵌套数组
来源：http://lbv.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://poe.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://oay.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lqz.zdbjq.cn

TS:   nested.flat();
来源：http://yha.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pgq.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://mjl.hongshengwenyu.top

Ruby: nested.flatten
来源：http://ocg.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kpu.bjfxy.top

[D19] 按字段分组
来源：http://skw.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jdo.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ydr.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eqx.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zap.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mvu.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://spm.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://bse.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ddl.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://osj.hfpthk.cn

Py:   Counter(arr)
来源：http://lce.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://wpf.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxj.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://piv.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cwj.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://meu.xuanzx.com

Ruby: arr.tally
来源：http://zbz.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bkp.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://seq.hnxiangtu.top

Py:   x in arr
来源：http://vmg.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://bml.jiagoushi.top

JS:   arr.includes(x)
来源：http://tkd.cqqwz.cn

TS:   arr.includes(x)
来源：http://dky.daxiang520.top

Java: list.contains(x)
来源：http://cbg.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://nis.gzhubu.top

Ruby: arr.include?(x)
来源：http://sds.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://olj.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://loh.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ckp.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rew.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qjd.vqdsnc.cn

TS:   [...arr];
来源：http://mla.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://sce.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://sax.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://ehj.tianlin.xyz

C#:   new List<int>(list);
来源：http://rko.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://zno.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rae.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://edn.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qpx.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dmk.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://euu.mhx1999.top

Go:   // 手写循环
来源：http://mvy.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nbv.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pte.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://byr.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jfw.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oub.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kji.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iwx.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bjk.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mwz.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bhn.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://scu.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://gnr.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rpk.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aie.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lsz.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oje.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://opn.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://adu.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://alc.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bhc.guowangkeji.top

[D26] 数组转字符串
来源：http://mjp.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://csw.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://xkb.quarkkingdee.top

JS:   arr.join(", ")
来源：http://tjl.fktsv.cn

TS:   arr.join(", ")
来源：http://lvt.yuanzhike.top

Java: String.join(", ", list)
来源：http://xjk.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://jud.hcnkem.com

Ruby: arr.join(", ")
来源：http://zjx.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://twp.yuxming.cn

================================================================================
来源：http://coh.vqdsnc.cn

E. 字符串处理
来源：http://nri.zhijiandao.cn

================================================================================
来源：http://tet.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://npd.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nfo.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ixr.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://anw.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fip.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ctm.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://slh.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gth.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vpm.jqgfzy.top

[E02] 重复字符串
来源：http://zgu.tianlin.xyz

Py:   "ab" * 3
来源：http://miv.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://wkt.birdmap.top

JS:   "ab".repeat(3)
来源：http://axu.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://gam.shzxlz.cn

Java: "ab".repeat(3)
来源：http://ctf.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://ioh.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://xpq.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tpv.aizwys.cn

[E03] 截取子串
来源：http://ral.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tqs.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vnw.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tmo.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://pfl.gogol.net.cn

Java: s.substring(1, 4)
来源：http://hjf.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://chg.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://iaz.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://zmh.zhiwuduotai.top

[E04] 查找子串位置
来源：http://zol.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://hte.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://dag.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://div.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://ljf.gaohongyu789.top

Java: s.indexOf("x")
来源：http://rzx.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://mwo.zdqjudy.top

Ruby: s.index("x")
来源：http://slb.mhx1999.top

C#:   s.IndexOf("x")
来源：http://gfq.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pnd.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uwt.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esl.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybz.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kkl.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvl.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eil.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kra.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjw.52xcode.cn

[E06] 替换子串
来源：http://mon.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tfu.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://tel.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fns.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://zqx.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ese.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://exn.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lyy.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://viy.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://ign.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lgx.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://axm.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rpl.nwbrower.top

TS:   s.split(",")
来源：http://vud.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://wvh.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fpp.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://red.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wxb.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://izz.feifeiyinyue.top

Py:   ",".join(items)
来源：http://pun.xinyue.icu

PHP:  implode(",", $items);
来源：http://vly.cdnleiting.top

JS:   items.join(",")
来源：http://dkb.zdqjudy.top

TS:   items.join(",")
来源：http://yff.fktsv.cn

Java: String.join(",", items)
来源：http://opp.yj202588.top

Go:   strings.Join(items, ",")
来源：http://pan.chenjidiqi.icu

Ruby: items.join(",")
来源：http://gzp.yangfankeji.com

C#:   string.Join(",", items)
来源：http://sgv.jiagoushi.top

[E09] 去除所有空白字符
来源：http://wwa.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ljc.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vjt.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://dql.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://adr.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://wut.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rto.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ayo.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oui.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://czm.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://brz.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sji.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://eqz.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://ubz.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://psq.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eyz.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fnj.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ccq.sufxvd.cn

[E11] 反转字符串
来源：http://mfg.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://odd.zdqjudy.top

PHP:  strrev($s);
来源：http://khp.316326.xyz

JS:   [...s].reverse().join("")
来源：http://frg.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://qep.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tqs.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dfw.ydzc1.top

Ruby: s.reverse
来源：http://ulb.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://amq.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://wjt.jianghu66.top

Py:   s.count("a")
来源：http://fxk.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://kpg.hnqzz.top

JS:   s.split("a").length - 1
来源：http://ujj.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://dbz.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uhu.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://deq.yj202588.top

Ruby: s.count("a")
来源：http://xnk.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://rnn.yongpay.top

[E13] 逐字符遍历
来源：http://etz.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://qtd.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://shs.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zrg.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wnf.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jtn.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oem.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tko.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kez.yfazqb.com

[E14] URL 编码与 Base64
来源：http://yfk.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yyd.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kov.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qid.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zhw.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lbl.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tso.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ycr.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cdw.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://gts.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iyl.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xgn.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yag.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sps.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cpi.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wsc.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://boi.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fud.guannengcc.top

[E16] 数字千分位
来源：http://zaw.uphjek.com

Py:   f"{1234567:,}"
来源：http://uec.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://req.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cgz.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kga.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://leu.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://voh.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gnt.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://sic.gaohongyu789.top

[E17] 首字母大写
来源：http://foh.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ssr.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cqg.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbf.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ulz.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baq.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://myd.shangyingyoupin.top

Ruby: s.capitalize
来源：http://qfr.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rkm.c1oappe.top

[E18] 模板占位符替换
来源：http://wxi.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kdh.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tdd.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ime.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zrz.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijr.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nlc.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xfr.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aka.hnqzz.top

[E19] 多行文本按行拆分
来源：http://rdc.yj20258.top

Py:   s.splitlines()
来源：http://bnd.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ghb.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://lqf.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://wwe.yanxiufei.cn

Java: s.lines().toList()
来源：http://bmo.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://wiz.jiagoushi.top

Ruby: s.lines
来源：http://qyl.bjfxy.top

C#:   s.Split('\n')
来源：http://fpt.birdmap.top

[E20] 判断字符串是否为空
来源：http://lii.ybcxt.top

Py:   if not s:
来源：http://eun.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eqq.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pii.epnwcf.com

TS:   if (s === "") {}
来源：http://pvl.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://tqy.yanxiufei.cn

Go:   if s == "" {}
来源：http://swg.haohaochexian.top

Ruby: if s.empty?
来源：http://rqb.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qfd.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://cef.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oju.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://efa.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogx.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pes.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://myo.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://sez.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nry.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ogu.epnwcf.com

[E22] 字节长度与字符长度
来源：http://psr.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nyb.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://prd.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvh.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sxt.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pco.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wtf.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://uke.52xcode.cn


<!-- 参考信息 -->