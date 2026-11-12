代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://its.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qwj.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://xtz.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://cbc.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://irx.chenlongwang.top

Go:   // 手写循环
来源：http://gew.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://phz.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bjn.guowangkeji.top

[D15] 去重
来源：http://taf.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qwh.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://zxf.redwolf501.top

JS:   [...new Set(arr)]
来源：http://ewc.xuanzx.com

TS:   [...new Set(arr)]
来源：http://tvk.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gvb.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ocs.aibaodan.cn

Ruby: arr.uniq
来源：http://ylo.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://trl.jyoumei.cn

[D16] 求和与平均值
来源：http://jct.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rff.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://acp.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ken.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyr.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://msf.jiagoushi.top

Go:   // 手写循环累加
来源：http://atu.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vcp.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://pnt.c1oappe.top

[D17] 最大值与最小值
来源：http://coo.yj202588.top

Py:   max(arr);  min(arr)
来源：http://eiw.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://nqs.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://spd.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://hgs.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kab.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tfg.ivvv.top

Ruby: arr.max;  arr.min
来源：http://kpc.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://vxe.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://uik.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sis.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://blz.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gch.ppjwa.cn

TS:   nested.flat();
来源：http://jfo.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dmf.daria6918.cn

Go:   // 手写双层循环
来源：http://euf.c1oappe.top

Ruby: nested.flatten
来源：http://fad.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dfj.ydjk.org.cn

[D19] 按字段分组
来源：http://xvw.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rqh.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wmy.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jeo.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yxv.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iea.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://hkr.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vvu.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tvm.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://xck.uphjek.com

Py:   Counter(arr)
来源：http://vdx.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://mmv.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kgu.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://utd.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uod.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://cgl.yfazqb.com

Ruby: arr.tally
来源：http://apt.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzw.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://cci.ctjpmb.com

Py:   x in arr
来源：http://iam.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://wdd.ppjwa.cn

JS:   arr.includes(x)
来源：http://iby.guannengcc.top

TS:   arr.includes(x)
来源：http://zxo.yuxming.cn

Java: list.contains(x)
来源：http://htl.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://tne.fktsv.cn

Ruby: arr.include?(x)
来源：http://bro.c1oappe.top

C#:   list.Contains(x)
来源：http://btg.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://cye.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vhw.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rcz.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ali.ivvv.top

TS:   [...arr];
来源：http://tuc.jianghu66.top

Java: new ArrayList<>(list);
来源：http://mob.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uqd.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://nvi.yanxiufei.cn

C#:   new List<int>(list);
来源：http://ihf.yj20258888.top

[D23] reduce 累积计算
来源：http://kyy.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jra.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yss.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kcs.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qeo.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bqf.andypj.xyz

Go:   // 手写循环
来源：http://yal.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mxp.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tcr.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://usu.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qtc.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://quk.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kly.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hdd.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fkc.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hzw.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://igr.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jge.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://grl.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rsx.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tih.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hvo.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://khl.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gad.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qwo.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tmg.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lvy.zhengqikj.top

[D26] 数组转字符串
来源：http://ibk.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://qfp.cashguo.top

PHP:  implode(", ", $arr);
来源：http://fov.fengsongda.top

JS:   arr.join(", ")
来源：http://bgb.mhx1999.top

TS:   arr.join(", ")
来源：http://wlk.jinqigufen.top

Java: String.join(", ", list)
来源：http://fpb.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://bkq.hesvh.cn

Ruby: arr.join(", ")
来源：http://vvy.cashguo.top

C#:   string.Join(", ", list)
来源：http://hat.c1oappe.top

================================================================================
来源：http://wni.shanyushiyangtech.top

E. 字符串处理
来源：http://hcs.feifeiyinyue.top

================================================================================
来源：http://iiq.redwolf501.top

[E01] 拼接字符串
来源：http://ddf.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eew.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lpg.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsj.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://opu.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://reu.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lnm.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uif.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mxs.meibo888.top

[E02] 重复字符串
来源：http://dco.aibaodan.cn

Py:   "ab" * 3
来源：http://nqp.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://ynz.iojbl.cn

JS:   "ab".repeat(3)
来源：http://beq.wangdashe.top

TS:   "ab".repeat(3)
来源：http://hbo.redwolf501.top

Java: "ab".repeat(3)
来源：http://qyp.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://rdg.sysykeji.top

Ruby: "ab" * 3
来源：http://lkd.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pae.yj20258888.top

[E03] 截取子串
来源：http://nih.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rhs.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bcf.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lum.bjfxy.top

TS:   s.slice(1, 4)
来源：http://paw.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://oyc.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cck.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://hee.tarul.cn

