代发 wailian999

Ruby: arr.index(x)
来源：http://bys.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://swp.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://uaz.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://doj.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wdt.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://hsu.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://mgh.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hxj.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ltt.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hqn.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gyy.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://swa.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxg.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iep.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://fix.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://wsi.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfu.bjfxy.top

Go:   // 手写循环
来源：http://hna.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://mnb.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mjo.zycfv.cn

[D15] 去重
来源：http://vlh.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sps.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://rwd.daria6918.cn

JS:   [...new Set(arr)]
来源：http://bjf.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://fim.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ywl.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fnp.havefunace.top

Ruby: arr.uniq
来源：http://cfy.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://leh.ydzc1.top

[D16] 求和与平均值
来源：http://fbs.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tgp.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://glr.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzk.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://olo.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://heo.jinqigfzy.top

Go:   // 手写循环累加
来源：http://umn.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://efi.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://kfr.nanxuanxn.top

[D17] 最大值与最小值
来源：http://cvz.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://bmh.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://ajg.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qys.iojbl.cn

TS:   Math.max(...arr);
来源：http://cpo.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ivx.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bha.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://lak.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://orr.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://uqr.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hwm.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://pjm.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://btk.zycfv.cn

TS:   nested.flat();
来源：http://zid.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kgq.hywenlv.cn

Go:   // 手写双层循环
来源：http://ptk.feifeiyinyue.top

Ruby: nested.flatten
来源：http://ykq.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nwh.shzxlz.cn

[D19] 按字段分组
来源：http://nag.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://otx.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ocq.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gvv.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fci.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zww.pycfn.com

Go:   // 手写 map[string][]T
来源：http://iww.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnz.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbp.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://qmd.epnwcf.com

Py:   Counter(arr)
来源：http://dys.mhx1999.top

PHP:  array_count_values($arr);
来源：http://lml.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wth.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mkp.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://udp.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://goj.nwbrower.top

Ruby: arr.tally
来源：http://nny.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xjb.vehdjk.com

[D21] 判断是否包含某元素
来源：http://gde.aizwys.cn

Py:   x in arr
来源：http://scy.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://ngv.xinyue.icu

JS:   arr.includes(x)
来源：http://ton.hesvh.cn

TS:   arr.includes(x)
来源：http://xst.9152youxi.cn

Java: list.contains(x)
来源：http://cac.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://wnc.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://due.tanke756.top

C#:   list.Contains(x)
来源：http://qpq.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://pto.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rcl.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cec.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pah.jinghuilouyu.cn

TS:   [...arr];
来源：http://xzf.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://xaz.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kbo.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://ovv.gogol.net.cn

C#:   new List<int>(list);
来源：http://ddm.tian-w.cn

[D23] reduce 累积计算
来源：http://btl.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rdj.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://exq.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mla.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vlz.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vnk.cdnleiting.top

Go:   // 手写循环
来源：http://yhk.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qot.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://foo.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://pik.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://glq.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fco.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yrj.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://chk.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://chs.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ksg.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gie.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ulx.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://twr.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ezx.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zuq.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cff.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mlr.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vgc.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dua.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jof.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vhv.52xcode.cn

[D26] 数组转字符串
来源：http://gpd.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://avh.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://win.iojbl.cn

JS:   arr.join(", ")
来源：http://sqq.jlsjyb.cn

TS:   arr.join(", ")
来源：http://eku.fengsongda.top

Java: String.join(", ", list)
来源：http://yau.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://qow.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://wzv.cheryme.top

C#:   string.Join(", ", list)
来源：http://apf.cucudq.cn

================================================================================
来源：http://ebk.ybcxt.top

E. 字符串处理
来源：http://zhm.shzxlz.cn

================================================================================
来源：http://mrd.ehwqpu.com

[E01] 拼接字符串
来源：http://vmb.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://twy.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsh.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkj.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjj.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ejr.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lib.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wbr.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cft.meibo888.top

[E02] 重复字符串
来源：http://yez.c1oappe.top

Py:   "ab" * 3
来源：http://cqq.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://xmc.xylfe.cn

JS:   "ab".repeat(3)
来源：http://hdl.epnwcf.com

TS:   "ab".repeat(3)
来源：http://dnc.yuxming.cn

