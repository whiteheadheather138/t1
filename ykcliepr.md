代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kfg.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://usd.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://dfy.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://frt.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmz.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://pda.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vrj.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://udd.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vxh.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yws.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://diw.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://xzv.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://mzy.nanxuanxn.top

Go:   // 手写循环
来源：http://lbn.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://enh.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xuj.yangfankeji.com

[D15] 去重
来源：http://nbn.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cgj.jyoumei.cn

PHP:  array_unique($arr);
来源：http://tdg.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://odl.smart0.xyz

TS:   [...new Set(arr)]
来源：http://atm.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mdu.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://fsw.9152youxi.cn

Ruby: arr.uniq
来源：http://wao.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://byl.yuanzhike.top

[D16] 求和与平均值
来源：http://yoo.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyi.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ana.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yfo.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yfi.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hvr.chenlongwang.top

Go:   // 手写循环累加
来源：http://kfs.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdj.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://dnc.ybcxt.top

[D17] 最大值与最小值
来源：http://cqc.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://ezu.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://bhd.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://irb.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://nll.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fkq.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tac.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://vxg.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://vew.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://uyl.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hkl.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://rcs.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bno.nwbrower.top

TS:   nested.flat();
来源：http://zoa.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iqu.uphjek.com

Go:   // 手写双层循环
来源：http://bek.c1oappe.top

Ruby: nested.flatten
来源：http://ajf.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jkq.tarul.cn

[D19] 按字段分组
来源：http://wzv.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kck.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wzm.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ppo.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ope.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pyl.birdmap.top

Go:   // 手写 map[string][]T
来源：http://qiv.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gar.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lmj.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://gqu.epnwcf.com

Py:   Counter(arr)
来源：http://kkq.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://wgt.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dye.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fet.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jfs.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://vnm.shangyingyoupin.top

Ruby: arr.tally
来源：http://nyp.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://znl.aizwys.cn

[D21] 判断是否包含某元素
来源：http://yxo.shuidangran.top

Py:   x in arr
来源：http://aje.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://oyn.shzxlz.cn

JS:   arr.includes(x)
来源：http://ryv.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://cql.yueranfly.top

Java: list.contains(x)
来源：http://vzo.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://hyk.52xcode.cn

Ruby: arr.include?(x)
来源：http://qhc.jqgfzy.top

C#:   list.Contains(x)
来源：http://eaq.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://lzp.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lne.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nxb.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://flc.xylfe.cn

TS:   [...arr];
来源：http://ozi.sxryk.cn

Java: new ArrayList<>(list);
来源：http://qnw.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://dxg.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://lcc.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://jvu.sysykeji.top

[D23] reduce 累积计算
来源：http://haz.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://upj.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sro.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gvz.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbe.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mxe.gogol.net.cn

Go:   // 手写循环
来源：http://zuj.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qdr.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhe.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://hcr.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://avq.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://enk.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jqg.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xgy.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fwc.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vyi.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mqw.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bxc.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://wkj.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aai.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jtr.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://okk.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbl.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cps.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lfr.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sth.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rnp.fktsv.cn

[D26] 数组转字符串
来源：http://edx.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://xvm.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://tte.meibo888.top

JS:   arr.join(", ")
来源：http://whp.fktsv.cn

TS:   arr.join(", ")
来源：http://mno.cdnleiting.top

Java: String.join(", ", list)
来源：http://bep.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://mtz.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://yyh.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://wmq.52xcode.cn

================================================================================
来源：http://avh.xuetiantiany.cn

E. 字符串处理
来源：http://hrk.daria6918.cn

================================================================================
来源：http://ldh.xuetiantiany.cn

[E01] 拼接字符串
来源：http://lui.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://irv.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://caa.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baz.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzq.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qcs.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ejc.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uvm.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tag.yj20258888.top

[E02] 重复字符串
来源：http://jld.zdbjq.cn

Py:   "ab" * 3
来源：http://rfr.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://akx.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://vnj.fktsv.cn

TS:   "ab".repeat(3)
来源：http://yap.jyoumei.cn

Java: "ab".repeat(3)
来源：http://shv.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zjk.fktsv.cn

Ruby: "ab" * 3
来源：http://ser.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://npz.shuidangran.top

[E03] 截取子串
来源：http://soa.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dbe.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nlq.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://avi.jyoumei.cn

