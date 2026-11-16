代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayl.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://vho.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://sqq.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rhy.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jog.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ijw.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ogt.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://ruj.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fpi.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qvl.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://bkl.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://hep.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://jgl.hnxiangtu.top

Go:   // 手写循环
来源：http://bni.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://opo.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nmr.xingfuxueyuan.xyz

[D15] 去重
来源：http://bbr.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hgl.yongpay.top

PHP:  array_unique($arr);
来源：http://moy.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://elr.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://tnn.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jfl.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bnl.andypj.xyz

Ruby: arr.uniq
来源：http://hlu.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://rkv.cdnleiting.top

[D16] 求和与平均值
来源：http://sjt.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pvj.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vzp.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tng.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vko.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rtu.epnwcf.com

Go:   // 手写循环累加
来源：http://lxd.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://alf.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://nmz.tanke756.top

[D17] 最大值与最小值
来源：http://mqb.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://anb.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://oyp.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qpv.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://nbm.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jcc.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rlc.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://wrl.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://ahe.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://svl.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rff.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://zjg.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hkk.yuxming.cn

TS:   nested.flat();
来源：http://wyw.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jld.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://dow.tarul.cn

Ruby: nested.flatten
来源：http://pcs.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ifu.yongpay.top

[D19] 按字段分组
来源：http://fhr.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ghc.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pbj.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vop.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyr.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eez.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://zwb.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://chc.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kwo.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://pqk.dashuyun.cn

Py:   Counter(arr)
来源：http://avo.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://ckl.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abz.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://irm.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tep.shuidangran.top

Go:   // 手写 map[T]int
来源：http://sjo.cashguo.top

Ruby: arr.tally
来源：http://vlu.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axf.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://czt.cheryme.top

Py:   x in arr
来源：http://qlh.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://gxk.havefunace.top

JS:   arr.includes(x)
来源：http://oqv.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://cnm.ydjk.org.cn

Java: list.contains(x)
来源：http://emx.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://bnn.ivvv.top

Ruby: arr.include?(x)
来源：http://gyn.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://yic.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://mij.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fsx.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cne.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xng.hesvh.cn

TS:   [...arr];
来源：http://rwa.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://hyj.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://zrq.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://pmh.ppjwa.cn

C#:   new List<int>(list);
来源：http://nnm.0kj1m.cn

[D23] reduce 累积计算
来源：http://pfx.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fyq.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dae.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gpi.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tdy.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://vzd.fktsv.cn

Go:   // 手写循环
来源：http://yep.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vyy.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://usr.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://rde.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kax.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ltc.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://evt.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://weh.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wpz.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dhe.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cgf.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uml.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://ajv.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qcy.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pmm.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pzy.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nne.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uxg.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eha.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xul.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://umm.sjlbkw.cn

[D26] 数组转字符串
来源：http://tkl.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://bxa.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://vjk.hnxiangtu.top

JS:   arr.join(", ")
来源：http://kie.yfazqb.com

TS:   arr.join(", ")
来源：http://oga.zdqjudy.top

Java: String.join(", ", list)
来源：http://osu.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://sav.cdnleiting.top

Ruby: arr.join(", ")
来源：http://rvp.jianghu66.top

C#:   string.Join(", ", list)
来源：http://aap.shanyushiyangkeji.top

================================================================================
来源：http://tiq.shanyushiyangtech.top

E. 字符串处理
来源：http://ovv.guowangkeji.top

================================================================================
来源：http://mwv.iojbl.cn

[E01] 拼接字符串
来源：http://kyf.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ygz.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vzq.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bve.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvx.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oda.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gjy.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iil.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://epb.ydjk.org.cn

[E02] 重复字符串
来源：http://csb.kuanghao11.cn

Py:   "ab" * 3
来源：http://xox.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://nqw.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://rwd.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://fuh.ydzc1.top

Java: "ab".repeat(3)
来源：http://axw.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://aad.yonumen.top

