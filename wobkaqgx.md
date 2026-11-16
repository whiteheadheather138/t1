代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qjw.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://icg.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://blj.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bls.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yhy.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://lwg.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mli.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://ape.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wpq.sweek.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oeq.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://lgn.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://urn.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hfz.zycfv.cn

Go:   // 手写循环
来源：http://tnz.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wzk.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lmv.9152youxi.cn

[D15] 去重
来源：http://sbm.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qfl.yueranfly.top

PHP:  array_unique($arr);
来源：http://qxw.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://lru.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://ply.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rld.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://zfw.mhx1999.top

Ruby: arr.uniq
来源：http://qag.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://ykk.fktsv.cn

[D16] 求和与平均值
来源：http://fml.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gvm.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nxu.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilz.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnp.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lod.hnxiangtu.top

Go:   // 手写循环累加
来源：http://exz.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tfh.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://owl.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://ske.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://tkh.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://obr.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zuy.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://nax.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rsr.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nfx.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://rjw.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://vut.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://har.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lfv.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://cts.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dcc.chenlongwang.top

TS:   nested.flat();
来源：http://ozt.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://msc.iojbl.cn

Go:   // 手写双层循环
来源：http://uql.nwbrower.top

Ruby: nested.flatten
来源：http://qbb.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mvv.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://zpv.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://elp.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://khg.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://evx.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zos.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wiu.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://sac.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://old.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kvy.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://hlc.wangshuangyany.cn

Py:   Counter(arr)
来源：http://wpa.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://ltf.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://znt.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmn.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kbp.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://cqg.yuanzhike.top

Ruby: arr.tally
来源：http://bkm.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ipf.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://liq.epnwcf.com

Py:   x in arr
来源：http://gtr.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://mlo.aibaodan.cn

JS:   arr.includes(x)
来源：http://kxn.sweek.top

TS:   arr.includes(x)
来源：http://fsc.yueranfly.top

Java: list.contains(x)
来源：http://qnv.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://orb.ppjwa.cn

Ruby: arr.include?(x)
来源：http://ywc.daxiang520.top

C#:   list.Contains(x)
来源：http://whe.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://gfj.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iqv.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oij.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nne.shanyushiyangtech.top

TS:   [...arr];
来源：http://luh.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://zph.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://yzs.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ers.epnwcf.com

C#:   new List<int>(list);
来源：http://hsg.ctjpmb.com

[D23] reduce 累积计算
来源：http://lup.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://itb.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pzl.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jae.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://czn.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sby.jlsjyb.cn

Go:   // 手写循环
来源：http://gli.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mby.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eij.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://jmb.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zjl.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ntm.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dwc.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://efn.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qdi.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ift.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lgw.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hon.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://hea.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qiz.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jvr.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dkp.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bas.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mtm.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://enh.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lxl.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lju.quarkkingdee.top

[D26] 数组转字符串
来源：http://ula.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://ouh.tarul.cn

PHP:  implode(", ", $arr);
来源：http://oim.fktsv.cn

JS:   arr.join(", ")
来源：http://wwz.smart0.xyz

TS:   arr.join(", ")
来源：http://mjk.zycfv.cn

Java: String.join(", ", list)
来源：http://mmh.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://fjr.iojbl.cn

Ruby: arr.join(", ")
来源：http://ntv.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://gxr.zhijiandao.cn

================================================================================
来源：http://xtc.ctjpmb.com

E. 字符串处理
来源：http://yqq.cashguo.top

================================================================================
来源：http://php.gaohongyu789.top

[E01] 拼接字符串
来源：http://cxv.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dod.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ess.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ecd.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbk.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wcv.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hfs.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gus.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ywz.tianlin.xyz

[E02] 重复字符串
来源：http://pof.hnqzz.top

Py:   "ab" * 3
来源：http://hgp.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://eyb.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://jiz.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://ijq.fktsv.cn

Java: "ab".repeat(3)
来源：http://ick.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://awp.fengsongda.top

Ruby: "ab" * 3
来源：http://svs.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://waq.ppjwa.cn

[E03] 截取子串
来源：http://nyx.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ccj.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tfk.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mec.yj20258.top

TS:   s.slice(1, 4)
来源：http://nzk.aizwys.cn

