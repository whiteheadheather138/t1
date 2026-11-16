代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wre.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pua.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://rya.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://zax.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cos.zhoulong.xyz

Go:   // 手写循环
来源：http://env.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://yvu.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lel.svipenyu.cn

[D15] 去重
来源：http://prf.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cvw.cqqwz.cn

PHP:  array_unique($arr);
来源：http://fot.sxryk.cn

JS:   [...new Set(arr)]
来源：http://uyp.fehbvm.com

TS:   [...new Set(arr)]
来源：http://azw.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ksx.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hht.chenzaomai.com

Ruby: arr.uniq
来源：http://zic.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://jhl.snrcjt.cn

[D16] 求和与平均值
来源：http://mxv.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kvl.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ndz.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jwi.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://utu.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywx.jianghu66.top

Go:   // 手写循环累加
来源：http://ajq.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ekp.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://yrh.yanxiufei.cn

[D17] 最大值与最小值
来源：http://mli.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://xlu.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://afj.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://who.gotoacloud.top

TS:   Math.max(...arr);
来源：http://zdz.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zoi.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tup.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://xxd.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://suz.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://bpd.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wzy.tanke756.top

PHP:  array_merge(...$nested);
来源：http://xnu.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yoa.tianlin.xyz

TS:   nested.flat();
来源：http://caq.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://adv.hfpthk.cn

Go:   // 手写双层循环
来源：http://iiv.hfpthk.cn

Ruby: nested.flatten
来源：http://nsb.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vcv.chenlongwang.top

[D19] 按字段分组
来源：http://bav.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eyn.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddg.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vjg.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xxj.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mcy.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://bjf.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jmn.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://srh.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://prd.cqqwz.cn

Py:   Counter(arr)
来源：http://sew.52xcode.cn

PHP:  array_count_values($arr);
来源：http://dtt.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kex.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqb.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lpm.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://ewl.fzhhl.top

Ruby: arr.tally
来源：http://wgn.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ajm.redwolf501.top

[D21] 判断是否包含某元素
来源：http://aoa.yuanzhike.top

Py:   x in arr
来源：http://alu.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://dvv.cashguo.top

JS:   arr.includes(x)
来源：http://ump.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://nkc.gzhubu.top

Java: list.contains(x)
来源：http://occ.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://jgd.jinqigufen.top

Ruby: arr.include?(x)
来源：http://toy.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://cck.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://pnm.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qfq.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rob.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wdq.vehdjk.com

TS:   [...arr];
来源：http://ixu.wangdashe.top

Java: new ArrayList<>(list);
来源：http://cen.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://tsq.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://tpf.hywenlv.cn

C#:   new List<int>(list);
来源：http://dlw.fktsv.cn

[D23] reduce 累积计算
来源：http://xha.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eiw.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bvu.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hey.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lla.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vbt.hnqzz.top

Go:   // 手写循环
来源：http://zke.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fcy.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gbe.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://rdr.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqw.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kxx.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jpp.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://akt.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ehb.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kzh.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ico.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://utu.tarul.cn

[D25] Set 集合去重与交并差
来源：http://yqx.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://erh.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://loc.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://doy.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qvs.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uok.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rop.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://irf.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://soy.guowangkeji.top

[D26] 数组转字符串
来源：http://hhq.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://oyd.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://nyj.gotoacloud.top

JS:   arr.join(", ")
来源：http://voo.hysaishi.cn

TS:   arr.join(", ")
来源：http://obk.hywenlv.cn

Java: String.join(", ", list)
来源：http://ssc.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://tqk.yuanzhike.top

Ruby: arr.join(", ")
来源：http://zco.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://xrl.ydjk.org.cn

================================================================================
来源：http://yxk.jianghu66.top

E. 字符串处理
来源：http://vyf.aizwys.cn

================================================================================
来源：http://cue.nanxuanxn.top

[E01] 拼接字符串
来源：http://xjp.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://grm.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://puh.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hvn.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rvs.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nsy.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ksa.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gyn.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wwj.ybcxt.top

[E02] 重复字符串
来源：http://hqj.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://ywo.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://wyp.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://tjz.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://wjg.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://dfg.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://imf.hcnkem.com

Ruby: "ab" * 3
来源：http://peu.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rpq.yongpay.top

[E03] 截取子串
来源：http://ihg.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zbk.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bsq.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cqm.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://ocb.ctjpmb.com

