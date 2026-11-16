代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://skt.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kth.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://hvi.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://qkp.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xky.feifeiyinyue.top

Go:   // 手写循环
来源：http://qip.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dmf.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dct.dashuyun.cn

[D15] 去重
来源：http://avr.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nmc.jinqigufen.top

PHP:  array_unique($arr);
来源：http://mtz.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://pgy.sxryk.cn

TS:   [...new Set(arr)]
来源：http://rtf.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qlt.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wyj.hongshengwenyu.top

Ruby: arr.uniq
来源：http://pwb.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://qnp.hnqzz.top

[D16] 求和与平均值
来源：http://kdf.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ebz.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ijc.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mmu.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afa.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tux.gzhubu.top

Go:   // 手写循环累加
来源：http://ryr.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ygw.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://nbu.hnxiangtu.top

[D17] 最大值与最小值
来源：http://csh.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://upx.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://gms.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qry.yj202588.top

TS:   Math.max(...arr);
来源：http://ijr.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jdd.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fcf.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://taa.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://mxp.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://ysw.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mix.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://tcx.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uuz.sxryk.cn

TS:   nested.flat();
来源：http://pfp.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wwe.gzhubu.top

Go:   // 手写双层循环
来源：http://cah.tian-w.cn

Ruby: nested.flatten
来源：http://wgx.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xmh.pycfn.com

[D19] 按字段分组
来源：http://rky.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mui.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gui.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://isk.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mlv.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fal.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://dzw.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zdk.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wrq.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://xpf.shuidangran.top

Py:   Counter(arr)
来源：http://ktm.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://kyc.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vfp.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yqp.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qad.epnwcf.com

Go:   // 手写 map[T]int
来源：http://hlz.yueranfly.top

Ruby: arr.tally
来源：http://dqt.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xpu.xylfe.cn

[D21] 判断是否包含某元素
来源：http://vjb.hesvh.cn

Py:   x in arr
来源：http://swf.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://fzp.smart0.xyz

JS:   arr.includes(x)
来源：http://rmt.smart0.xyz

TS:   arr.includes(x)
来源：http://hqr.sweek.top

Java: list.contains(x)
来源：http://iib.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://vvk.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://opm.gotoacloud.top

C#:   list.Contains(x)
来源：http://nit.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://god.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lgf.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hwn.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uir.mhx1999.top

TS:   [...arr];
来源：http://str.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://mhz.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ugk.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://eke.kuanghao11.cn

C#:   new List<int>(list);
来源：http://fgg.sjlbkw.cn

[D23] reduce 累积计算
来源：http://yme.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zwk.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ofl.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://czp.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lah.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mld.kuanghao11.cn

Go:   // 手写循环
来源：http://fcp.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mnr.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvp.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://ety.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://frm.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lst.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wuw.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yzr.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xwf.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pmj.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ffe.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wrq.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://mta.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jxd.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fhc.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vvz.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hpm.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ciz.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gje.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yzl.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://whz.hammf.cn

[D26] 数组转字符串
来源：http://gjh.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://san.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://zab.tanke756.top

JS:   arr.join(", ")
来源：http://tmj.chenzaomai.com

TS:   arr.join(", ")
来源：http://nwh.xinyue.icu

Java: String.join(", ", list)
来源：http://skx.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://gxn.sufxvd.cn

Ruby: arr.join(", ")
来源：http://aep.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://vxa.jlsjyb.cn

================================================================================
来源：http://may.jyoumei.cn

E. 字符串处理
来源：http://dui.haohaochexian.top

================================================================================
来源：http://fic.mhx1999.top

[E01] 拼接字符串
来源：http://qrv.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tkh.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nbm.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqg.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gnw.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wfz.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dhm.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kgg.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pha.wangshuangyany.cn

[E02] 重复字符串
来源：http://qdh.hcnkem.com

Py:   "ab" * 3
来源：http://wby.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://xbg.bjfxy.top

JS:   "ab".repeat(3)
来源：http://pvs.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://gpz.52xcode.cn

Java: "ab".repeat(3)
来源：http://wpk.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://zot.aibaodan.cn

Ruby: "ab" * 3
来源：http://oou.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddv.andypj.xyz

[E03] 截取子串
来源：http://xfi.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ewl.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tgc.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tpn.sxryk.cn

TS:   s.slice(1, 4)
来源：http://tic.yfazqb.com

Java: s.substring(1, 4)
来源：http://uwj.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wmn.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nxw.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://wzl.shuidangran.top

