代发 wailian999

[D15] 去重
来源：http://usv.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fhy.yj20258.top

PHP:  array_unique($arr);
来源：http://goy.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://lqs.xinyue.icu

TS:   [...new Set(arr)]
来源：http://ewg.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgs.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bzy.iojbl.cn

Ruby: arr.uniq
来源：http://xhb.ivvv.top

C#:   list.Distinct().ToList()
来源：http://dub.yuanzhike.top

[D16] 求和与平均值
来源：http://sxd.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zia.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jtl.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pui.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofe.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dql.chenzaomai.com

Go:   // 手写循环累加
来源：http://mgz.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tdk.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://vio.meibo888.top

[D17] 最大值与最小值
来源：http://nsr.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://npc.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://pxy.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rdn.sweek.top

TS:   Math.max(...arr);
来源：http://htm.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://wez.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yhq.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://lgh.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://tpx.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://gkn.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oln.cashguo.top

PHP:  array_merge(...$nested);
来源：http://ajb.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://odl.jyoumei.cn

TS:   nested.flat();
来源：http://mej.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ifv.vqdsnc.cn

Go:   // 手写双层循环
来源：http://vnz.sxryk.cn

Ruby: nested.flatten
来源：http://vjg.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bcm.zhiwuduotai.top

[D19] 按字段分组
来源：http://flx.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dnw.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jeu.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wyf.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cyr.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://joe.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://wcv.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qnf.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ptm.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://zmw.iojbl.cn

Py:   Counter(arr)
来源：http://eqt.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://sso.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwt.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vsp.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vnz.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://qyv.316326.xyz

Ruby: arr.tally
来源：http://lcf.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mzw.havefunace.top

[D21] 判断是否包含某元素
来源：http://gph.wangdashe.top

Py:   x in arr
来源：http://umm.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://wxv.hnqzz.top

JS:   arr.includes(x)
来源：http://mdb.nanxuanxn.top

TS:   arr.includes(x)
来源：http://hgq.jqgfzy.top

Java: list.contains(x)
来源：http://qxo.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://dqx.hywenlv.cn

Ruby: arr.include?(x)
来源：http://dzy.fehbvm.com

C#:   list.Contains(x)
来源：http://gnm.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://lzs.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://udi.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pvm.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tvu.xuetiantiany.cn

TS:   [...arr];
来源：http://fvo.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://hur.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dlv.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://elx.mhx1999.top

C#:   new List<int>(list);
来源：http://gwi.daria6918.cn

[D23] reduce 累积计算
来源：http://xwi.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tmh.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cxu.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysv.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tua.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vqx.yj202588.top

Go:   // 手写循环
来源：http://leo.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sjg.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iyv.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://hqr.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://txx.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://haa.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kux.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://saw.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://myu.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xxj.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://owo.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iwh.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://zfh.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xut.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ekm.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vch.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://odw.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qsb.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://syb.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tva.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bns.aibaodan.cn

[D26] 数组转字符串
来源：http://ret.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://koo.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://ynb.hnqzz.top

JS:   arr.join(", ")
来源：http://fbf.nanxinkj.top

TS:   arr.join(", ")
来源：http://vvd.yangfankeji.com

Java: String.join(", ", list)
来源：http://ibu.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://bqq.xuanzx.com

Ruby: arr.join(", ")
来源：http://fiu.ybcxt.top

C#:   string.Join(", ", list)
来源：http://rsn.guannengcc.top

================================================================================
来源：http://mow.mhx1999.top

E. 字符串处理
来源：http://udt.redwolf501.top

================================================================================
来源：http://jlv.chenzaomai.com

[E01] 拼接字符串
来源：http://ppr.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://est.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjk.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://etc.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fag.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iew.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://owz.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dwb.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agr.bbcook.cn

[E02] 重复字符串
来源：http://yaw.xuetiantiany.cn

Py:   "ab" * 3
来源：http://ofm.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://jvr.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://dcm.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://gnm.vehdjk.com

Java: "ab".repeat(3)
来源：http://joj.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://xya.c1oappe.top

Ruby: "ab" * 3
来源：http://hrm.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://arg.zhongyouzk.top

[E03] 截取子串
来源：http://pbx.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yew.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yix.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wem.tanke756.top

TS:   s.slice(1, 4)
来源：http://fna.ehwqpu.com

Java: s.substring(1, 4)
来源：http://jmw.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://her.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://nwa.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://pny.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://bgw.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://mxh.yongpay.top

