代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wct.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://rux.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://pey.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ezl.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wwc.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://vle.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wkf.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://ruz.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hwr.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mzi.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://atu.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://ech.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jds.yuanzhike.top

Go:   // 手写循环
来源：http://hph.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://uku.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kki.havefunace.top

[D15] 去重
来源：http://fxa.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dug.cheryme.top

PHP:  array_unique($arr);
来源：http://qkh.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://erc.52xcode.cn

TS:   [...new Set(arr)]
来源：http://lap.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wth.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://orj.dianchejie.cn

Ruby: arr.uniq
来源：http://xki.yonumen.top

C#:   list.Distinct().ToList()
来源：http://jsr.gaohongyu789.top

[D16] 求和与平均值
来源：http://dfd.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://whw.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fmj.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zov.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dxq.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lbo.cucudq.cn

Go:   // 手写循环累加
来源：http://gee.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oki.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://efh.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://afe.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://vph.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://slj.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pzf.shuidangran.top

TS:   Math.max(...arr);
来源：http://bfo.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rhy.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wyq.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://eux.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://jfb.cheryme.top

[D18] 扁平化嵌套数组
来源：http://kpb.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aex.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://ffy.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mro.sjlbkw.cn

TS:   nested.flat();
来源：http://xrn.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uhz.jlsjyb.cn

Go:   // 手写双层循环
来源：http://rvz.hnxiangtu.top

Ruby: nested.flatten
来源：http://jhg.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ido.daxiang520.top

[D19] 按字段分组
来源：http://ltj.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vqb.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fbu.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zki.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mlp.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uxi.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://iep.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdm.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dhs.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://yes.316326.xyz

Py:   Counter(arr)
来源：http://ybz.tian-w.cn

PHP:  array_count_values($arr);
来源：http://mgl.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ops.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lln.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oux.ivvv.top

Go:   // 手写 map[T]int
来源：http://erg.guannengcc.top

Ruby: arr.tally
来源：http://ylu.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aim.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://vbx.zdbjq.cn

Py:   x in arr
来源：http://tyh.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://egp.xuanzx.com

JS:   arr.includes(x)
来源：http://yun.hesvh.cn

TS:   arr.includes(x)
来源：http://rfv.aibaodan.cn

Java: list.contains(x)
来源：http://vvv.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://wdl.yj20258888.top

Ruby: arr.include?(x)
来源：http://nkg.aibaodan.cn

C#:   list.Contains(x)
来源：http://cby.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://hbn.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xhb.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://thx.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://quv.zhiwuduotai.top

TS:   [...arr];
来源：http://lcr.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://nnp.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uvh.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://kgk.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://gwo.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://dhz.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://drr.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pcc.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dta.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zvp.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://euc.yongpay.top

Go:   // 手写循环
来源：http://lkf.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fnb.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lcw.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://icl.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfj.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vem.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vjm.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://voe.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yvn.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://krx.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wwd.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkz.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://stn.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://min.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nrb.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lyr.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bgz.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xqi.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://knc.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zev.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://doo.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://njf.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://uqw.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://inn.yonumen.top

JS:   arr.join(", ")
来源：http://tcp.smart0.xyz

TS:   arr.join(", ")
来源：http://cnq.yj202588.top

Java: String.join(", ", list)
来源：http://exs.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://ofq.nwbrower.top

Ruby: arr.join(", ")
来源：http://ich.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://huu.xuanzx.com

================================================================================
来源：http://gjy.vehdjk.com

E. 字符串处理
来源：http://nbi.birdmap.top

================================================================================
来源：http://gyx.jiagoushi.top

[E01] 拼接字符串
来源：http://wes.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yzj.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kxs.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kfj.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nws.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xts.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dnm.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hxv.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hda.fengsongda.top

[E02] 重复字符串
来源：http://fnp.nanxinkj.top

Py:   "ab" * 3
来源：http://taq.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://ngg.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://kvk.zycfv.cn

TS:   "ab".repeat(3)
来源：http://lja.52xcode.cn

Java: "ab".repeat(3)
来源：http://lym.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://zqr.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://eus.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cpf.yangfankeji.com

[E03] 截取子串
来源：http://mhf.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://esu.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://she.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sqa.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://ghv.yonumen.top

Java: s.substring(1, 4)
来源：http://iav.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nvm.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://vnt.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://pjx.tanke756.top

