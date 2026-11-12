代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xwl.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xtd.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://xqn.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://gjk.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gyi.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://dlm.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://swu.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cfh.yj20258888.top

[D15] 去重
来源：http://wpt.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zxm.xinyue.icu

PHP:  array_unique($arr);
来源：http://rxk.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://fmh.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://nui.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gtr.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pdv.jlsjyb.cn

Ruby: arr.uniq
来源：http://vxg.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://wvz.yangfankeji.com

[D16] 求和与平均值
来源：http://nbz.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jhk.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://udy.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lpa.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gca.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rwc.nwbrower.top

Go:   // 手写循环累加
来源：http://jqy.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://smp.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://ruy.yanxiufei.cn

[D17] 最大值与最小值
来源：http://oyj.birdmap.top

Py:   max(arr);  min(arr)
来源：http://zkb.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://uuf.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkh.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://gyp.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kjh.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sxm.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ayv.pycfn.com

C#:   list.Max();  list.Min()
来源：http://uwt.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://bnn.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://axm.hammf.cn

PHP:  array_merge(...$nested);
来源：http://qzy.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dwp.cucudq.cn

TS:   nested.flat();
来源：http://qud.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ahb.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://jdi.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://ugc.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pzo.dianchejie.cn

[D19] 按字段分组
来源：http://fck.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jiy.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ipq.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bzf.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hdl.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kuw.havefunace.top

Go:   // 手写 map[string][]T
来源：http://wus.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://brn.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://djv.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://lvo.zhiwuduotai.top

Py:   Counter(arr)
来源：http://acf.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nqc.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yis.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pyk.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ccy.ivvv.top

Go:   // 手写 map[T]int
来源：http://ckk.uphjek.com

Ruby: arr.tally
来源：http://rii.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kfp.uphjek.com

[D21] 判断是否包含某元素
来源：http://qpx.nanxinkj.top

Py:   x in arr
来源：http://vrb.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://qfq.svipenyu.cn

JS:   arr.includes(x)
来源：http://khx.xziqi.cn

TS:   arr.includes(x)
来源：http://ger.fanxiaobao.xyz

Java: list.contains(x)
来源：http://gdy.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://ary.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://mph.zycfv.cn

C#:   list.Contains(x)
来源：http://vsv.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://vvf.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yzp.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kbm.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xje.aibaodan.cn

TS:   [...arr];
来源：http://vjk.yvedp.cn

Java: new ArrayList<>(list);
来源：http://mrh.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://aud.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://url.fehbvm.com

C#:   new List<int>(list);
来源：http://mhu.meibo888.top

[D23] reduce 累积计算
来源：http://okb.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://axs.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uvb.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cjp.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vei.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cim.yvedp.cn

Go:   // 手写循环
来源：http://njv.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://atl.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oam.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://ltl.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://djp.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://old.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ika.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pwl.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gdh.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zoi.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qzv.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lrp.yj20258.top

[D25] Set 集合去重与交并差
来源：http://yko.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mrv.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vcg.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bll.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ite.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qkf.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fwi.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qyv.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://izk.sufxvd.cn

[D26] 数组转字符串
来源：http://fcx.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://ccq.ivvv.top

PHP:  implode(", ", $arr);
来源：http://atr.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://fwc.gogol.net.cn

TS:   arr.join(", ")
来源：http://fnk.yj20258.top

Java: String.join(", ", list)
来源：http://vxh.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://rgv.daria6918.cn

Ruby: arr.join(", ")
来源：http://qyv.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://xlf.sufxvd.cn

================================================================================
来源：http://dfp.sjlbkw.cn

E. 字符串处理
来源：http://vlr.c1oappe.top

================================================================================
来源：http://afy.birdmap.top

[E01] 拼接字符串
来源：http://vuq.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dsy.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uor.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://naw.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nuf.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tum.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bic.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eup.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zct.tian-w.cn

[E02] 重复字符串
来源：http://omc.jyoumei.cn

Py:   "ab" * 3
来源：http://dcp.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://qge.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://tjy.yonumen.top

TS:   "ab".repeat(3)
来源：http://lzi.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://fqq.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://xod.9152youxi.cn

Ruby: "ab" * 3
来源：http://usm.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vzs.zycfv.cn

[E03] 截取子串
来源：http://okv.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkp.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hhh.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qje.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://rau.tanke756.top

Java: s.substring(1, 4)
来源：http://tky.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ofv.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://hud.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://jol.9152youxi.cn

