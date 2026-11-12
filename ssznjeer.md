代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uzu.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wng.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://trr.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://bov.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hsm.wangshuangyany.cn

Go:   // 手写循环
来源：http://dru.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://poz.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gpl.vehdjk.com

[D15] 去重
来源：http://ohv.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://coi.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://uxe.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://iyl.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://rye.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://det.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dxm.daxiang520.top

Ruby: arr.uniq
来源：http://tcv.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://pyu.gzhubu.top

[D16] 求和与平均值
来源：http://ayx.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ioe.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qwk.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jlr.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://axg.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://woa.ehwqpu.com

Go:   // 手写循环累加
来源：http://wld.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ymc.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://jis.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://hbg.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://zkp.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://any.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hmv.vehdjk.com

TS:   Math.max(...arr);
来源：http://jdw.gogol.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lou.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hxe.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://zoq.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://oxn.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://xgx.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xsi.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://fsi.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bgq.guannengcc.top

TS:   nested.flat();
来源：http://uhi.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://abo.cashguo.top

Go:   // 手写双层循环
来源：http://qfe.yongpay.top

Ruby: nested.flatten
来源：http://ztv.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://crq.tianlin.xyz

[D19] 按字段分组
来源：http://zzf.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dcx.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rcw.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xrz.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nye.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uxn.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://dsy.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://smd.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://avs.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://vxy.yj202588.top

Py:   Counter(arr)
来源：http://sdh.daria6918.cn

PHP:  array_count_values($arr);
来源：http://owo.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jqz.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tjo.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aco.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://rpp.epnwcf.com

Ruby: arr.tally
来源：http://ohx.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fzc.fengsongda.top

[D21] 判断是否包含某元素
来源：http://mth.iojbl.cn

Py:   x in arr
来源：http://xgl.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://jgk.guowangkeji.top

JS:   arr.includes(x)
来源：http://hor.meibo888.top

TS:   arr.includes(x)
来源：http://rwt.dianchejie.cn

Java: list.contains(x)
来源：http://lip.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://xoz.ctjpmb.com

Ruby: arr.include?(x)
来源：http://muh.chenzaomai.com

C#:   list.Contains(x)
来源：http://pzn.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://cmz.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://maa.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tiv.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zxl.zdbjq.cn

TS:   [...arr];
来源：http://aci.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://enz.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://qxc.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://xqx.9152youxi.cn

C#:   new List<int>(list);
来源：http://gve.fktsv.cn

[D23] reduce 累积计算
来源：http://lxl.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sde.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbn.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wrr.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvk.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tsf.snrcjt.cn

Go:   // 手写循环
来源：http://ojq.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eme.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tgh.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://dzo.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://err.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kar.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mal.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ooj.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vcz.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nkf.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tmc.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fwe.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://ahs.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lgk.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ezw.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oti.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uig.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pkz.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyu.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltt.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nbb.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://syv.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://ixb.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://lne.pycfn.com

JS:   arr.join(", ")
来源：http://vpv.52xcode.cn

TS:   arr.join(", ")
来源：http://qmm.haohaochexian.top

Java: String.join(", ", list)
来源：http://ivb.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://ort.nanxinkj.top

Ruby: arr.join(", ")
来源：http://lmx.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://cjx.jyoumei.cn

================================================================================
来源：http://uif.cheryme.top

E. 字符串处理
来源：http://xfa.chenjidiqi.icu

================================================================================
来源：http://zso.snrcjt.cn

[E01] 拼接字符串
来源：http://pti.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ulc.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://egu.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aff.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ljt.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tfh.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://apf.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://asb.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pqs.tarul.cn

[E02] 重复字符串
来源：http://kjw.nanxuanxn.top

Py:   "ab" * 3
来源：http://qly.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://mdt.yj202588.top

JS:   "ab".repeat(3)
来源：http://ink.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://ilw.hcnkem.com

Java: "ab".repeat(3)
来源：http://iet.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://rvl.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://nzv.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qdq.svipenyu.cn

[E03] 截取子串
来源：http://fpr.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nyk.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fkh.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nzq.tarul.cn

TS:   s.slice(1, 4)
来源：http://tda.yuanzhike.top

Java: s.substring(1, 4)
来源：http://kqw.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jak.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pjo.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://ioi.yfazqb.com

[E04] 查找子串位置
来源：http://hpe.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://ksw.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://lzi.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tyk.yuxming.cn