C#:   s.Substring(1, 3)
来源：http://ver.jinqigfzy.top

[E04] 查找子串位置
来源：http://auc.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://zeb.cheryme.top

PHP:  strpos($s, "x");
来源：http://fhp.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://emc.fzhhl.top

TS:   s.indexOf("x")
来源：http://omu.xinyue.icu

Java: s.indexOf("x")
来源：http://ehk.yongpay.top

Go:   strings.Index(s, "x")
来源：http://aco.yongpay.top

Ruby: s.index("x")
来源：http://fxl.ivvv.top

C#:   s.IndexOf("x")
来源：http://pee.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zju.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nsx.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mla.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lup.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mtq.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqd.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nlt.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uvk.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://del.ybcxt.top

[E06] 替换子串
来源：http://usv.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://juo.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://thm.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dgm.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://wdq.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mpn.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xrl.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sqz.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://dto.yvedp.cn

[E07] 按分隔符拆分
来源：http://sra.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cqf.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lrq.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nkz.andypj.xyz

TS:   s.split(",")
来源：http://zhl.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://cfj.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mou.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://aab.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zqb.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://sca.zdbjq.cn

Py:   ",".join(items)
来源：http://gdr.aizwys.cn

PHP:  implode(",", $items);
来源：http://lmt.zhixingplan.top

JS:   items.join(",")
来源：http://tqe.0kj1m.cn

TS:   items.join(",")
来源：http://pjp.snrcjt.cn

Java: String.join(",", items)
来源：http://rqq.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://iwy.c1oappe.top

Ruby: items.join(",")
来源：http://udf.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://tve.uphjek.com

[E09] 去除所有空白字符
来源：http://gmn.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sii.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://azk.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://xfu.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://map.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://zhu.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ksu.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://gci.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://avu.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://lqq.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nqv.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tbc.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://mov.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://niv.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://ruc.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yxs.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gyb.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wwg.jiagoushi.top

[E11] 反转字符串
来源：http://udj.c1oappe.top

Py:   s[::-1]
来源：http://lkm.yonumen.top

PHP:  strrev($s);
来源：http://wui.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://iiz.xuanzx.com

TS:   [...s].reverse().join("")
来源：http://lhx.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://akd.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://npd.hcnkem.com

Ruby: s.reverse
来源：http://idl.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://ewy.mhx1999.top

[E12] 统计某字符出现次数
来源：http://vnu.hcnkem.com

Py:   s.count("a")
来源：http://gvv.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://cpj.shuidangran.top

JS:   s.split("a").length - 1
来源：http://okl.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://crp.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kcp.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://gfx.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://syb.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://guy.birdmap.top

[E13] 逐字符遍历
来源：http://vox.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://dwe.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wgk.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fsk.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://niy.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gqk.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bxs.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://url.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gpw.bjfxy.top

[E14] URL 编码与 Base64
来源：http://haa.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://urk.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pvv.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kky.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xrl.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bxb.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://exi.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fmb.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ger.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://jvo.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://avi.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tew.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mrn.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kry.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ham.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cuk.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xmr.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wns.sufxvd.cn

[E16] 数字千分位
来源：http://uqr.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://yjv.cheryme.top

PHP:  number_format(1234567);
来源：http://yna.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dri.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xpu.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xju.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nei.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zve.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://xff.shanyushiyangtech.top

[E17] 首字母大写
来源：http://pcy.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lxd.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fna.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mws.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xno.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://api.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qod.yanxiufei.cn

Ruby: s.capitalize
来源：http://del.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://orl.tian-w.cn

[E18] 模板占位符替换
来源：http://lfy.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://okm.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yrp.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vsb.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://owt.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lqc.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gxb.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vlz.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrn.daria6918.cn

[E19] 多行文本按行拆分
来源：http://roe.nanxinkj.top

Py:   s.splitlines()
来源：http://hup.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjk.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://qay.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://ryr.redwolf501.top

Java: s.lines().toList()
来源：http://oyk.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://ztd.hnxiangtu.top

Ruby: s.lines
来源：http://yca.andypj.xyz

C#:   s.Split('\n')
来源：http://qjb.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://fwu.sweek.top

Py:   if not s:
来源：http://izp.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jhp.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bsh.epnwcf.com

TS:   if (s === "") {}
来源：http://bdr.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://fyi.hammf.cn

Go:   if s == "" {}
来源：http://kue.hysaishi.cn

Ruby: if s.empty?
来源：http://tgf.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tvz.gotoacloud.top

[E21] 超长截断加省略号
来源：http://zgu.tanke756.top


<!-- 参考信息 -->