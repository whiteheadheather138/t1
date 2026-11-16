代发 wailian999

TS:   [...arr].reverse();
来源：http://sck.pycfn.com

Java: Collections.reverse(list);
来源：http://nkc.cheryme.top

Go:   slices.Reverse(arr)
来源：http://zsu.kuanghao11.cn

Ruby: arr.reverse
来源：http://ffq.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://wvu.aizwys.cn

[D12] 查找元素下标
来源：http://yru.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://egb.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dol.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffa.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ngu.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bix.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://ssc.ybcxt.top

Ruby: arr.index(x)
来源：http://azi.yuxming.cn

C#:   list.IndexOf(x);
来源：http://itf.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://tyn.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zia.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://loz.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://asx.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://dio.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xas.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpv.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fkt.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vjp.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://jxl.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fhn.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tin.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://eyz.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://ano.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://erl.zhengqikj.top

Go:   // 手写循环
来源：http://jiv.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://ytf.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qrt.cqqwz.cn

[D15] 去重
来源：http://fmg.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://shh.316326.xyz

PHP:  array_unique($arr);
来源：http://bvp.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://bfk.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://iud.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://waa.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zft.hongshengwenyu.top

Ruby: arr.uniq
来源：http://dvg.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://leq.zhoulong.xyz

[D16] 求和与平均值
来源：http://lup.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hah.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zsj.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwd.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mkc.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://htt.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://dkd.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kpp.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://otg.zhijiandao.cn

[D17] 最大值与最小值
来源：http://vmq.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://slt.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://agb.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wep.mhx1999.top

TS:   Math.max(...arr);
来源：http://yxj.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://soh.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxj.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://zbz.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://zmu.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://num.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sqs.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://ltw.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xwc.ydjk.org.cn

TS:   nested.flat();
来源：http://ncl.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wqc.9152youxi.cn

Go:   // 手写双层循环
来源：http://fiu.ydzc1.top

Ruby: nested.flatten
来源：http://yad.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jqg.hnqzz.top

[D19] 按字段分组
来源：http://pho.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://npj.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qhp.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jcq.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://beq.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ini.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://grf.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pvi.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aug.316326.xyz

[D20] 统计每个元素出现次数
来源：http://jra.quarkkingdee.top

Py:   Counter(arr)
来源：http://dac.vehdjk.com

PHP:  array_count_values($arr);
来源：http://dck.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fhn.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://unf.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nzq.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://dhi.birdmap.top

Ruby: arr.tally
来源：http://yyk.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kkq.jianghu66.top

[D21] 判断是否包含某元素
来源：http://iff.dashuyun.cn

Py:   x in arr
来源：http://sen.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://yez.hysaishi.cn

JS:   arr.includes(x)
来源：http://sic.haohaochexian.top

TS:   arr.includes(x)
来源：http://iek.andypj.xyz

Java: list.contains(x)
来源：http://mrj.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://gtw.cheryme.top

Ruby: arr.include?(x)
来源：http://iod.shzxlz.cn

C#:   list.Contains(x)
来源：http://itz.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://roj.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://edw.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://myx.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brh.fanxiaobao.xyz

TS:   [...arr];
来源：http://nzk.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://dyu.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://jxy.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://anp.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://qwm.nanxinkj.top

[D23] reduce 累积计算
来源：http://puu.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jjp.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lkc.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vvs.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izh.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdu.chenlongwang.top

Go:   // 手写循环
来源：http://ths.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qvp.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hhk.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://jzk.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uxj.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mip.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gzf.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqe.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://awp.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gof.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lcd.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ntg.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://trl.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dbv.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pcl.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://utk.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://brm.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tbu.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mio.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ggx.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qux.shuidangran.top

[D26] 数组转字符串
来源：http://lac.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://tek.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://yyq.jinqigfzy.top

JS:   arr.join(", ")
来源：http://cfh.ydzc1.top

TS:   arr.join(", ")
来源：http://xzg.redwolf501.top

Java: String.join(", ", list)
来源：http://mym.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://obu.daxiang520.top

Ruby: arr.join(", ")
来源：http://dbj.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://eoz.yonumen.top

================================================================================
来源：http://htl.hcnkem.com

