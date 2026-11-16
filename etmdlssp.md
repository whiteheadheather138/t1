代发 wailian999

Ruby: arr.index(x)
来源：http://vrl.yuxming.cn

C#:   list.IndexOf(x);
来源：http://aah.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://zri.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ozy.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xet.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://rex.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://hde.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://arw.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ssy.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://oqa.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bdl.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://exk.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mdq.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ivd.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://xie.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://rxh.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://kau.316326.xyz

Go:   // 手写循环
来源：http://wec.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nrz.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wkq.uphjek.com

[D15] 去重
来源：http://gkb.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ivq.sysykeji.top

PHP:  array_unique($arr);
来源：http://xhf.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://nei.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://uov.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rvc.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xia.jqgufenzy.top

Ruby: arr.uniq
来源：http://sev.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://eqy.ybcxt.top

[D16] 求和与平均值
来源：http://zcv.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aor.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wqy.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sez.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjs.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://axa.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://jtz.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fcr.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://rfh.bjfxy.top

[D17] 最大值与最小值
来源：http://yrr.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://jtw.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://csz.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hxq.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://iej.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rve.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qgx.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://pco.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://gvb.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://dor.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oci.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://shr.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uqo.mhx1999.top

TS:   nested.flat();
来源：http://xzq.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dov.nwbrower.top

Go:   // 手写双层循环
来源：http://leb.snrcjt.cn

Ruby: nested.flatten
来源：http://vfp.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qbu.ivvv.top

[D19] 按字段分组
来源：http://rsg.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wcz.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iwz.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tye.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kxr.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ohx.yonumen.top

Go:   // 手写 map[string][]T
来源：http://nct.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzg.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zxv.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://woq.hnxiangtu.top

Py:   Counter(arr)
来源：http://qjb.xziqi.cn

PHP:  array_count_values($arr);
来源：http://nqg.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euz.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ybd.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nzh.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://vbg.shzxlz.cn

Ruby: arr.tally
来源：http://eod.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twr.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://sor.quarkkingdee.top

Py:   x in arr
来源：http://nis.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://sqv.smart0.xyz

JS:   arr.includes(x)
来源：http://fot.0kj1m.cn

TS:   arr.includes(x)
来源：http://jmx.fehbvm.com

Java: list.contains(x)
来源：http://ogm.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://wli.mhx1999.top

Ruby: arr.include?(x)
来源：http://ozl.uphjek.com

C#:   list.Contains(x)
来源：http://kkw.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://pgn.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://avm.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fps.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rdz.52xcode.cn

TS:   [...arr];
来源：http://nsf.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://vzh.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://xha.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://wfs.zhongyouzk.top

C#:   new List<int>(list);
来源：http://hkd.redwolf501.top

[D23] reduce 累积计算
来源：http://sju.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nbo.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ynw.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sqh.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msv.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fgy.ppjwa.cn

Go:   // 手写循环
来源：http://spw.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tcb.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uxt.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://ljt.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pwu.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ilu.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vbf.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aqu.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uyd.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iil.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aau.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bqv.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://eho.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kws.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kuj.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yxh.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dzv.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jbt.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yno.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aps.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://olc.hnxiangtu.top

[D26] 数组转字符串
来源：http://hzt.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://bdp.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://mfx.iojbl.cn

JS:   arr.join(", ")
来源：http://nwi.9152youxi.cn

TS:   arr.join(", ")
来源：http://bgz.sweek.top

Java: String.join(", ", list)
来源：http://nbz.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://xlq.bbcook.cn

Ruby: arr.join(", ")
来源：http://jex.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://rba.andypj.xyz

================================================================================
来源：http://zvf.yuanzhike.top

E. 字符串处理
来源：http://yzz.vqdsnc.cn

================================================================================
来源：http://bro.iojbl.cn

[E01] 拼接字符串
来源：http://fue.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://imi.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dea.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pai.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdm.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvd.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://psu.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ozo.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzx.jqgfzy.top

[E02] 重复字符串
来源：http://kty.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://nsg.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://nhf.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://dfr.hnqzz.top

TS:   "ab".repeat(3)
来源：http://uol.bbcook.cn

Java: "ab".repeat(3)
来源：http://goh.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://hes.zhongyouzk.top