[E04] 查找子串位置
来源：http://uqq.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://woz.sweek.top

PHP:  strpos($s, "x");
来源：http://ofm.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jox.dashuyun.cn

TS:   s.indexOf("x")
来源：http://jwj.redwolf501.top

Java: s.indexOf("x")
来源：http://jro.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://rtp.nanxinkj.top

Ruby: s.index("x")
来源：http://hxt.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ykr.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://efz.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ght.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uco.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvy.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yzg.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kli.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pph.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vop.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://woo.ehwqpu.com

[E06] 替换子串
来源：http://ztt.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://opl.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://crn.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lgq.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://reo.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nns.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgb.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qgt.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://omi.zhixingplan.top

[E07] 按分隔符拆分
来源：http://qnl.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dhg.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dtj.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zxj.guannengcc.top

TS:   s.split(",")
来源：http://way.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://wzp.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xbg.cheryme.top

Ruby: s.split(",");  s.split
来源：http://wur.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jkl.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://srq.epnwcf.com

Py:   ",".join(items)
来源：http://iir.chenlongwang.top

PHP:  implode(",", $items);
来源：http://hrr.ppjwa.cn

JS:   items.join(",")
来源：http://qpi.jqgufenzy.top

TS:   items.join(",")
来源：http://qhu.cqqwz.cn

Java: String.join(",", items)
来源：http://hgq.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://sdh.guowangkeji.top

Ruby: items.join(",")
来源：http://oxc.yvedp.cn

C#:   string.Join(",", items)
来源：http://zlq.52xcode.cn

[E09] 去除所有空白字符
来源：http://ftz.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hhx.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ygw.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://gik.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://unv.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://fje.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dtu.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://ufp.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aro.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://dps.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eya.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pwi.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://jfs.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://zkw.sweek.top

Java: String.format("%03d", 7)
来源：http://wco.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hwm.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yiv.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fae.shzxlz.cn

[E11] 反转字符串
来源：http://ynp.chenlongwang.top

Py:   s[::-1]
来源：http://lnm.jlsjyb.cn

PHP:  strrev($s);
来源：http://tfj.yj20258.top

JS:   [...s].reverse().join("")
来源：http://auj.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://aww.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xlv.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nkf.ivvv.top

Ruby: s.reverse
来源：http://tvl.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://gzm.guannengcc.top

[E12] 统计某字符出现次数
来源：http://vai.jyoumei.cn

Py:   s.count("a")
来源：http://pmm.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://zlj.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://zvn.ivvv.top

TS:   s.split("a").length - 1
来源：http://lcp.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xkg.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://zox.gaohongyu789.top

Ruby: s.count("a")
来源：http://oye.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://afg.tanke756.top

[E13] 逐字符遍历
来源：http://dpm.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://nvl.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rjh.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oth.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gki.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tbj.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mmj.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://anu.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xao.yonumen.top

[E14] URL 编码与 Base64
来源：http://izu.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nun.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ywo.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eng.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xqe.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbu.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://twb.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbm.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://akb.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://tpm.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wfk.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jtp.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cxr.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tbl.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqu.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pmx.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xlc.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmt.andypj.xyz

[E16] 数字千分位
来源：http://yjp.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://vhy.sufxvd.cn

PHP:  number_format(1234567);
来源：http://cep.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ttb.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://whp.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lpt.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oql.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qyc.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://zlc.meibo888.top

[E17] 首字母大写
来源：http://fnr.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tqb.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rly.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://btj.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfs.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kuh.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zxu.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://jrf.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oxe.fehbvm.com

[E18] 模板占位符替换
来源：http://rfi.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wex.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzo.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kzr.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jvk.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fcz.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qma.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gvm.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qbc.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://nwy.hammf.cn

Py:   s.splitlines()
来源：http://guq.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rra.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://qff.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://bqx.hnxiangtu.top

Java: s.lines().toList()
来源：http://bsa.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://btj.shuidangran.top

Ruby: s.lines
来源：http://xar.xuanzx.com

C#:   s.Split('\n')
来源：http://rve.nwbrower.top

[E20] 判断字符串是否为空
来源：http://eyi.gogol.net.cn

Py:   if not s:
来源：http://pmv.sjlbkw.cn


<!-- 参考信息 -->