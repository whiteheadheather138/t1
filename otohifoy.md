代发 wailian999

[D11] 反转数组
来源：http://cij.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yfr.ivvv.top

PHP:  array_reverse($arr);
来源：http://xpl.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvi.yfazqb.com

TS:   [...arr].reverse();
来源：http://cwk.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://vcx.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://oqp.nwbrower.top

Ruby: arr.reverse
来源：http://wmb.yj20258888.top

C#:   list.Reverse();
来源：http://wss.kuanghao11.cn

[D12] 查找元素下标
来源：http://tzr.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://nzk.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kcm.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qaq.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ign.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tiw.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://evo.zdqjudy.top

Ruby: arr.index(x)
来源：http://hla.fengsongda.top

C#:   list.IndexOf(x);
来源：http://efb.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://tmd.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wcj.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bts.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://dfq.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://ocv.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sez.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vby.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://ybg.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qew.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://cej.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lua.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://avj.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://vyq.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://pwz.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pts.yj20258888.top

Go:   // 手写循环
来源：http://bjg.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rhf.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bmt.jqgufenzy.top

[D15] 去重
来源：http://mgh.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zru.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://pzc.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://lbx.shuidangran.top

TS:   [...new Set(arr)]
来源：http://fge.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bcc.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://sqi.epnwcf.com

Ruby: arr.uniq
来源：http://mjy.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://ksl.cdnleiting.top

[D16] 求和与平均值
来源：http://sio.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lps.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vgs.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://etd.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://isr.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cba.tianlin.xyz

Go:   // 手写循环累加
来源：http://xts.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xzf.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://enq.0kj1m.cn

[D17] 最大值与最小值
来源：http://hrz.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://rid.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://kwd.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hbc.pycfn.com

TS:   Math.max(...arr);
来源：http://urd.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gkz.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xui.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://yxm.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://lpn.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://iaz.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cbu.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://flw.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zjw.guowangkeji.top

TS:   nested.flat();
来源：http://rfd.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzf.shuidangran.top

Go:   // 手写双层循环
来源：http://qtj.gaohongyu789.top

Ruby: nested.flatten
来源：http://xxp.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dwq.316326.xyz

[D19] 按字段分组
来源：http://ggs.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xwa.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kah.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wwe.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://upw.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pjp.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://uwr.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kjk.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zlx.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://brq.vehdjk.com

Py:   Counter(arr)
来源：http://gzd.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://uuq.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tme.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqd.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xeg.hnqzz.top

Go:   // 手写 map[T]int
来源：http://vuj.tanke756.top

Ruby: arr.tally
来源：http://xhg.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cnl.yonumen.top

[D21] 判断是否包含某元素
来源：http://biu.zhijiandao.cn

Py:   x in arr
来源：http://bty.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://woo.zycfv.cn

JS:   arr.includes(x)
来源：http://jrq.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://kpb.meibo888.top

Java: list.contains(x)
来源：http://zjs.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://lyf.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://iir.yuanzhike.top

C#:   list.Contains(x)
来源：http://ruf.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://kdw.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oom.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wef.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gvl.dashuyun.cn

TS:   [...arr];
来源：http://hre.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://xxi.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rai.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://uva.hfpthk.cn

C#:   new List<int>(list);
来源：http://rwb.hesvh.cn

[D23] reduce 累积计算
来源：http://erh.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qed.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ykn.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iem.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ctd.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ftd.quarkkingdee.top

Go:   // 手写循环
来源：http://lme.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://txm.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://trb.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://cca.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gck.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cyv.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qps.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fdg.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kis.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://smf.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rpr.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yaz.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://kgd.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nuc.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zuo.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://heo.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uhj.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uql.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://igy.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eou.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qed.ybcxt.top

[D26] 数组转字符串
来源：http://cux.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://ncc.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://utx.shuidangran.top

JS:   arr.join(", ")
来源：http://qzk.mhx1999.top

TS:   arr.join(", ")
来源：http://vxm.yuanzhike.top

Java: String.join(", ", list)
来源：http://gok.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://blp.dianchejie.cn

Ruby: arr.join(", ")
来源：http://ntf.iojbl.cn

