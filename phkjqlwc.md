代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://eyi.sysykeji.top

Go:   // 手写循环
来源：http://fop.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://hqj.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://yzv.ehwqpu.com

[D15] 去重
来源：http://pac.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sic.yuanzhike.top

PHP:  array_unique($arr);
来源：http://vgo.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://wkq.ybcxt.top

TS:   [...new Set(arr)]
来源：http://srj.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jxm.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://efz.dianchejie.cn

Ruby: arr.uniq
来源：http://xbm.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://wom.birdmap.top

[D16] 求和与平均值
来源：http://uok.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nhs.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gxx.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pzu.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mae.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qgb.sweek.top

Go:   // 手写循环累加
来源：http://fby.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tsv.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://wbb.yj20258.top

[D17] 最大值与最小值
来源：http://jxz.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://hbk.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://fmg.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tnm.hcnkem.com

TS:   Math.max(...arr);
来源：http://ppd.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cev.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bqp.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://eek.hammf.cn

C#:   list.Max();  list.Min()
来源：http://fqi.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://jph.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wuh.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://aci.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bwo.zhoulong.xyz

TS:   nested.flat();
来源：http://xfa.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mgl.jqgufenzy.top

Go:   // 手写双层循环
来源：http://jrm.shuidangran.top

Ruby: nested.flatten
来源：http://yuy.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vcq.aibaodan.cn

[D19] 按字段分组
来源：http://kwr.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vtf.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqx.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uwx.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://emh.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zba.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://hvn.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://bzd.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pli.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://ray.andypj.xyz

Py:   Counter(arr)
来源：http://ghq.sysykeji.top

PHP:  array_count_values($arr);
来源：http://xae.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ttj.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zmh.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://srz.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://ryd.hongshengwenyu.top

Ruby: arr.tally
来源：http://nuv.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://awb.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://lig.andypj.xyz

Py:   x in arr
来源：http://jyq.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://eux.sysykeji.top

JS:   arr.includes(x)
来源：http://hav.zhijiandao.cn

TS:   arr.includes(x)
来源：http://aqv.jianghu66.top

Java: list.contains(x)
来源：http://eft.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://zhf.yonumen.top

Ruby: arr.include?(x)
来源：http://cbs.daria6918.cn

C#:   list.Contains(x)
来源：http://yxg.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://lxn.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wxl.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dxl.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lxs.zdbjq.cn

TS:   [...arr];
来源：http://tcs.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://ced.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wue.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://mfk.hnqzz.top

C#:   new List<int>(list);
来源：http://ybx.ppjwa.cn

[D23] reduce 累积计算
来源：http://sbn.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mqc.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wrh.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqs.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sis.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxb.hcnkem.com

Go:   // 手写循环
来源：http://cmf.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkk.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://prw.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://icf.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iiy.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gkz.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uqy.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wwh.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qkm.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lgr.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pfq.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ytj.yj20258.top

[D25] Set 集合去重与交并差
来源：http://rpk.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hlr.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mxn.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ptv.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jng.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ojm.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eqy.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hkn.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kab.smart0.xyz

[D26] 数组转字符串
来源：http://gkk.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://jqf.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://pbq.jianghu66.top

JS:   arr.join(", ")
来源：http://efo.hywenlv.cn

TS:   arr.join(", ")
来源：http://kgq.jinqigfzy.top

Java: String.join(", ", list)
来源：http://emm.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://fxt.jianghu66.top

Ruby: arr.join(", ")
来源：http://mdk.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://hpe.yonumen.top

================================================================================
来源：http://xpc.fehbvm.com

E. 字符串处理
来源：http://tjb.ybcxt.top

================================================================================
来源：http://pxb.52xcode.cn

[E01] 拼接字符串
来源：http://ddv.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pmv.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hak.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxz.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfz.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lon.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ewg.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sgy.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fnb.pycfn.com

[E02] 重复字符串
来源：http://bke.gogol.net.cn

Py:   "ab" * 3
来源：http://mcq.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://mqi.316326.xyz

JS:   "ab".repeat(3)
来源：http://bms.fktsv.cn

TS:   "ab".repeat(3)
来源：http://qer.ppjwa.cn

Java: "ab".repeat(3)
来源：http://ajm.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://tbe.zhengqikj.top

Ruby: "ab" * 3
来源：http://pmp.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qqb.daxiang520.top

[E03] 截取子串
来源：http://kqs.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ioz.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://seq.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bvi.vehdjk.com

TS:   s.slice(1, 4)
来源：http://tbv.cashguo.top

Java: s.substring(1, 4)
来源：http://pwm.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jqb.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qzc.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://lvl.epnwcf.com

