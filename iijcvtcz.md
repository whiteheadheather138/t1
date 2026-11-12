代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://omu.tarul.cn

Go:   // 手写循环
来源：http://hjn.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zcq.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fcx.gogol.net.cn

[D15] 去重
来源：http://sps.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gsr.nwbrower.top

PHP:  array_unique($arr);
来源：http://rhu.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://kwn.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://zef.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vkp.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ukb.zhongyouzk.top

Ruby: arr.uniq
来源：http://wrn.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://esf.jianghu66.top

[D16] 求和与平均值
来源：http://crg.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pwj.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uai.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://njk.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vtt.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bpk.ppjwa.cn

Go:   // 手写循环累加
来源：http://hyt.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qtk.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://nyw.guannengcc.top

[D17] 最大值与最小值
来源：http://dxw.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://ylb.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://ekd.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oqe.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://svf.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ynk.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgw.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://miw.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://fov.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://zqj.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hnz.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://ren.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gmk.hongshengwenyu.top

TS:   nested.flat();
来源：http://txa.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nai.yuanzhike.top

Go:   // 手写双层循环
来源：http://vvd.chenjidiqi.icu

Ruby: nested.flatten
来源：http://fid.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mny.sjlbkw.cn

[D19] 按字段分组
来源：http://xid.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://few.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://beh.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pfm.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://puo.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://siq.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://csa.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gud.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gdi.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://hms.kuanghao11.cn

Py:   Counter(arr)
来源：http://hot.daxiang520.top

PHP:  array_count_values($arr);
来源：http://piv.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcr.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgy.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lkm.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://yat.yueranfly.top

Ruby: arr.tally
来源：http://qtp.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ije.jianghu66.top

[D21] 判断是否包含某元素
来源：http://ddn.fengsongda.top

Py:   x in arr
来源：http://cdk.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://gwu.hesvh.cn

JS:   arr.includes(x)
来源：http://hmb.52xcode.cn

TS:   arr.includes(x)
来源：http://fbd.tanke756.top

Java: list.contains(x)
来源：http://jww.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://zto.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://sft.ctjpmb.com

C#:   list.Contains(x)
来源：http://zqk.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://qgs.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ukn.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lgf.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fot.hnxiangtu.top

TS:   [...arr];
来源：http://owz.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://huk.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://osc.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://wwk.xylfe.cn

C#:   new List<int>(list);
来源：http://eub.fehbvm.com

[D23] reduce 累积计算
来源：http://idd.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lxt.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pxe.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jua.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yqe.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bsz.kuanghao11.cn

Go:   // 手写循环
来源：http://ktb.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qad.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tll.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://ich.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eyz.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sju.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sqt.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oam.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fos.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://reh.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pmx.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mll.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://uhv.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pep.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xqt.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aes.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qdd.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jtk.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yph.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zrh.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://koo.xuetiantiany.cn

[D26] 数组转字符串
来源：http://pcd.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://lqy.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://udt.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://ztf.jinqigfzy.top

TS:   arr.join(", ")
来源：http://pie.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://soj.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://dqo.sxryk.cn

Ruby: arr.join(", ")
来源：http://lfh.daria6918.cn

C#:   string.Join(", ", list)
来源：http://trp.sweek.top

================================================================================
来源：http://jtn.meibo888.top

E. 字符串处理
来源：http://tin.gaohongyu789.top

================================================================================
来源：http://rft.ydzc1.top

[E01] 拼接字符串
来源：http://sry.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gov.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yhl.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://byx.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://men.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hqy.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tgr.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vyo.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tqv.cashguo.top

[E02] 重复字符串
来源：http://nux.sxryk.cn

Py:   "ab" * 3
来源：http://ast.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://bto.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://wdz.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://qje.9152youxi.cn

Java: "ab".repeat(3)
来源：http://zcm.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://khw.cqqwz.cn

Ruby: "ab" * 3
来源：http://xby.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sbw.tarul.cn

[E03] 截取子串
来源：http://chc.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ljt.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mye.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gvq.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://nru.aibaodan.cn

Java: s.substring(1, 4)
来源：http://tdg.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://avg.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://hwr.hammf.cn

C#:   s.Substring(1, 3)
来源：http://suo.daria6918.cn

[E04] 查找子串位置
来源：http://lxi.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://hyy.fzhhl.top

PHP:  strpos($s, "x");
来源：http://kzu.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hnu.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://cnl.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://lvu.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://yjw.ctjpmb.com