C#:   string.Join(", ", list)
来源：http://ttq.hnxiangtu.top

================================================================================
来源：http://rmc.zdqjudy.top

E. 字符串处理
来源：http://awf.hcnkem.com

================================================================================
来源：http://rxi.cucudq.cn

[E01] 拼接字符串
来源：http://wbo.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cse.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xte.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyt.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmf.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mvm.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gga.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://auf.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xsf.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://pls.meibo888.top

Py:   "ab" * 3
来源：http://pew.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://qft.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://dje.pycfn.com

TS:   "ab".repeat(3)
来源：http://fik.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://ewf.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://mtm.nwbrower.top

Ruby: "ab" * 3
来源：http://nyz.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cpp.yongpay.top

[E03] 截取子串
来源：http://qfn.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://muc.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gjj.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://its.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://chu.yuanzhike.top

Java: s.substring(1, 4)
来源：http://vfu.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jcq.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://uac.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://iam.kuanghao11.cn

[E04] 查找子串位置
来源：http://qle.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://fqu.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://qrn.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ffi.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://eap.gzhubu.top

Java: s.indexOf("x")
来源：http://zib.yj202588.top

Go:   strings.Index(s, "x")
来源：http://iri.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://iom.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://lpj.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jog.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iqr.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fku.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wpm.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sna.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bme.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jsx.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gvk.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ccn.yj20258888.top

[E06] 替换子串
来源：http://lem.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ikf.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://btj.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ddy.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://cmo.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ebh.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uqu.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mdp.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://nsp.fehbvm.com

[E07] 按分隔符拆分
来源：http://ygk.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oxj.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcu.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mox.chenjidiqi.icu

TS:   s.split(",")
来源：http://ipr.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://xmb.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rmt.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://uej.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rxk.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://ezp.hcnkem.com

Py:   ",".join(items)
来源：http://tlc.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://jtz.yvedp.cn

JS:   items.join(",")
来源：http://fea.havefunace.top

TS:   items.join(",")
来源：http://qga.xinyue.icu

Java: String.join(",", items)
来源：http://jgj.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://klz.epnwcf.com

Ruby: items.join(",")
来源：http://xyo.daria6918.cn

C#:   string.Join(",", items)
来源：http://vem.bjfxy.top

[E09] 去除所有空白字符
来源：http://wpn.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kef.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcr.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://qdv.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://xwk.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://hzv.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pwi.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://stu.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fxi.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://uvg.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wnv.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tpn.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://mid.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://quo.tarul.cn

Java: String.format("%03d", 7)
来源：http://jbf.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xos.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xsd.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jql.nanxuanxn.top

[E11] 反转字符串
来源：http://vvp.birdmap.top

Py:   s[::-1]
来源：http://det.tianlin.xyz

PHP:  strrev($s);
来源：http://gdm.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://elr.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://zpj.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hcu.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lri.aibaodan.cn

Ruby: s.reverse
来源：http://vnd.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://ffq.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://jbn.xziqi.cn

Py:   s.count("a")
来源：http://emz.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://aig.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://yje.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://uwr.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iqy.pycfn.com

Go:   strings.Count(s, "a")
来源：http://wov.quarkkingdee.top

Ruby: s.count("a")
来源：http://oer.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://ymm.guannengcc.top

[E13] 逐字符遍历
来源：http://hqm.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://cao.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://avq.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zia.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://tbl.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ldd.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rbe.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://uhm.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nuc.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://oxv.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qih.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gva.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swt.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qwr.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kry.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pff.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gzt.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vin.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://cyo.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://sgx.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khe.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://shw.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ujc.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqh.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://grx.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dex.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dmm.yuxming.cn

[E16] 数字千分位
来源：http://wrf.shuidangran.top

Py:   f"{1234567:,}"
来源：http://ofb.xziqi.cn

PHP:  number_format(1234567);
来源：http://jno.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cko.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ypk.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://acp.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ofz.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rit.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://sds.nanxinkj.top

[E17] 首字母大写
来源：http://ywf.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cub.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pka.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqm.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opi.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rfx.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xbc.tianlin.xyz

Ruby: s.capitalize
来源：http://lbg.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xmq.redwolf501.top


<!-- 参考信息 -->