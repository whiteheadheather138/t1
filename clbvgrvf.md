代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgh.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zlu.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jtt.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://qss.iojbl.cn

Ruby: arr.index(x)
来源：http://bnd.wangdashe.top

C#:   list.IndexOf(x);
来源：http://gew.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://vot.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bfr.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxl.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://hvz.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://cka.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nel.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lrr.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lsx.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xbn.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://vql.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pls.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nuh.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://eus.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://tzk.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yqd.hnqzz.top

Go:   // 手写循环
来源：http://bdm.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hcj.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ppl.daxiang520.top

[D15] 去重
来源：http://dzu.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oxz.cucudq.cn

PHP:  array_unique($arr);
来源：http://xrv.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://wnu.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://tmb.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wbu.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://nix.hysaishi.cn

Ruby: arr.uniq
来源：http://pab.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://jgm.jianghu66.top

[D16] 求和与平均值
来源：http://zkd.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://psq.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rfm.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbu.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hna.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fjv.yonumen.top

Go:   // 手写循环累加
来源：http://gpa.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ftr.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://wdr.ehwqpu.com

[D17] 最大值与最小值
来源：http://csf.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://unn.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://rjd.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ego.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://lea.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://izo.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ckf.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://hiv.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://gaj.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://ozt.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ndy.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://jfp.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aqd.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://ikq.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yov.dashuyun.cn

Go:   // 手写双层循环
来源：http://caf.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://vxh.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://vti.fehbvm.com

[D19] 按字段分组
来源：http://mtu.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ymb.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jah.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bqz.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wme.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbu.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://imk.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hcs.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://toy.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://ide.yanxiufei.cn

Py:   Counter(arr)
来源：http://vzv.c1oappe.top

PHP:  array_count_values($arr);
来源：http://hdq.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jhk.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqk.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vwd.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://jpb.52xcode.cn

Ruby: arr.tally
来源：http://wxe.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dki.yj20258888.top

[D21] 判断是否包含某元素
来源：http://tpw.yfazqb.com

Py:   x in arr
来源：http://svq.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://afj.fehbvm.com

JS:   arr.includes(x)
来源：http://asp.yfazqb.com

TS:   arr.includes(x)
来源：http://ukd.ydzc1.top

Java: list.contains(x)
来源：http://fts.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://ygb.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://lbx.hysaishi.cn

C#:   list.Contains(x)
来源：http://dje.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://sqm.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tii.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfv.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://srf.yj20258888.top

TS:   [...arr];
来源：http://uzk.guannengcc.top

Java: new ArrayList<>(list);
来源：http://dhg.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://kej.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://noa.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://dwv.xuanzx.com

[D23] reduce 累积计算
来源：http://yyw.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ypl.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bwa.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wye.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zpa.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cll.chenzaomai.com

Go:   // 手写循环
来源：http://qgq.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mmh.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pwm.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://tkz.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mxa.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aof.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://igt.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ypz.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pgp.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qst.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcz.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gqk.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://tip.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://usz.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://swc.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lfc.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tpg.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ycq.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fba.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wln.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fif.svipenyu.cn

[D26] 数组转字符串
来源：http://iee.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://cet.yj202588.top

PHP:  implode(", ", $arr);
来源：http://eau.bbcook.cn

JS:   arr.join(", ")
来源：http://zuf.hnxiangtu.top

TS:   arr.join(", ")
来源：http://txf.hnxiangtu.top

Java: String.join(", ", list)
来源：http://wvn.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://wsw.xziqi.cn

Ruby: arr.join(", ")
来源：http://sas.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://wnl.sxryk.cn

================================================================================
来源：http://dzd.shzxlz.cn

E. 字符串处理
来源：http://elz.sweek.top

================================================================================
来源：http://bfv.ppjwa.cn

[E01] 拼接字符串
来源：http://ssz.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iwd.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://quw.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mey.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ekp.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yjh.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdc.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqc.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cey.yonumen.top

[E02] 重复字符串
来源：http://tdd.52xcode.cn

Py:   "ab" * 3
来源：http://hnw.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://tfq.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://vyx.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://heg.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://ukd.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://uya.vqdsnc.cn