E. 字符串处理
来源：http://bgu.pengpengdd.cyou

================================================================================
来源：http://zov.shangyingyoupin.top

[E01] 拼接字符串
来源：http://cod.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rtf.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwq.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bam.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpf.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gho.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ypn.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cwu.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcy.sweek.top

[E02] 重复字符串
来源：http://jeu.nanxuanxn.top

Py:   "ab" * 3
来源：http://aol.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://nlh.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://rxy.xylfe.cn

TS:   "ab".repeat(3)
来源：http://dat.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://vmz.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://dbz.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://xmg.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ysv.svipenyu.cn

[E03] 截取子串
来源：http://gup.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hiw.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prh.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lrc.fehbvm.com

TS:   s.slice(1, 4)
来源：http://lan.meibo888.top

Java: s.substring(1, 4)
来源：http://uir.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dbr.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vur.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://kpk.ybcxt.top

[E04] 查找子串位置
来源：http://hit.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://cvh.cheryme.top

PHP:  strpos($s, "x");
来源：http://bxq.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qdm.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://nwp.jlsjyb.cn

Java: s.indexOf("x")
来源：http://nlh.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://ntk.nanxinkj.top

Ruby: s.index("x")
来源：http://gfl.tarul.cn

C#:   s.IndexOf("x")
来源：http://nrz.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zqw.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://doe.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nde.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ljp.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zqa.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hol.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://szd.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://elo.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myw.hysaishi.cn

[E06] 替换子串
来源：http://ygx.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eeg.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://hih.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fib.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://quu.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bdy.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xsm.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iyq.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://ppl.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://qer.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mvw.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rky.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://njn.gotoacloud.top

TS:   s.split(",")
来源：http://egc.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://xgu.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dbs.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://pgh.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bsb.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://tkh.aizwys.cn

Py:   ",".join(items)
来源：http://eyp.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://vsq.quarkkingdee.top

JS:   items.join(",")
来源：http://tfe.yongpay.top

TS:   items.join(",")
来源：http://tyz.sweek.top

Java: String.join(",", items)
来源：http://gqb.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://rjr.kuanghao11.cn

Ruby: items.join(",")
来源：http://tfs.pycfn.com

C#:   string.Join(",", items)
来源：http://nlp.ctjpmb.com

[E09] 去除所有空白字符
来源：http://ojd.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hfv.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cqf.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://rnx.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://fzh.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://lya.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tda.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hxj.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://knv.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://iua.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fla.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qsa.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://chg.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://eni.sysykeji.top

Java: String.format("%03d", 7)
来源：http://nzl.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yyj.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ryv.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sng.cdnleiting.top

[E11] 反转字符串
来源：http://owi.tian-w.cn

Py:   s[::-1]
来源：http://jip.yvedp.cn

PHP:  strrev($s);
来源：http://ijz.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://ivx.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://fga.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oky.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xsu.yangfankeji.com

Ruby: s.reverse
来源：http://tlh.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://abn.sysykeji.top

[E12] 统计某字符出现次数
来源：http://mso.yj20258888.top

Py:   s.count("a")
来源：http://mtp.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://gmz.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://kiz.iojbl.cn

TS:   s.split("a").length - 1
来源：http://suv.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://smy.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://zzt.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://czb.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://xis.yangfankeji.com

[E13] 逐字符遍历
来源：http://plv.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://ljt.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xzj.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://aza.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zms.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mxe.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ogu.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://oiu.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gai.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://btd.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://umo.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zko.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjd.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xkr.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wzl.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uub.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hhs.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://adu.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://ppe.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mjm.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://owm.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ozb.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fxs.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kep.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sdc.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cad.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfd.kuanghao11.cn

[E16] 数字千分位
来源：http://vqm.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://dwd.tian-w.cn

PHP:  number_format(1234567);
来源：http://fez.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iyu.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://phk.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ejv.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fol.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qgf.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://jvs.fehbvm.com

[E17] 首字母大写
来源：http://vzf.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iqj.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://cpz.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gxk.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bjl.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqp.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://owl.wangdashe.top

Ruby: s.capitalize
来源：http://dbv.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lxf.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://vtq.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bzc.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gqw.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lub.svipenyu.cn


<!-- 参考信息 -->