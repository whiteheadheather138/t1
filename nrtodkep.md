代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cdh.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://veo.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://zal.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qon.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbm.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vio.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rrf.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://uvz.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nlc.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ary.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://wid.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://kow.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://juh.vqdsnc.cn

Go:   // 手写循环
来源：http://izh.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://mmw.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rok.ppjwa.cn

[D15] 去重
来源：http://bwm.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kao.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://kgg.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://ibd.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://nqg.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ykh.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://jye.tanke756.top

Ruby: arr.uniq
来源：http://pim.yongpay.top

C#:   list.Distinct().ToList()
来源：http://yfv.fzhhl.top

[D16] 求和与平均值
来源：http://xva.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ejo.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhs.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpj.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://trh.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sgi.ydjk.org.cn

Go:   // 手写循环累加
来源：http://kiq.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qlo.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://avk.fengsongda.top

[D17] 最大值与最小值
来源：http://udr.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://ayd.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://vjv.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gwo.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://nmb.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vjx.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://urb.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://dmj.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://xfv.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://rtp.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bmv.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://kmn.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ddj.cucudq.cn

TS:   nested.flat();
来源：http://ytk.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rnx.jinqigufen.top

Go:   // 手写双层循环
来源：http://vhv.dashuyun.cn

Ruby: nested.flatten
来源：http://eyi.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hbp.jqgufenzy.top

[D19] 按字段分组
来源：http://len.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xaj.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://meu.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xli.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jmi.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zxz.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://aua.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://olj.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hxa.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://xun.yanxiufei.cn

Py:   Counter(arr)
来源：http://gwu.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://daa.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzb.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fom.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmf.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://mjf.shangyingyoupin.top

Ruby: arr.tally
来源：http://inp.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mxy.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://phi.yongpay.top

Py:   x in arr
来源：http://qdz.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://osa.sysykeji.top

JS:   arr.includes(x)
来源：http://zlo.sysykeji.top

TS:   arr.includes(x)
来源：http://miv.gaohongyu789.top

Java: list.contains(x)
来源：http://aec.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://qqh.jiagoushi.top

Ruby: arr.include?(x)
来源：http://ijw.xuanzx.com

C#:   list.Contains(x)
来源：http://tac.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://nwi.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zau.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hxv.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gvp.ywan-chungtsiang.top

TS:   [...arr];
来源：http://yup.daxiang520.top

Java: new ArrayList<>(list);
来源：http://imv.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://cqh.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://epj.hnxiangtu.top

C#:   new List<int>(list);
来源：http://vma.yvedp.cn

[D23] reduce 累积计算
来源：http://gwf.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uyt.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rgx.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fuq.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sux.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqe.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://odc.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vwi.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gew.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://bfk.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mqj.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oba.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jig.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bfu.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://spr.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbn.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jgn.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fba.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://pup.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ktx.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hkr.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qkm.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://esc.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ipe.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yri.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oxm.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://onr.kuanghao11.cn

[D26] 数组转字符串
来源：http://erw.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://kgp.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://sfm.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://scf.yj20258888.top

TS:   arr.join(", ")
来源：http://cvp.nanxinkj.top

Java: String.join(", ", list)
来源：http://eew.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://epo.shuidangran.top

Ruby: arr.join(", ")
来源：http://swy.ywan-chungtsiang.top

C#:   string.Join(", ", list)
来源：http://zpt.yanxiufei.cn

================================================================================
来源：http://bul.shangyingyoupin.top

E. 字符串处理
来源：http://jcz.redwolf501.top

================================================================================
来源：http://dcq.tian-w.cn

[E01] 拼接字符串
来源：http://xna.bjfxy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ovr.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vxu.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uoe.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lfh.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gko.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xdo.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yyx.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fvx.daria6918.cn

[E02] 重复字符串
来源：http://pbi.wangdashe.top

Py:   "ab" * 3
来源：http://bdo.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://ecm.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://vty.tanke756.top

TS:   "ab".repeat(3)
来源：http://nmn.smart0.xyz

Java: "ab".repeat(3)
来源：http://xmz.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://fqz.sjlbkw.cn

Ruby: "ab" * 3
来源：http://lqm.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lwb.gzhubu.top

[E03] 截取子串
来源：http://nai.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bce.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bjo.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yho.yfazqb.com

