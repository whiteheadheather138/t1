代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hit.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uur.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://qub.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://wht.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://aoi.redwolf501.top

Go:   // 手写循环
来源：http://qww.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aph.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wlo.vehdjk.com

[D15] 去重
来源：http://vxz.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jok.chenlongwang.top

PHP:  array_unique($arr);
来源：http://sfy.fengsongda.top

JS:   [...new Set(arr)]
来源：http://vyx.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://wvw.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vys.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://eat.redwolf501.top

Ruby: arr.uniq
来源：http://ewf.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://oyu.xylfe.cn

[D16] 求和与平均值
来源：http://jwu.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://weh.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dlm.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejq.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpj.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://krb.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://gde.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://idv.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://mxb.shzxlz.cn

[D17] 最大值与最小值
来源：http://qjz.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://csi.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://elp.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cev.svipenyu.cn

TS:   Math.max(...arr);
来源：http://jic.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tmz.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgs.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://ksm.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://pop.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://pbi.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pyl.yj202588.top

PHP:  array_merge(...$nested);
来源：http://pux.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mwa.zhiwuduotai.top

TS:   nested.flat();
来源：http://phb.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jiv.zycfv.cn

Go:   // 手写双层循环
来源：http://wok.zhiwuduotai.top

Ruby: nested.flatten
来源：http://dpd.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sdn.gogol.net.cn

[D19] 按字段分组
来源：http://tcl.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tcn.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jph.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://onz.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvt.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kbn.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://kbe.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://afi.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cal.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://hgv.cheryme.top

Py:   Counter(arr)
来源：http://mog.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://kcp.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uon.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://the.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mbc.vehdjk.com

Go:   // 手写 map[T]int
来源：http://icp.nanxinkj.top

Ruby: arr.tally
来源：http://mxw.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dtr.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://fdl.nanxinkj.top

Py:   x in arr
来源：http://six.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://iis.zhijiandao.cn

JS:   arr.includes(x)
来源：http://ynw.fengsongda.top

TS:   arr.includes(x)
来源：http://wfs.9152youxi.cn

Java: list.contains(x)
来源：http://tkh.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://ycy.yangfankeji.com

Ruby: arr.include?(x)
来源：http://fex.cheryme.top

C#:   list.Contains(x)
来源：http://xfy.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://hqu.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fpx.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tik.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://awc.fanxiaobao.xyz

TS:   [...arr];
来源：http://cus.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://khd.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://ugf.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://cxs.nanxuanxn.top

C#:   new List<int>(list);
来源：http://iqw.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://wle.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iuv.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://avq.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://inq.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fhk.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://odo.chenjidiqi.icu

Go:   // 手写循环
来源：http://ase.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vpk.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tqo.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://irr.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lzr.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jzt.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wse.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tlx.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qyu.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cyr.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://znc.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vlj.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://kab.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xzt.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qen.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mmn.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nsg.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://syw.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kgh.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvc.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nnc.yangfankeji.com

[D26] 数组转字符串
来源：http://qnv.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://ltb.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://noq.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://wzl.pycfn.com

TS:   arr.join(", ")
来源：http://xjs.ppjwa.cn

Java: String.join(", ", list)
来源：http://xny.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://hwd.fzhhl.top

Ruby: arr.join(", ")
来源：http://pxv.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://ihr.fktsv.cn

================================================================================
来源：http://rkt.havefunace.top

E. 字符串处理
来源：http://hre.shzxlz.cn

================================================================================
来源：http://qkh.hongshengwenyu.top

[E01] 拼接字符串
来源：http://tzw.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yne.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kjs.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://awp.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbo.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://svs.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kgy.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://das.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jtb.smart0.xyz

[E02] 重复字符串
来源：http://kjs.sjlbkw.cn

Py:   "ab" * 3
来源：http://kht.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://seg.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://yhz.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://rya.guannengcc.top

Java: "ab".repeat(3)
来源：http://dly.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://usr.ybcxt.top

Ruby: "ab" * 3
来源：http://uur.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bmg.yueranfly.top

[E03] 截取子串
来源：http://ozk.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hwg.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://soz.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ask.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://zvf.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://gzz.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dxi.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qcg.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://twr.sweek.top

[E04] 查找子串位置
来源：http://igx.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://qwz.c1oappe.top