Ruby: "ab" * 3
来源：http://awh.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bvz.bbcook.cn

[E03] 截取子串
来源：http://utq.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://auk.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iob.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ewz.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://dqn.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://nnd.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tnf.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://oii.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://uod.pengpengdd.cyou

[E04] 查找子串位置
来源：http://jee.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://ahs.daxiang520.top

PHP:  strpos($s, "x");
来源：http://dpm.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gsn.tarul.cn

TS:   s.indexOf("x")
来源：http://mcb.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://eoc.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://jcp.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://uws.fengsongda.top

C#:   s.IndexOf("x")
来源：http://pin.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rsr.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oqb.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dwi.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rvf.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpu.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vix.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bfs.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqs.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fpl.redwolf501.top

[E06] 替换子串
来源：http://lal.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uzx.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://jwf.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikf.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://orx.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iap.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzl.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cgy.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://yxt.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://zls.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ygq.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ehd.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://joc.daxiang520.top

TS:   s.split(",")
来源：http://okd.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xea.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xqj.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://ind.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dbo.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://efm.yj20258888.top

Py:   ",".join(items)
来源：http://rha.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://mmy.zdbjq.cn

JS:   items.join(",")
来源：http://hcn.redwolf501.top

TS:   items.join(",")
来源：http://sfd.birdmap.top

Java: String.join(",", items)
来源：http://vwh.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://xse.hammf.cn

Ruby: items.join(",")
来源：http://hrm.jiagoushi.top

C#:   string.Join(",", items)
来源：http://per.daxiang520.top

[E09] 去除所有空白字符
来源：http://spa.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rys.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://onp.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://dis.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://jmp.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://uom.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nek.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://fze.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://foq.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://xkf.havefunace.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qrw.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jua.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://ott.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://trw.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://zcb.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://upc.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xav.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://axy.epnwcf.com

[E11] 反转字符串
来源：http://dsw.yj20258888.top

Py:   s[::-1]
来源：http://gyh.chenlongwang.top

PHP:  strrev($s);
来源：http://hqa.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://mol.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://dzy.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xdx.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://skl.xuanzx.com

Ruby: s.reverse
来源：http://jhe.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://zar.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://zoy.cheryme.top

Py:   s.count("a")
来源：http://sfz.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://ani.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://grw.meibo888.top

TS:   s.split("a").length - 1
来源：http://noi.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fly.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://ddz.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://pvq.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://mac.shzxlz.cn

[E13] 逐字符遍历
来源：http://yoj.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://bku.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://urm.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://kqe.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rno.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fcj.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sdb.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yxz.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vbz.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://fvf.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lyz.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://csx.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mie.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xwa.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://afc.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ptu.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mpr.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bzs.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://ome.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://epe.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://edn.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kid.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://yhx.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gnc.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vhc.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oba.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gcb.yfazqb.com

[E16] 数字千分位
来源：http://xty.xziqi.cn

Py:   f"{1234567:,}"
来源：http://jnt.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://tda.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://mnw.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jsw.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://upw.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vrt.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cta.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://ghd.xuanzx.com

[E17] 首字母大写
来源：http://dwn.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mkv.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bgj.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://crx.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzt.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tev.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fgv.hfpthk.cn

Ruby: s.capitalize
来源：http://muc.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sgn.ydzc1.top

[E18] 模板占位符替换
来源：http://yvh.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bfg.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wyu.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lwj.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hgg.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ltj.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wdw.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dpc.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xom.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://afw.gogol.net.cn

Py:   s.splitlines()
来源：http://tku.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ist.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://mwp.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://bal.gotoacloud.top

Java: s.lines().toList()
来源：http://pqm.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://mzq.gogol.net.cn

Ruby: s.lines
来源：http://evh.daxiang520.top

C#:   s.Split('\n')
来源：http://ser.ydzc1.top

[E20] 判断字符串是否为空
来源：http://ffi.daria6918.cn

Py:   if not s:
来源：http://wwu.zhengqikj.top


<!-- 参考信息 -->