Java: s.substring(1, 4)
来源：http://lzq.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lki.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://pma.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://jay.nwbrower.top

[E04] 查找子串位置
来源：http://fir.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://zue.yfazqb.com

PHP:  strpos($s, "x");
来源：http://dvn.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lgs.daxiang520.top

TS:   s.indexOf("x")
来源：http://bkh.yuxming.cn

Java: s.indexOf("x")
来源：http://fpc.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://oqx.daxiang520.top

Ruby: s.index("x")
来源：http://glx.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://jwt.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yjy.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xsn.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aka.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdq.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rjp.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvf.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wpx.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://llj.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sip.yuxming.cn

[E06] 替换子串
来源：http://zsn.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jnc.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://jeg.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://njk.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://fvd.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgp.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pom.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oxg.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://fnm.gzhubu.top

[E07] 按分隔符拆分
来源：http://mkm.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lrf.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zco.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kxv.yongpay.top

TS:   s.split(",")
来源：http://twx.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://gwe.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qov.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://lhv.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ofe.tarul.cn

[E08] 数组按分隔符合并
来源：http://rsr.wangshuangyany.cn

Py:   ",".join(items)
来源：http://qnl.yueranfly.top

PHP:  implode(",", $items);
来源：http://lmp.sufxvd.cn

JS:   items.join(",")
来源：http://geg.jianghu66.top

TS:   items.join(",")
来源：http://sbo.jyoumei.cn

Java: String.join(",", items)
来源：http://ova.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://erm.guowangkeji.top

Ruby: items.join(",")
来源：http://cnl.0kj1m.cn

C#:   string.Join(",", items)
来源：http://yxi.jyoumei.cn

[E09] 去除所有空白字符
来源：http://huu.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dpj.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ltd.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://spe.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://hoc.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://hvk.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vjy.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vwd.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqy.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://adw.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eah.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qse.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://aho.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://xvn.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://vei.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nzb.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cja.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://izt.sysykeji.top

[E11] 反转字符串
来源：http://jqr.bbcook.cn

Py:   s[::-1]
来源：http://pqs.dashuyun.cn

PHP:  strrev($s);
来源：http://uze.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://qmf.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://rpf.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ykt.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ezg.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://uuz.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://crn.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://xes.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://bdw.birdmap.top

PHP:  substr_count($s, "a");
来源：http://gjo.316326.xyz

JS:   s.split("a").length - 1
来源：http://vpw.fengsongda.top

TS:   s.split("a").length - 1
来源：http://dgy.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bmm.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://jcw.xuetiantiany.cn

Ruby: s.count("a")
来源：http://fzd.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://mtz.nanxinkj.top

[E13] 逐字符遍历
来源：http://icj.hcnkem.com

Py:   for ch in s: print(ch)
来源：http://tkj.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmd.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qkg.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://eir.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jvv.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tum.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fxj.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pij.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://pdo.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gzv.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gew.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://znc.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ail.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dth.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dyz.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://afd.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dhg.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://yji.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://cvp.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gav.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://chq.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xup.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://buw.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kom.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fgx.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nke.52xcode.cn

[E16] 数字千分位
来源：http://rug.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://tfx.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://fte.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wyl.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lzh.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bxi.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hnc.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ngt.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://xee.redwolf501.top

[E17] 首字母大写
来源：http://ntg.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nuq.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kcz.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kal.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sya.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jbk.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qwb.jqgufenzy.top

Ruby: s.capitalize
来源：http://cul.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mej.fehbvm.com

[E18] 模板占位符替换
来源：http://gez.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://taa.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbt.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oun.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jth.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://phf.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vai.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mif.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vvn.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://izh.jqgufenzy.top

Py:   s.splitlines()
来源：http://fjz.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vrv.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://yfk.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://pkb.bjfxy.top

Java: s.lines().toList()
来源：http://psv.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://vco.zhijiandao.cn

Ruby: s.lines
来源：http://edr.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://oga.smart0.xyz

[E20] 判断字符串是否为空
来源：http://ssz.zhengqikj.top

Py:   if not s:
来源：http://zci.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://atv.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fkc.yfazqb.com

TS:   if (s === "") {}
来源：http://maf.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://mrj.tanke756.top

Go:   if s == "" {}
来源：http://ryf.redwolf501.top

Ruby: if s.empty?
来源：http://tks.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qqr.hcnkem.com

[E21] 超长截断加省略号
来源：http://tjr.zhongyouzk.top


<!-- 参考信息 -->