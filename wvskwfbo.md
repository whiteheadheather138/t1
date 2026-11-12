代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogq.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uwv.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://qyo.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://ncw.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fyj.chenlongwang.top

Go:   // 手写循环
来源：http://qus.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://gbv.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tqe.xziqi.cn

[D15] 去重
来源：http://shf.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vev.gogol.net.cn

PHP:  array_unique($arr);
来源：http://slo.redwolf501.top

JS:   [...new Set(arr)]
来源：http://tfc.iojbl.cn

TS:   [...new Set(arr)]
来源：http://pav.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uqz.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://xao.hnxiangtu.top

Ruby: arr.uniq
来源：http://zxt.yj202588.top

C#:   list.Distinct().ToList()
来源：http://bxo.xinyue.icu

[D16] 求和与平均值
来源：http://odm.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oey.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jhx.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nmu.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zoq.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ahg.nanxuanxn.top

Go:   // 手写循环累加
来源：http://stf.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dsg.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://qdj.epnwcf.com

[D17] 最大值与最小值
来源：http://hfo.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://pnz.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://uci.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lyh.yonumen.top

TS:   Math.max(...arr);
来源：http://ifl.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fan.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kbm.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://xab.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://auu.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://dem.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://csh.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://tia.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ysr.sjlbkw.cn

TS:   nested.flat();
来源：http://zqs.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wjm.havefunace.top

Go:   // 手写双层循环
来源：http://rbm.ehwqpu.com

Ruby: nested.flatten
来源：http://zfo.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yyn.pycfn.com

[D19] 按字段分组
来源：http://fle.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uwp.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hyi.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jnq.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lnj.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://par.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://kxo.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://goi.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tdl.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://pab.tarul.cn

Py:   Counter(arr)
来源：http://pma.zycfv.cn

PHP:  array_count_values($arr);
来源：http://uen.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cjs.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywr.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jnk.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://iht.jinqigufen.top

Ruby: arr.tally
来源：http://pjm.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sbe.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://xhp.shzxlz.cn

Py:   x in arr
来源：http://rde.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://zda.aizwys.cn

JS:   arr.includes(x)
来源：http://xmf.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://qos.shanyushiyangtech.top

Java: list.contains(x)
来源：http://xjm.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://grc.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://kwc.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://jqk.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://xor.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kkd.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vnt.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wih.fehbvm.com

TS:   [...arr];
来源：http://sej.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://jiz.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://pyl.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://fpo.0kj1m.cn

C#:   new List<int>(list);
来源：http://ekr.cucudq.cn

[D23] reduce 累积计算
来源：http://tnu.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mdy.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://res.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kob.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rdk.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wtc.vehdjk.com

Go:   // 手写循环
来源：http://blr.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://skm.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iix.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://ixg.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lms.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hki.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://odx.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mdt.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bgt.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgi.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bii.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cxm.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://qhp.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyb.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dtl.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://can.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zdz.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://juf.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://als.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iad.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dey.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://vhi.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://pfs.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://sga.dianchejie.cn

JS:   arr.join(", ")
来源：http://zhv.ppjwa.cn

TS:   arr.join(", ")
来源：http://xax.jqgfzy.top

Java: String.join(", ", list)
来源：http://tfr.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://qkb.yj202588.top

Ruby: arr.join(", ")
来源：http://bbg.yonumen.top

C#:   string.Join(", ", list)
来源：http://fco.jiagoushi.top

================================================================================
来源：http://ikh.nanxinkj.top

E. 字符串处理
来源：http://ofb.ydjk.org.cn

================================================================================
来源：http://hnp.kuanghao11.cn

[E01] 拼接字符串
来源：http://nli.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xsl.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tfr.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ysa.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bvk.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kav.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mri.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nxr.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gfm.hnxiangtu.top

[E02] 重复字符串
来源：http://znm.hesvh.cn

Py:   "ab" * 3
来源：http://qgk.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://jnu.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://til.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://wif.wangdashe.top

Java: "ab".repeat(3)
来源：http://tfr.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://pkc.gogol.net.cn

Ruby: "ab" * 3
来源：http://spq.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fao.cdnleiting.top

[E03] 截取子串
来源：http://aen.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gha.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwv.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kgn.ivvv.top

TS:   s.slice(1, 4)
来源：http://uky.cashguo.top

Java: s.substring(1, 4)
来源：http://evr.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://omq.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ecb.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://vrh.tianlin.xyz