Ruby: "ab" * 3
来源：http://pcz.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vlv.yangfankeji.com

[E03] 截取子串
来源：http://fia.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://koq.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tfl.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jkb.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://nkg.yongpay.top

Java: s.substring(1, 4)
来源：http://opt.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ota.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ofq.sweek.top

C#:   s.Substring(1, 3)
来源：http://jco.sxryk.cn

[E04] 查找子串位置
来源：http://mjj.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://afg.yueranfly.top

PHP:  strpos($s, "x");
来源：http://pta.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ulg.dashuyun.cn

TS:   s.indexOf("x")
来源：http://mnb.tarul.cn

Java: s.indexOf("x")
来源：http://eae.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://sij.nwbrower.top

Ruby: s.index("x")
来源：http://uhk.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://fpi.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wfj.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://phd.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://edi.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lsp.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kab.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvc.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kkc.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://coz.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lzs.redwolf501.top

[E06] 替换子串
来源：http://hrw.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fvy.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://zbd.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uni.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://dxs.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qmy.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://izu.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sjk.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://ixq.jinqigufen.top

[E07] 按分隔符拆分
来源：http://ran.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aie.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hdh.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://idj.guannengcc.top

TS:   s.split(",")
来源：http://rhp.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://ixf.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oie.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://zjb.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pti.hcnkem.com

[E08] 数组按分隔符合并
来源：http://ctb.xuanzx.com

Py:   ",".join(items)
来源：http://nze.hysaishi.cn

PHP:  implode(",", $items);
来源：http://mdt.nanxinkj.top

JS:   items.join(",")
来源：http://wrp.fehbvm.com

TS:   items.join(",")
来源：http://sjg.guannengcc.top

Java: String.join(",", items)
来源：http://uud.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://egj.ivvv.top

Ruby: items.join(",")
来源：http://ddx.jiagoushi.top

C#:   string.Join(",", items)
来源：http://bcv.cdnleiting.top

[E09] 去除所有空白字符
来源：http://sof.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qnz.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tkw.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://dma.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ywj.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://rtu.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ogw.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://nwx.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nha.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://cyr.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xka.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xat.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://aup.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://vvq.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://qku.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ofo.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jmc.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nvp.vqdsnc.cn

[E11] 反转字符串
来源：http://lzy.yongpay.top

Py:   s[::-1]
来源：http://oub.shuidangran.top

PHP:  strrev($s);
来源：http://lzi.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://yon.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://zbs.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ovz.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rku.jlsjyb.cn

Ruby: s.reverse
来源：http://gmy.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://afc.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://aoa.shuidangran.top

Py:   s.count("a")
来源：http://yic.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://fxb.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://zje.bbcook.cn

TS:   s.split("a").length - 1
来源：http://enz.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lsr.cheryme.top

Go:   strings.Count(s, "a")
来源：http://zvr.gzhubu.top

Ruby: s.count("a")
来源：http://bnz.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://gqq.bbcook.cn

[E13] 逐字符遍历
来源：http://pzg.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://anx.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mny.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bsn.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ojl.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pik.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gtr.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mki.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xpk.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://psd.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xot.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dol.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwq.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lvd.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://osx.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lra.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ypd.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uid.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://vuw.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://juc.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fui.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cvg.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://itm.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bda.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qfa.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rof.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tzf.yj20258.top

[E16] 数字千分位
来源：http://phx.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://ufj.yvedp.cn

PHP:  number_format(1234567);
来源：http://gdm.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jzf.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pnc.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ozy.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eps.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dpq.316326.xyz

C#:   1234567.ToString("N0")
来源：http://ygl.0kj1m.cn

[E17] 首字母大写
来源：http://cen.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fvg.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ezy.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyg.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xot.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jmy.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mpf.daxiang520.top

Ruby: s.capitalize
来源：http://nvt.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ekn.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://eky.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tua.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qxl.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sbx.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ktq.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oiu.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bvs.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wkp.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fdm.nwbrower.top

[E19] 多行文本按行拆分
来源：http://cmp.iojbl.cn

Py:   s.splitlines()
来源：http://ais.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xfo.ywan-chungtsiang.top


<!-- 参考信息 -->