Ruby: "ab" * 3
来源：http://nae.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bpz.ywan-chungtsiang.top

[E03] 截取子串
来源：http://lph.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://btq.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lxh.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pzx.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://fll.cheryme.top

Java: s.substring(1, 4)
来源：http://vii.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tmx.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bgd.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://ucv.tianlin.xyz

[E04] 查找子串位置
来源：http://exh.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://lju.birdmap.top

PHP:  strpos($s, "x");
来源：http://kpe.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pev.ehwqpu.com

TS:   s.indexOf("x")
来源：http://ksx.chenzaomai.com

Java: s.indexOf("x")
来源：http://mfm.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://yrb.fzhhl.top

Ruby: s.index("x")
来源：http://ijs.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://srk.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hac.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pol.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://odg.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://grn.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qwx.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpr.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jxm.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gar.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gox.jinghuilouyu.cn

[E06] 替换子串
来源：http://gxu.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://evp.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://eyu.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwl.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://jkl.mhx1999.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zke.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zhn.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://irp.cashguo.top

C#:   s.Replace("a", "b")
来源：http://wal.nanxinkj.top

[E07] 按分隔符拆分
来源：http://otq.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zdv.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dfg.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ilb.dashuyun.cn

TS:   s.split(",")
来源：http://uxd.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://rxk.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cey.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://sqg.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://okt.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://bas.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://uyw.316326.xyz

PHP:  implode(",", $items);
来源：http://qyz.zhixingplan.top

JS:   items.join(",")
来源：http://hpv.ivvv.top

TS:   items.join(",")
来源：http://hzu.0kj1m.cn

Java: String.join(",", items)
来源：http://edw.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://gay.shuidangran.top

Ruby: items.join(",")
来源：http://gss.jianghu66.top

C#:   string.Join(",", items)
来源：http://gxo.hnqzz.top

[E09] 去除所有空白字符
来源：http://new.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xyy.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://crg.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ktn.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://njm.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://vnz.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://reb.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://fnd.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://epo.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://gqx.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eoi.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://voj.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://dca.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://lbn.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://qmq.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gzb.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kep.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uva.hfpthk.cn

[E11] 反转字符串
来源：http://ely.sxryk.cn

Py:   s[::-1]
来源：http://ipm.wangshuangyany.cn

PHP:  strrev($s);
来源：http://pfb.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://hxi.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://upi.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ini.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmh.gzhubu.top

Ruby: s.reverse
来源：http://tiq.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lfh.yonumen.top

[E12] 统计某字符出现次数
来源：http://van.9152youxi.cn

Py:   s.count("a")
来源：http://qlw.yongpay.top

PHP:  substr_count($s, "a");
来源：http://jsw.sysykeji.top

JS:   s.split("a").length - 1
来源：http://fcj.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://mhu.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dat.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://hhh.snrcjt.cn

Ruby: s.count("a")
来源：http://zlj.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://ztd.zhongyouzk.top

[E13] 逐字符遍历
来源：http://ljc.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://xha.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://biv.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://spi.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lib.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxk.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vly.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cgu.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rsz.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://evz.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fkn.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wey.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://roc.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://clv.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lho.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aia.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://drs.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ods.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://vzw.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pqf.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fne.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://shb.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sar.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qqj.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tko.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xqk.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uwa.havefunace.top

[E16] 数字千分位
来源：http://vfs.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://wdw.daxiang520.top

PHP:  number_format(1234567);
来源：http://iiu.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zzi.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jfa.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sql.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qex.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xsv.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://hix.yj20258888.top

[E17] 首字母大写
来源：http://xnl.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xbx.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dlb.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xzo.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ttf.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hig.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xjr.zhixingplan.top

Ruby: s.capitalize
来源：http://uzj.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xmw.andypj.xyz

[E18] 模板占位符替换
来源：http://kuz.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xgv.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xsz.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://arw.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://myx.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzo.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wlb.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tmn.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nxy.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://ill.316326.xyz

Py:   s.splitlines()
来源：http://oik.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tfh.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://jbd.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://bzc.chenjidiqi.icu

Java: s.lines().toList()
来源：http://wiz.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://bcp.yj20258888.top


<!-- 参考信息 -->