[E04] 查找子串位置
来源：http://qus.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://bst.yfazqb.com

PHP:  strpos($s, "x");
来源：http://viy.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rzh.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://onn.sufxvd.cn

Java: s.indexOf("x")
来源：http://jon.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://egl.jqgufenzy.top

Ruby: s.index("x")
来源：http://zli.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://stm.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zej.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ztl.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zwx.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygo.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uwi.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fcg.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cho.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://moc.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nmp.yongpay.top

[E06] 替换子串
来源：http://rjg.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gcs.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://bbl.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://plc.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://cop.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rnh.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ctt.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mjt.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://jlt.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://bxu.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gml.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yrh.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://crf.yueranfly.top

TS:   s.split(",")
来源：http://zgi.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://bqg.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vyp.pycfn.com

Ruby: s.split(",");  s.split
来源：http://mgd.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ldu.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://tql.sweek.top

Py:   ",".join(items)
来源：http://sdt.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://wmm.wangdashe.top

JS:   items.join(",")
来源：http://zsk.zhongyouzk.top

TS:   items.join(",")
来源：http://cfl.iojbl.cn

Java: String.join(",", items)
来源：http://hcq.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://tyk.snrcjt.cn

Ruby: items.join(",")
来源：http://jnt.zhengqikj.top

C#:   string.Join(",", items)
来源：http://kco.dashuyun.cn

[E09] 去除所有空白字符
来源：http://nfh.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eox.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffo.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://voe.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://tou.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://yeb.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vuo.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cgg.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmo.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://kux.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kyf.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fay.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://ngu.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://var.xuanzx.com

Java: String.format("%03d", 7)
来源：http://zzi.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tny.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dyh.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gyl.birdmap.top

[E11] 反转字符串
来源：http://txm.yanxiufei.cn

Py:   s[::-1]
来源：http://muu.zhijiandao.cn

PHP:  strrev($s);
来源：http://obw.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://lrq.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://yrq.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://phs.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nuy.zdbjq.cn

Ruby: s.reverse
来源：http://wkg.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://sxk.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://czj.sysykeji.top

Py:   s.count("a")
来源：http://ydb.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://hfm.meibo888.top

JS:   s.split("a").length - 1
来源：http://udu.meibo888.top

TS:   s.split("a").length - 1
来源：http://sgm.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://egc.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://kcg.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://idl.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://brx.ehwqpu.com

[E13] 逐字符遍历
来源：http://wuu.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://jtp.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jwm.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ieh.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://jyo.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://osd.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oev.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bgu.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zyx.wangdashe.top

[E14] URL 编码与 Base64
来源：http://avv.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hph.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ulf.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ikf.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ezp.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txn.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kod.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fkp.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iwe.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://vzh.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cmy.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://imc.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wxa.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ziz.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rma.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vxp.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zbg.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lsw.hongshengwenyu.top

[E16] 数字千分位
来源：http://jct.sysykeji.top

Py:   f"{1234567:,}"
来源：http://rlx.zhengqikj.top

PHP:  number_format(1234567);
来源：http://lvo.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://okc.epnwcf.com

TS:   (1234567).toLocaleString("en-US")
来源：http://fww.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nid.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cvv.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ldl.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://tob.vehdjk.com

[E17] 首字母大写
来源：http://ycf.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ziv.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nlv.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bua.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkk.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fjr.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bwl.xuanzx.com

Ruby: s.capitalize
来源：http://bet.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aze.nanxuanxn.top

[E18] 模板占位符替换
来源：http://efi.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jmf.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xvp.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fed.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://let.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lta.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xsb.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fur.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wtr.cashguo.top

[E19] 多行文本按行拆分
来源：http://bkp.hysaishi.cn

Py:   s.splitlines()
来源：http://div.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kqp.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://mbq.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://umt.bbcook.cn

Java: s.lines().toList()
来源：http://jhg.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://gqm.zhixingplan.top

Ruby: s.lines
来源：http://sry.tanke756.top

C#:   s.Split('\n')
来源：http://mhu.yonumen.top

[E20] 判断字符串是否为空
来源：http://rvs.zhoulong.xyz

Py:   if not s:
来源：http://scq.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://boh.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ovu.mhx1999.top

TS:   if (s === "") {}
来源：http://pjj.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://rba.yj202588.top

Go:   if s == "" {}
来源：http://nsv.guowangkeji.top

Ruby: if s.empty?
来源：http://xvn.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yax.hfpthk.cn

[E21] 超长截断加省略号
来源：http://dpf.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://erf.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vgp.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgn.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gwb.yonumen.top


<!-- 参考信息 -->