PHP:  strpos($s, "x");
来源：http://rol.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yps.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://pwy.daxiang520.top

Java: s.indexOf("x")
来源：http://jwf.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://rpe.kuanghao11.cn

Ruby: s.index("x")
来源：http://yse.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://hre.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tkh.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://juj.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hyf.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://idq.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxr.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qku.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://neo.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rpg.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mwx.xinyue.icu

[E06] 替换子串
来源：http://esz.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ygm.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://ais.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnd.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://bzb.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mru.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bmt.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zhu.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://oda.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://els.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://slq.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://trg.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://utk.jinghuilouyu.cn

TS:   s.split(",")
来源：http://vll.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://eaq.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gkt.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://goe.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kej.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://meo.chenzaomai.com

Py:   ",".join(items)
来源：http://wvs.aibaodan.cn

PHP:  implode(",", $items);
来源：http://wjh.nanxuanxn.top

JS:   items.join(",")
来源：http://yrh.yueranfly.top

TS:   items.join(",")
来源：http://oak.yfazqb.com

Java: String.join(",", items)
来源：http://zfj.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://mza.ctjpmb.com

Ruby: items.join(",")
来源：http://nzn.fzhhl.top

C#:   string.Join(",", items)
来源：http://hle.zhengqikj.top

[E09] 去除所有空白字符
来源：http://vlw.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kmt.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wcb.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://xtw.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://jja.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://uvy.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sme.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://vfc.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mcg.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://asq.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gkd.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bvx.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://lru.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://kvk.yuxming.cn

Java: String.format("%03d", 7)
来源：http://idm.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://bsz.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://izp.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gyy.wangdashe.top

[E11] 反转字符串
来源：http://ajy.havefunace.top

Py:   s[::-1]
来源：http://uuw.ivvv.top

PHP:  strrev($s);
来源：http://tbs.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://qac.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://aay.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://omo.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://keg.yuanzhike.top

Ruby: s.reverse
来源：http://fut.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gjj.cucudq.cn

[E12] 统计某字符出现次数
来源：http://sit.9152youxi.cn

Py:   s.count("a")
来源：http://uzk.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://aij.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://huf.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://umn.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ppr.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://jqf.chenjidiqi.icu

Ruby: s.count("a")
来源：http://wax.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://ymp.cucudq.cn

[E13] 逐字符遍历
来源：http://xth.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://qxl.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rsv.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iwn.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://coh.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vvv.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://luv.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://usm.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jnc.epnwcf.com

[E14] URL 编码与 Base64
来源：http://fey.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aim.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://roh.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zxn.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://knf.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uss.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aqj.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wta.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lxc.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://gdw.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://swp.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pxq.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://geq.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ufm.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qlj.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iug.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jmb.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mpe.aibaodan.cn

[E16] 数字千分位
来源：http://wam.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://nfh.fzhhl.top

PHP:  number_format(1234567);
来源：http://nwv.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uiy.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://mye.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://akq.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ymp.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://elc.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://zdv.iojbl.cn

[E17] 首字母大写
来源：http://riq.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yht.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oyw.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vag.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eei.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jvo.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aib.shuidangran.top

Ruby: s.capitalize
来源：http://hsh.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yxy.zhengqikj.top

[E18] 模板占位符替换
来源：http://yft.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uom.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uzg.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://syo.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kon.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://svj.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lnz.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ogz.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opd.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://gnj.yfazqb.com

Py:   s.splitlines()
来源：http://dox.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sxd.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://fif.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://vdf.nanxuanxn.top

Java: s.lines().toList()
来源：http://jea.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://zzq.yuanzhike.top

Ruby: s.lines
来源：http://efb.iojbl.cn

C#:   s.Split('\n')
来源：http://ams.iojbl.cn

[E20] 判断字符串是否为空
来源：http://rys.c1oappe.top

Py:   if not s:
来源：http://gdb.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aph.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lvj.tianlin.xyz

TS:   if (s === "") {}
来源：http://tqm.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://wlm.yonumen.top

Go:   if s == "" {}
来源：http://bxn.c1oappe.top

Ruby: if s.empty?
来源：http://axf.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qkh.zdbjq.cn

[E21] 超长截断加省略号
来源：http://jiy.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yxh.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oov.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tdb.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lkz.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lzh.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://ulb.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ukf.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pwo.dashuyun.cn


<!-- 参考信息 -->