Java: "ab".repeat(3)
来源：http://rgy.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://dms.yonumen.top

Ruby: "ab" * 3
来源：http://lcg.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rqp.hesvh.cn

[E03] 截取子串
来源：http://old.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xla.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ncx.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hwm.gzhubu.top

TS:   s.slice(1, 4)
来源：http://ulv.hnqzz.top

Java: s.substring(1, 4)
来源：http://izx.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pti.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://udb.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://uxg.yonumen.top

[E04] 查找子串位置
来源：http://grr.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://upg.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://psd.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lxo.shuidangran.top

TS:   s.indexOf("x")
来源：http://vkb.sysykeji.top

Java: s.indexOf("x")
来源：http://ogs.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://ikx.zhongyouzk.top

Ruby: s.index("x")
来源：http://phg.yj202588.top

C#:   s.IndexOf("x")
来源：http://lji.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ioh.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xay.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oyt.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpp.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://qom.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyr.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kax.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kft.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ves.vqdsnc.cn

[E06] 替换子串
来源：http://rns.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://npj.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://xwq.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyx.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://uvf.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xap.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zfq.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibj.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://yxx.ydzc1.top

[E07] 按分隔符拆分
来源：http://agj.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nzx.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yxr.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://djd.kuanghao11.cn

TS:   s.split(",")
来源：http://xgp.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ooh.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jbg.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://eoh.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://weh.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://rmz.quarkkingdee.top

Py:   ",".join(items)
来源：http://div.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://gjd.ehwqpu.com

JS:   items.join(",")
来源：http://wdn.shanyushiyangtech.top

TS:   items.join(",")
来源：http://djz.iojbl.cn

Java: String.join(",", items)
来源：http://cbj.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://wbb.ctjpmb.com

Ruby: items.join(",")
来源：http://ayv.guannengcc.top

C#:   string.Join(",", items)
来源：http://mfe.xylfe.cn

[E09] 去除所有空白字符
来源：http://axo.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tss.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jrb.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://tzd.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://vdn.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://kai.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yqa.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://mmx.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ysy.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://mpo.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cce.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://okw.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://qfs.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://qeo.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://pef.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://haa.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kaf.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://msd.hesvh.cn

[E11] 反转字符串
来源：http://dcw.fanxiaobao.xyz

Py:   s[::-1]
来源：http://yni.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://dbq.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://rld.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://ywg.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zvu.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgq.vqdsnc.cn

Ruby: s.reverse
来源：http://wcv.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qdt.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://vhr.shanyushiyangtech.top

Py:   s.count("a")
来源：http://msf.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://hlt.52xcode.cn

JS:   s.split("a").length - 1
来源：http://lel.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://ndg.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dqt.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://aef.meibo888.top

Ruby: s.count("a")
来源：http://jxs.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://bke.yueranfly.top

[E13] 逐字符遍历
来源：http://xln.yj20258.top

Py:   for ch in s: print(ch)
来源：http://erk.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ulc.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hko.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tib.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfu.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jqd.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fmt.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mtm.shuidangran.top

[E14] URL 编码与 Base64
来源：http://qrz.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sph.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://axr.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ymv.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ftb.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://myf.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nej.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ibl.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbg.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://alc.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fox.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fng.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ylz.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kue.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wes.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xqb.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lsb.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://efd.yvedp.cn

[E16] 数字千分位
来源：http://kgy.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://nfl.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://lcy.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kyu.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wki.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fjp.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qkz.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lbg.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://dtr.zhongyouzk.top

[E17] 首字母大写
来源：http://ojz.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ipj.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mix.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rnl.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bhr.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aec.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://psg.cdnleiting.top

Ruby: s.capitalize
来源：http://mtz.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wst.shuidangran.top

[E18] 模板占位符替换
来源：http://xli.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rjy.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qzn.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ief.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uzv.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tfn.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rli.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pta.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nmr.pycfn.com

[E19] 多行文本按行拆分
来源：http://hoy.yangfankeji.com

Py:   s.splitlines()
来源：http://ctj.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wfd.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://ycs.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://vax.tian-w.cn

Java: s.lines().toList()
来源：http://spr.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://lau.ybcxt.top


<!-- 参考信息 -->