PHP:  strpos($s, "x");
来源：http://rfu.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dbw.xinyue.icu

TS:   s.indexOf("x")
来源：http://fxa.nanxinkj.top

Java: s.indexOf("x")
来源：http://cyx.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://rqt.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://ukw.fktsv.cn

C#:   s.IndexOf("x")
来源：http://euq.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sya.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aqe.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hqi.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzc.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://yjh.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://smf.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sgv.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zwd.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ote.ywan-chungtsiang.top

[E06] 替换子串
来源：http://lao.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmr.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://bfe.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vek.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://fox.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lqw.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wtt.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fdn.yj20258.top

C#:   s.Replace("a", "b")
来源：http://htb.jyoumei.cn

[E07] 按分隔符拆分
来源：http://duw.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bax.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pmi.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktx.ybcxt.top

TS:   s.split(",")
来源：http://vqc.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kxg.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lhf.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://ytj.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pqg.sweek.top

[E08] 数组按分隔符合并
来源：http://cjm.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://qlh.dashuyun.cn

PHP:  implode(",", $items);
来源：http://ing.zhijiandao.cn

JS:   items.join(",")
来源：http://hkl.cdnleiting.top

TS:   items.join(",")
来源：http://zkp.dianchejie.cn

Java: String.join(",", items)
来源：http://mhv.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://cnx.jiagoushi.top

Ruby: items.join(",")
来源：http://rck.cheryme.top

C#:   string.Join(",", items)
来源：http://ceb.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://bxu.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://coq.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zsv.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://lew.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://xax.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://qcf.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ffq.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://zms.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jmx.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://pxa.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oiy.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vip.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://iuj.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://maq.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://dao.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://efd.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mja.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cds.ybcxt.top

[E11] 反转字符串
来源：http://eqs.haohaochexian.top

Py:   s[::-1]
来源：http://mij.gaohongyu789.top

PHP:  strrev($s);
来源：http://dgc.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://pxf.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://fvi.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gzn.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://snc.kuanghao11.cn

Ruby: s.reverse
来源：http://tkp.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zir.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://trk.hnxiangtu.top

Py:   s.count("a")
来源：http://wgm.tanke756.top

PHP:  substr_count($s, "a");
来源：http://ctk.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://wed.pycfn.com

TS:   s.split("a").length - 1
来源：http://cwq.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://axf.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://juq.snrcjt.cn

Ruby: s.count("a")
来源：http://quu.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://ocl.daxiang520.top

[E13] 逐字符遍历
来源：http://odp.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://xte.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://efd.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jdf.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kxv.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lvc.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sll.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wyo.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://daj.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://yrc.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iyf.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sxx.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ksq.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xig.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mlm.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wxk.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yaj.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://irc.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://tyf.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wdu.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cqc.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ivz.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hcv.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zfq.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://glx.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jvu.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kpf.sjlbkw.cn

[E16] 数字千分位
来源：http://hrg.hnqzz.top

Py:   f"{1234567:,}"
来源：http://cpi.bjfxy.top

PHP:  number_format(1234567);
来源：http://nyh.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xpe.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ydu.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zig.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ohb.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bew.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://gns.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://miw.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nvj.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://mlw.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hjn.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lhr.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knb.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://voy.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://xxf.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://azp.gaohongyu789.top

[E18] 模板占位符替换
来源：http://uno.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ocw.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ede.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rav.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xal.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zzi.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://caq.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pcn.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://juz.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://wxn.xuetiantiany.cn

Py:   s.splitlines()
来源：http://umb.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zav.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://oeb.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://chd.tian-w.cn

Java: s.lines().toList()
来源：http://sry.wangshuangyany.cn

Go:   strings.Split(s, "\n")
来源：http://ogx.daria6918.cn

Ruby: s.lines
来源：http://pfw.yuxming.cn

C#:   s.Split('\n')
来源：http://kxv.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://wff.jinghuilouyu.cn

Py:   if not s:
来源：http://vwa.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cje.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mgb.chenlongwang.top

TS:   if (s === "") {}
来源：http://owz.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://adh.zhiwuduotai.top

Go:   if s == "" {}
来源：http://wzw.yonumen.top

Ruby: if s.empty?
来源：http://hhx.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://noh.hnqzz.top

[E21] 超长截断加省略号
来源：http://fhw.uphjek.com


<!-- 参考信息 -->