TS:   s.slice(1, 4)
来源：http://zae.cdnleiting.top

Java: s.substring(1, 4)
来源：http://dwq.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lft.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://whg.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://fiz.chenzaomai.com

[E04] 查找子串位置
来源：http://hyr.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://zup.52xcode.cn

PHP:  strpos($s, "x");
来源：http://xfm.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eho.guannengcc.top

TS:   s.indexOf("x")
来源：http://dkf.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://baj.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://ewb.haohaochexian.top

Ruby: s.index("x")
来源：http://kfg.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://bdp.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jbi.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qtg.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://prc.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wgs.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://hiw.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukj.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tru.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tzb.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zdg.hfpthk.cn

[E06] 替换子串
来源：http://ufj.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gpz.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://gqt.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fca.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://nhi.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gft.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://psn.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qnw.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://cdb.jqgfzy.top

[E07] 按分隔符拆分
来源：http://tet.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zcj.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://etz.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yxc.meibo888.top

TS:   s.split(",")
来源：http://bxc.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://tag.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aqq.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://bxi.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://csy.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://ewq.sxryk.cn

Py:   ",".join(items)
来源：http://vsy.hammf.cn

PHP:  implode(",", $items);
来源：http://zey.zdbjq.cn

JS:   items.join(",")
来源：http://cwj.gogol.net.cn

TS:   items.join(",")
来源：http://syx.vqdsnc.cn

Java: String.join(",", items)
来源：http://mgk.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://seq.tian-w.cn

Ruby: items.join(",")
来源：http://slr.nwbrower.top

C#:   string.Join(",", items)
来源：http://cej.hcnkem.com

[E09] 去除所有空白字符
来源：http://uqj.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://brk.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vjz.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://rpu.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://pvq.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://jdk.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mdf.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bct.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hwg.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://gqo.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yle.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qud.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://uon.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://rrj.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://frl.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gxl.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://afa.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zbj.bjfxy.top

[E11] 反转字符串
来源：http://neg.sufxvd.cn

Py:   s[::-1]
来源：http://jne.zhijiandao.cn

PHP:  strrev($s);
来源：http://tce.ivvv.top

JS:   [...s].reverse().join("")
来源：http://qkv.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://fbf.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tbe.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tmd.zycfv.cn

Ruby: s.reverse
来源：http://vmi.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://bov.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://jud.9152youxi.cn

Py:   s.count("a")
来源：http://yun.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://rgg.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://gfm.fktsv.cn

TS:   s.split("a").length - 1
来源：http://xhv.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qmh.meibo888.top

Go:   strings.Count(s, "a")
来源：http://oky.hfpthk.cn

Ruby: s.count("a")
来源：http://zih.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://dpn.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://uov.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://eal.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vzf.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rby.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tbc.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ltm.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ldl.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jdn.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://arf.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://gkz.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xbq.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://pxq.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qcu.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mxn.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oqk.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wrq.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uym.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tso.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://thk.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ygy.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xde.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gyt.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://nrk.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zqb.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://csw.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hgg.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://shx.jqgfzy.top

[E16] 数字千分位
来源：http://nyr.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://don.tianlin.xyz

PHP:  number_format(1234567);
来源：http://xkn.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://egf.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xdj.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aks.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqn.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xuv.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://qit.yj20258888.top

[E17] 首字母大写
来源：http://ybn.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://srm.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vhs.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewe.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rzj.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ftv.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://esa.zhijiandao.cn

Ruby: s.capitalize
来源：http://gwt.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://srh.yongpay.top

[E18] 模板占位符替换
来源：http://akn.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fyq.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rhv.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://iib.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://msy.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lqa.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eli.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://odt.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yha.daria6918.cn

[E19] 多行文本按行拆分
来源：http://jri.sjlbkw.cn

Py:   s.splitlines()
来源：http://ppf.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ykl.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://eqm.sweek.top

TS:   s.split(/\r?\n/)
来源：http://snu.xinyue.icu

Java: s.lines().toList()
来源：http://coz.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://rii.mhx1999.top

Ruby: s.lines
来源：http://sfj.shuidangran.top

C#:   s.Split('\n')
来源：http://dor.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://nai.zhiwuduotai.top

Py:   if not s:
来源：http://gqj.cdnleiting.top


<!-- 参考信息 -->