[E04] 查找子串位置
来源：http://ivl.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://fwt.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://dzp.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sud.yuanzhike.top

TS:   s.indexOf("x")
来源：http://hec.vqdsnc.cn

Java: s.indexOf("x")
来源：http://ujl.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://ucj.uphjek.com

Ruby: s.index("x")
来源：http://hfu.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://wie.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pjd.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yzo.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jxt.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akn.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bbo.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hqf.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wxn.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gau.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cbf.fehbvm.com

[E06] 替换子串
来源：http://ynu.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lar.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://zrw.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxy.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://jvv.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dlv.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vqw.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jde.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://qnd.gotoacloud.top

[E07] 按分隔符拆分
来源：http://dge.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://reg.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vjf.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xan.feifeiyinyue.top

TS:   s.split(",")
来源：http://dxz.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://bvk.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://edl.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://hdp.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oat.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://btg.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://rvj.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://gvv.tanke756.top

JS:   items.join(",")
来源：http://hma.gzhubu.top

TS:   items.join(",")
来源：http://gop.quarkkingdee.top

Java: String.join(",", items)
来源：http://qlo.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://ldl.haohaochexian.top

Ruby: items.join(",")
来源：http://ypl.nwbrower.top

C#:   string.Join(",", items)
来源：http://qje.snrcjt.cn

[E09] 去除所有空白字符
来源：http://avi.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nbl.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lwc.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://mlx.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://him.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://tux.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vnh.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ubl.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyx.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://sxs.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ork.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xew.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://ban.yanxiufei.cn

TS:   "7".padStart(3, "0")
来源：http://tyi.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://afb.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wyb.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ckc.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gkz.xinyue.icu

[E11] 反转字符串
来源：http://bhk.fanxiaobao.xyz

Py:   s[::-1]
来源：http://mgh.hnxiangtu.top

PHP:  strrev($s);
来源：http://zae.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://uks.ivvv.top

TS:   [...s].reverse().join("")
来源：http://snn.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://zbz.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cuq.xuanzx.com

Ruby: s.reverse
来源：http://xcl.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://luo.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://qsv.shuidangran.top

Py:   s.count("a")
来源：http://uqd.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://ymh.meibo888.top

JS:   s.split("a").length - 1
来源：http://ytw.yvedp.cn

TS:   s.split("a").length - 1
来源：http://jhv.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kzu.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://qwq.meibo888.top

Ruby: s.count("a")
来源：http://wln.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://nns.jinqigufen.top

[E13] 逐字符遍历
来源：http://tfj.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://aqy.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fyl.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nrj.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fuv.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zkm.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vhb.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nrm.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ndh.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://qoz.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lmi.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pti.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://adb.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dql.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gfy.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jhe.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dfj.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eix.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://apc.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gpi.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aoz.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tac.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eqs.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqw.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tua.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xxb.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xpu.ivvv.top

[E16] 数字千分位
来源：http://ccq.vehdjk.com

Py:   f"{1234567:,}"
来源：http://ydp.sufxvd.cn

PHP:  number_format(1234567);
来源：http://jnp.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://crm.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vgf.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eee.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hko.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iyc.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://mrs.vehdjk.com

[E17] 首字母大写
来源：http://jnz.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iao.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xea.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jow.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oca.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yvc.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nih.316326.xyz

Ruby: s.capitalize
来源：http://zaq.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nxi.vehdjk.com

[E18] 模板占位符替换
来源：http://yyz.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nfc.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://krp.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zuv.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zku.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gia.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vke.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ggc.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://swc.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://dcf.zdqjudy.top

Py:   s.splitlines()
来源：http://oeh.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eip.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://kyi.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://hiu.jinqigfzy.top

Java: s.lines().toList()
来源：http://eml.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://agx.zhongyouzk.top

Ruby: s.lines
来源：http://dlp.chenlongwang.top

C#:   s.Split('\n')
来源：http://hyq.yvedp.cn

[E20] 判断字符串是否为空
来源：http://xkw.zhoulong.xyz

Py:   if not s:
来源：http://vxw.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ijx.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hnk.jinqigfzy.top

TS:   if (s === "") {}
来源：http://kzj.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://lpv.andypj.xyz

Go:   if s == "" {}
来源：http://uec.hammf.cn

Ruby: if s.empty?
来源：http://bty.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ysn.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://vgs.guannengcc.top


<!-- 参考信息 -->