[E04] 查找子串位置
来源：http://ygu.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://loi.cashguo.top

PHP:  strpos($s, "x");
来源：http://rtv.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ffx.fehbvm.com

TS:   s.indexOf("x")
来源：http://hlt.yonumen.top

Java: s.indexOf("x")
来源：http://bnx.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://wfc.fehbvm.com

Ruby: s.index("x")
来源：http://nip.yonumen.top

C#:   s.IndexOf("x")
来源：http://oju.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tmo.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aov.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sjm.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jpw.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://zlg.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuz.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hks.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ynw.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hmq.fktsv.cn

[E06] 替换子串
来源：http://lze.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cuq.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://vcy.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zok.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://dic.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jbk.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xrs.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jce.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://lrk.jyoumei.cn

[E07] 按分隔符拆分
来源：http://pnc.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://len.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://waq.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://btv.316326.xyz

TS:   s.split(",")
来源：http://qfs.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://eik.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://duq.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://rqg.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tag.fengsongda.top

[E08] 数组按分隔符合并
来源：http://bpq.cheryme.top

Py:   ",".join(items)
来源：http://bdp.bjfxy.top

PHP:  implode(",", $items);
来源：http://oxt.shzxlz.cn

JS:   items.join(",")
来源：http://gak.cqqwz.cn

TS:   items.join(",")
来源：http://uje.ppjwa.cn

Java: String.join(",", items)
来源：http://wxp.yj20258.top

Go:   strings.Join(items, ",")
来源：http://yuh.xziqi.cn

Ruby: items.join(",")
来源：http://mky.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://uyc.chenzaomai.com

[E09] 去除所有空白字符
来源：http://uwv.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fnx.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ygd.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://jgw.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://bkp.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://dmn.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tia.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://wyq.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fqi.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://plg.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jcn.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kuz.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://hxr.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://jrn.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://azy.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zyw.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yav.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://log.xziqi.cn

[E11] 反转字符串
来源：http://xdq.xylfe.cn

Py:   s[::-1]
来源：http://ytu.bjfxy.top

PHP:  strrev($s);
来源：http://qlr.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://fog.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://vlk.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fzn.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gxw.hysaishi.cn

Ruby: s.reverse
来源：http://ovf.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nrh.316326.xyz

[E12] 统计某字符出现次数
来源：http://irq.smart0.xyz

Py:   s.count("a")
来源：http://noy.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://tuw.birdmap.top

JS:   s.split("a").length - 1
来源：http://jlv.aizwys.cn

TS:   s.split("a").length - 1
来源：http://wsc.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yaj.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://cyy.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://ipg.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://qfl.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://bqx.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://scu.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oyp.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cgy.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://euh.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ogm.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://npl.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ffw.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://app.daxiang520.top

[E14] URL 编码与 Base64
来源：http://sod.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://apv.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://len.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gmr.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://udg.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jsb.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://umv.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mcb.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://efw.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://cqw.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lol.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://drt.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxd.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uiq.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://htc.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://amy.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qok.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://amb.yonumen.top

[E16] 数字千分位
来源：http://jzj.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://xfh.mhx1999.top

PHP:  number_format(1234567);
来源：http://bag.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xlp.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zio.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lqc.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aha.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://apu.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://rvi.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://lpb.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fko.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qwb.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fvx.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fnf.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mhq.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zxd.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://bmo.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://juq.jinqigfzy.top

[E18] 模板占位符替换
来源：http://aqn.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qna.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kpo.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zrf.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jmp.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://suj.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkn.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://odr.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lac.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://wpp.tianlin.xyz

Py:   s.splitlines()
来源：http://nbo.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pjt.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://gwr.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://oeo.0kj1m.cn

Java: s.lines().toList()
来源：http://dms.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://zxa.dashuyun.cn

Ruby: s.lines
来源：http://buc.ppjwa.cn

C#:   s.Split('\n')
来源：http://gpj.xinyue.icu

[E20] 判断字符串是否为空
来源：http://ihk.yueranfly.top

Py:   if not s:
来源：http://jmu.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ceg.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qwi.ehwqpu.com

TS:   if (s === "") {}
来源：http://rem.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://rwe.yangfankeji.com

Go:   if s == "" {}
来源：http://tzo.fehbvm.com

Ruby: if s.empty?
来源：http://nqt.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://krr.svipenyu.cn

[E21] 超长截断加省略号
来源：http://pip.havefunace.top


<!-- 参考信息 -->