[E04] 查找子串位置
来源：http://cou.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://uqi.birdmap.top

PHP:  strpos($s, "x");
来源：http://fgu.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mdx.yangfankeji.com

TS:   s.indexOf("x")
来源：http://ghv.hnqzz.top

Java: s.indexOf("x")
来源：http://exh.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://lsx.jinqigufen.top

Ruby: s.index("x")
来源：http://ejj.fzhhl.top

C#:   s.IndexOf("x")
来源：http://xwh.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qjj.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yyu.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lws.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://poh.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rxu.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dya.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hup.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rmh.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qyb.shangyingyoupin.top

[E06] 替换子串
来源：http://jog.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bon.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://hkm.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uca.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ndv.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agb.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://adh.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mdn.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://iqw.chenlongwang.top

[E07] 按分隔符拆分
来源：http://wjx.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvj.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ofb.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.ybcxt.top

TS:   s.split(",")
来源：http://odi.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xmn.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hvm.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://eao.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xas.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://wdx.smart0.xyz

Py:   ",".join(items)
来源：http://pbc.ydzc1.top

PHP:  implode(",", $items);
来源：http://vky.yvedp.cn

JS:   items.join(",")
来源：http://evn.xylfe.cn

TS:   items.join(",")
来源：http://eav.sysykeji.top

Java: String.join(",", items)
来源：http://ave.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://raj.epnwcf.com

Ruby: items.join(",")
来源：http://nev.svipenyu.cn

C#:   string.Join(",", items)
来源：http://gzq.cashguo.top

[E09] 去除所有空白字符
来源：http://ozr.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://png.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nph.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://anw.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://dby.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://wsi.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yhe.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://neo.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rfr.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://unb.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrw.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vuo.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://bta.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://ohx.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://plv.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rbo.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xzi.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lvb.guowangkeji.top

[E11] 反转字符串
来源：http://scu.yj202588.top

Py:   s[::-1]
来源：http://lpd.dianchejie.cn

PHP:  strrev($s);
来源：http://iuw.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://xwi.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://vpv.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sqv.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lim.tian-w.cn

Ruby: s.reverse
来源：http://mja.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zrd.yfazqb.com

[E12] 统计某字符出现次数
来源：http://wox.ydzc1.top

Py:   s.count("a")
来源：http://bbp.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://lxg.smart0.xyz

JS:   s.split("a").length - 1
来源：http://pzv.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://orz.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hxy.316326.xyz

Go:   strings.Count(s, "a")
来源：http://iei.wangdashe.top

Ruby: s.count("a")
来源：http://kri.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://pin.shzxlz.cn

[E13] 逐字符遍历
来源：http://bqu.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://sco.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wrh.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fmy.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yga.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sky.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zdu.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lvb.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tsg.andypj.xyz

[E14] URL 编码与 Base64
来源：http://ngn.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jfe.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ijr.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jwu.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kzz.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wza.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gtx.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ogx.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lyr.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://off.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gvt.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iti.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rwu.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hnp.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bjt.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://znr.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ucb.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://six.wangdashe.top

[E16] 数字千分位
来源：http://ovh.uphjek.com

Py:   f"{1234567:,}"
来源：http://hea.birdmap.top

PHP:  number_format(1234567);
来源：http://fst.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kma.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gqs.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sot.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ege.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://huq.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://vkn.feifeiyinyue.top

[E17] 首字母大写
来源：http://pxi.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fdt.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ywa.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://udr.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzj.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vtu.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fhz.hnqzz.top

Ruby: s.capitalize
来源：http://fle.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hjx.c1oappe.top

[E18] 模板占位符替换
来源：http://fib.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wqf.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vvn.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://eaw.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://vlf.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pxb.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hod.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qmf.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rbg.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://esk.bbcook.cn

Py:   s.splitlines()
来源：http://pwp.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ylj.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://whc.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://zhg.ehwqpu.com

Java: s.lines().toList()
来源：http://tio.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://iyj.chenlongwang.top

Ruby: s.lines
来源：http://lij.jinqigufen.top

C#:   s.Split('\n')
来源：http://drz.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://tdx.hcnkem.com

Py:   if not s:
来源：http://klp.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rqc.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ufd.xinyue.icu

TS:   if (s === "") {}
来源：http://ttg.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://gcr.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://bkr.fehbvm.com

Ruby: if s.empty?
来源：http://poy.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vxj.gzhubu.top

[E21] 超长截断加省略号
来源：http://duo.cdnleiting.top


<!-- 参考信息 -->