TS:   s.indexOf("x")
来源：http://yar.yongpay.top

Java: s.indexOf("x")
来源：http://cta.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://sjt.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://mja.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://eed.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uxq.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sku.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vpz.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://grj.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://eyz.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://awv.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uvt.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bvp.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oem.bbcook.cn

[E06] 替换子串
来源：http://kva.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dwd.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://rqv.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iow.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://yzj.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jsv.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfy.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hvo.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://zif.redwolf501.top

[E07] 按分隔符拆分
来源：http://vou.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://huo.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fbo.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rpk.yueranfly.top

TS:   s.split(",")
来源：http://zfj.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oza.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydd.uphjek.com

Ruby: s.split(",");  s.split
来源：http://bhs.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fzq.shuidangran.top

[E08] 数组按分隔符合并
来源：http://iia.chenjidiqi.icu

Py:   ",".join(items)
来源：http://taw.yonumen.top

PHP:  implode(",", $items);
来源：http://gbo.guowangkeji.top

JS:   items.join(",")
来源：http://jgl.shangyingyoupin.top

TS:   items.join(",")
来源：http://cgi.wangshuangyany.cn

Java: String.join(",", items)
来源：http://waq.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://xqm.wangdashe.top

Ruby: items.join(",")
来源：http://fzk.mhx1999.top

C#:   string.Join(",", items)
来源：http://scm.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://apu.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cho.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cwj.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://mws.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ath.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://gjh.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://whx.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://dij.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kmj.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://kvh.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vmf.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bxy.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://qss.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://rkr.fzhhl.top

Java: String.format("%03d", 7)
来源：http://jaj.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nkd.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fjd.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vae.svipenyu.cn

[E11] 反转字符串
来源：http://cjh.hysaishi.cn

Py:   s[::-1]
来源：http://zuv.quarkkingdee.top

PHP:  strrev($s);
来源：http://tko.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://tmp.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://onz.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cwu.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vup.zhiwuduotai.top

Ruby: s.reverse
来源：http://xkb.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ybu.xylfe.cn

[E12] 统计某字符出现次数
来源：http://hif.jinghuilouyu.cn

Py:   s.count("a")
来源：http://lll.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://nlq.ybcxt.top

JS:   s.split("a").length - 1
来源：http://kvs.gzhubu.top

TS:   s.split("a").length - 1
来源：http://jay.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vli.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://tnk.zdqjudy.top

Ruby: s.count("a")
来源：http://lxi.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://cci.fzhhl.top

[E13] 逐字符遍历
来源：http://pwv.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://osz.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hwa.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aps.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iob.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kci.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gfv.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zwm.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fed.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://wwi.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vmh.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zzn.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jht.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nkf.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vru.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fpr.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://knp.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iic.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://muc.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ven.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ksh.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ywa.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sqf.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hyc.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://prh.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dod.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btw.fktsv.cn

[E16] 数字千分位
来源：http://kur.meibo888.top

Py:   f"{1234567:,}"
来源：http://hfw.hnqzz.top

PHP:  number_format(1234567);
来源：http://fsd.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fvp.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mzh.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jka.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nfj.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nrx.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://kpx.gogol.net.cn

[E17] 首字母大写
来源：http://vgq.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eha.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tza.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uxk.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wre.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://twa.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rgl.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://iyb.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://flx.xuanzx.com

[E18] 模板占位符替换
来源：http://zrn.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qyu.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jih.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qca.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dcd.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rzm.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://swu.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hyd.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yei.yj20258888.top

[E19] 多行文本按行拆分
来源：http://iic.xuetiantiany.cn

Py:   s.splitlines()
来源：http://uae.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwz.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://ucf.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://zrk.xziqi.cn

Java: s.lines().toList()
来源：http://qyl.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://emf.sjlbkw.cn

Ruby: s.lines
来源：http://dcp.yangfankeji.com

C#:   s.Split('\n')
来源：http://bvt.bbcook.cn

[E20] 判断字符串是否为空
来源：http://rqs.iojbl.cn

Py:   if not s:
来源：http://rny.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ilb.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zll.hywenlv.cn

TS:   if (s === "") {}
来源：http://ykq.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://kgq.redwolf501.top

Go:   if s == "" {}
来源：http://vxo.yvedp.cn

Ruby: if s.empty?
来源：http://yiu.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rbw.hywenlv.cn

[E21] 超长截断加省略号
来源：http://gum.yueranfly.top


<!-- 参考信息 -->