Ruby: s.index("x")
来源：http://tht.yonumen.top

C#:   s.IndexOf("x")
来源：http://ogx.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wnv.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lqj.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uhg.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnc.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pbc.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xwf.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sxq.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wtn.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvg.jlsjyb.cn

[E06] 替换子串
来源：http://urf.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bsf.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://por.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfa.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://djr.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://evb.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rnd.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qaw.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://dtn.sufxvd.cn

[E07] 按分隔符拆分
来源：http://kzx.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://upp.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://upz.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uix.zhongyouzk.top

TS:   s.split(",")
来源：http://bsr.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jtp.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gkl.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://ltp.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ksl.c1oappe.top

[E08] 数组按分隔符合并
来源：http://nes.dashuyun.cn

Py:   ",".join(items)
来源：http://fqa.yangfankeji.com

PHP:  implode(",", $items);
来源：http://atm.wangdashe.top

JS:   items.join(",")
来源：http://xna.hcnkem.com

TS:   items.join(",")
来源：http://txm.epnwcf.com

Java: String.join(",", items)
来源：http://inf.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://kgs.jiagoushi.top

Ruby: items.join(",")
来源：http://mkb.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://cda.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://ogp.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sfb.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzk.0kj1m.cn

JS:   s.replace(/\s+/g, "")
来源：http://grm.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://lhv.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://shq.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yth.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://wqr.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://irq.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://woe.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://knp.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vmb.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://pcv.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://ukc.tarul.cn

Java: String.format("%03d", 7)
来源：http://toy.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://byk.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esn.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bvb.ydzc1.top

[E11] 反转字符串
来源：http://zax.jyoumei.cn

Py:   s[::-1]
来源：http://szg.yuanzhike.top

PHP:  strrev($s);
来源：http://uao.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://qkf.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://tzr.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hbx.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cze.mhx1999.top

Ruby: s.reverse
来源：http://vkz.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kyb.pycfn.com

[E12] 统计某字符出现次数
来源：http://xrz.shangyingyoupin.top

Py:   s.count("a")
来源：http://kfu.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://hlu.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://ewd.tarul.cn

TS:   s.split("a").length - 1
来源：http://ywg.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xwg.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://uvf.fehbvm.com

Ruby: s.count("a")
来源：http://pvx.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://jmt.jianghu66.top

[E13] 逐字符遍历
来源：http://jtr.yongpay.top

Py:   for ch in s: print(ch)
来源：http://fcq.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gki.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cll.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zmr.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://suc.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mxl.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://twn.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uia.yj20258.top

[E14] URL 编码与 Base64
来源：http://snw.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xlk.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fhw.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mca.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jiy.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dtg.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mim.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fkb.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://upz.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://rfh.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rhm.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lqr.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oke.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://trx.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ppq.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lmq.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xrj.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cgw.mhx1999.top

[E16] 数字千分位
来源：http://yov.bjfxy.top

Py:   f"{1234567:,}"
来源：http://say.hammf.cn

PHP:  number_format(1234567);
来源：http://jar.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://erd.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xov.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rod.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://but.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uyp.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://biw.xziqi.cn

[E17] 首字母大写
来源：http://hmk.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rjh.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xgn.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://giq.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blz.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zau.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zlm.wangdashe.top

Ruby: s.capitalize
来源：http://toz.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mgu.hcnkem.com

[E18] 模板占位符替换
来源：http://zlp.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zfg.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xum.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://otr.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kxw.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tjc.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://suw.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ulg.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ryz.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://nrx.zhongyouzk.top

Py:   s.splitlines()
来源：http://clq.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mvu.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://wkd.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://nri.zdqjudy.top

Java: s.lines().toList()
来源：http://ktk.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://gqa.quarkkingdee.top

Ruby: s.lines
来源：http://ukz.316326.xyz

C#:   s.Split('\n')
来源：http://tkb.xylfe.cn

[E20] 判断字符串是否为空
来源：http://jzp.chenzaomai.com

Py:   if not s:
来源：http://lrf.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kqn.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ufa.cqqwz.cn

TS:   if (s === "") {}
来源：http://rld.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://jiu.cucudq.cn

Go:   if s == "" {}
来源：http://gwa.zhijiandao.cn

Ruby: if s.empty?
来源：http://ucv.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pvy.daria6918.cn

[E21] 超长截断加省略号
来源：http://mmw.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://unb.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nrl.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vnj.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dht.fzhhl.top


<!-- 参考信息 -->