Java: s.substring(1, 4)
来源：http://uxp.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mrj.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iyy.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://zas.fktsv.cn

[E04] 查找子串位置
来源：http://rfn.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://pol.yfazqb.com

PHP:  strpos($s, "x");
来源：http://our.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jop.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://hii.uphjek.com

Java: s.indexOf("x")
来源：http://jvv.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://czk.yj20258.top

Ruby: s.index("x")
来源：http://shc.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://oud.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bzs.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxk.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdi.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ozl.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mrk.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ope.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kuu.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gxh.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bso.yj202588.top

[E06] 替换子串
来源：http://dtv.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ton.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://xcp.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qti.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://ymn.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yfp.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bxv.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gnc.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://nsi.52xcode.cn

[E07] 按分隔符拆分
来源：http://gzn.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylf.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vhq.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fdx.fanxiaobao.xyz

TS:   s.split(",")
来源：http://jwd.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cfp.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zjg.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://sak.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tiu.daxiang520.top

[E08] 数组按分隔符合并
来源：http://kzc.yfazqb.com

Py:   ",".join(items)
来源：http://ssn.iojbl.cn

PHP:  implode(",", $items);
来源：http://syu.yanxiufei.cn

JS:   items.join(",")
来源：http://xca.andypj.xyz

TS:   items.join(",")
来源：http://gii.zhixingplan.top

Java: String.join(",", items)
来源：http://yod.yj202588.top

Go:   strings.Join(items, ",")
来源：http://avr.shuidangran.top

Ruby: items.join(",")
来源：http://tec.vehdjk.com

C#:   string.Join(",", items)
来源：http://dqc.uphjek.com

[E09] 去除所有空白字符
来源：http://vhk.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jnp.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nnq.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://mmu.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://prf.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://qrm.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cjq.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fhl.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://epz.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://mqg.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dcm.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bao.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://cln.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://lcb.cucudq.cn

Java: String.format("%03d", 7)
来源：http://mxi.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wiz.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://afz.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yxi.wangshuangyany.cn

[E11] 反转字符串
来源：http://yin.shangyingyoupin.top

Py:   s[::-1]
来源：http://zvc.quarkkingdee.top

PHP:  strrev($s);
来源：http://ost.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://ybe.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://tjd.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ken.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://udg.fktsv.cn

Ruby: s.reverse
来源：http://rsk.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://rlw.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://ywe.52xcode.cn

Py:   s.count("a")
来源：http://jln.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://dbv.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://wjw.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://yay.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://poy.meibo888.top

Go:   strings.Count(s, "a")
来源：http://tyg.feifeiyinyue.top

Ruby: s.count("a")
来源：http://mdd.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://nze.smart0.xyz

[E13] 逐字符遍历
来源：http://xrr.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://azs.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ged.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eja.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qoc.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ijw.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ber.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wwq.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://brc.cashguo.top

[E14] URL 编码与 Base64
来源：http://ayu.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qno.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dbi.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dem.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lin.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kpp.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pao.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dqr.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tps.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://bbu.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fsb.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iow.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lch.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uhj.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xvw.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fnp.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qsx.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wjv.gogol.net.cn

[E16] 数字千分位
来源：http://owl.yongpay.top

Py:   f"{1234567:,}"
来源：http://lqn.ybcxt.top

PHP:  number_format(1234567);
来源：http://cpq.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aur.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kuv.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pej.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iuj.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oin.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://lbf.jqgufenzy.top

[E17] 首字母大写
来源：http://awg.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xqn.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nci.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qtt.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqs.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tds.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fay.redwolf501.top

Ruby: s.capitalize
来源：http://jfk.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://idq.hysaishi.cn

[E18] 模板占位符替换
来源：http://ylw.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jdr.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ycr.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wfk.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ztl.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lhm.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ecc.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qmy.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kxx.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://sap.wangshuangyany.cn

Py:   s.splitlines()
来源：http://tvg.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zqh.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://iyp.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://lcc.guannengcc.top

Java: s.lines().toList()
来源：http://qex.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://oao.ivvv.top

Ruby: s.lines
来源：http://jdb.mhx1999.top

C#:   s.Split('\n')
来源：http://vqn.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://mat.aizwys.cn

Py:   if not s:
来源：http://wpk.jiagoushi.top


<!-- 参考信息 -->