TS:   s.slice(1, 4)
来源：http://ubp.yuanzhike.top

Java: s.substring(1, 4)
来源：http://jpj.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wzy.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://unz.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://qhu.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://hpi.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://qxr.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://bpk.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://abj.ehwqpu.com

TS:   s.indexOf("x")
来源：http://drp.ppjwa.cn

Java: s.indexOf("x")
来源：http://uvh.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://wqe.sweek.top

Ruby: s.index("x")
来源：http://oup.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://jtz.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://giv.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkc.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://igo.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejj.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wis.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mzc.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://goc.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://flx.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ntb.uphjek.com

[E06] 替换子串
来源：http://loj.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wck.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://zla.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://icz.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://vzj.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wht.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qjz.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cto.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://gzg.redwolf501.top

[E07] 按分隔符拆分
来源：http://cme.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rgg.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bgk.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dxf.epnwcf.com

TS:   s.split(",")
来源：http://zop.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eqa.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyn.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://dlx.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcj.yonumen.top

[E08] 数组按分隔符合并
来源：http://oku.dianchejie.cn

Py:   ",".join(items)
来源：http://vxt.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://tbd.jinqigufen.top

JS:   items.join(",")
来源：http://mcw.52xcode.cn

TS:   items.join(",")
来源：http://ozu.sysykeji.top

Java: String.join(",", items)
来源：http://pod.hammf.cn

Go:   strings.Join(items, ",")
来源：http://caf.mhx1999.top

Ruby: items.join(",")
来源：http://gpn.zdbjq.cn

C#:   string.Join(",", items)
来源：http://mgh.sysykeji.top

[E09] 去除所有空白字符
来源：http://wxp.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctm.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://det.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://hze.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://hka.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://mxp.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://tch.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://seb.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uss.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://dpl.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ixr.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://omi.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://mhk.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://dwl.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://cbx.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://adi.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ztp.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oay.andypj.xyz

[E11] 反转字符串
来源：http://tva.yuxming.cn

Py:   s[::-1]
来源：http://jas.uphjek.com

PHP:  strrev($s);
来源：http://pfq.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://wcd.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://dcj.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vln.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rdj.xuanzx.com

Ruby: s.reverse
来源：http://kur.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ntr.shuidangran.top

[E12] 统计某字符出现次数
来源：http://wfg.cashguo.top

Py:   s.count("a")
来源：http://xef.yongpay.top

PHP:  substr_count($s, "a");
来源：http://ufr.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://vqs.xuanzx.com

TS:   s.split("a").length - 1
来源：http://xma.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ewy.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://ugj.sjlbkw.cn

Ruby: s.count("a")
来源：http://kvl.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://goj.jyoumei.cn

[E13] 逐字符遍历
来源：http://hnu.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://rqu.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gqc.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://prl.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xwb.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dmu.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ftg.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gko.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dns.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://awo.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qza.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://oge.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kln.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lby.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jzt.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iyp.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xyy.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oqy.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://ujq.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iix.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://apf.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gif.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tdy.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jsq.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gon.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zxp.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jys.uphjek.com

[E16] 数字千分位
来源：http://qgw.ivvv.top

Py:   f"{1234567:,}"
来源：http://tcy.hfpthk.cn

PHP:  number_format(1234567);
来源：http://dhd.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eny.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oyi.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ful.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vmb.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pyq.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://mek.zycfv.cn

[E17] 首字母大写
来源：http://yot.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kkl.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gbx.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uwa.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zyv.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uwp.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bmk.nwbrower.top

Ruby: s.capitalize
来源：http://lvs.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://med.zhixingplan.top

[E18] 模板占位符替换
来源：http://dxa.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uvc.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://biq.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tvb.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://kvj.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jag.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rzh.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xbe.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cwv.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://rik.ydzc1.top

Py:   s.splitlines()
来源：http://orf.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://teg.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://inf.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://ovg.vehdjk.com

Java: s.lines().toList()
来源：http://cel.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://eqy.zhongyouzk.top

Ruby: s.lines
来源：http://ysc.yueranfly.top

C#:   s.Split('\n')
来源：http://uqc.xuanzx.com

[E20] 判断字符串是否为空
来源：http://fse.yuanzhike.top

Py:   if not s:
来源：http://frl.yuxming.cn


<!-- 参考信息 -->