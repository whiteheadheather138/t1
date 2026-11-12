代发 wailian999

C#:   list.Reverse();
来源：http://tjm.316326.xyz

[D12] 查找元素下标
来源：http://gzx.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://tpk.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vho.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmm.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xsv.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zwi.uphjek.com

Go:   slices.Index(arr, x)
来源：http://oft.guowangkeji.top

Ruby: arr.index(x)
来源：http://odc.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://zvp.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://ndz.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gct.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yis.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://xqo.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://fpb.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gag.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ntb.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://ayr.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uzy.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://duj.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://btc.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ieu.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://izr.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://wld.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://moc.sjlbkw.cn

Go:   // 手写循环
来源：http://dtn.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://tmu.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://trm.xziqi.cn

[D15] 去重
来源：http://bsm.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqp.yonumen.top

PHP:  array_unique($arr);
来源：http://avd.hnqzz.top

JS:   [...new Set(arr)]
来源：http://lvx.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://cbt.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xvu.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://obz.cqqwz.cn

Ruby: arr.uniq
来源：http://jhb.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://czj.svipenyu.cn

[D16] 求和与平均值
来源：http://opc.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vid.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eww.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewc.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://toy.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nwz.dianchejie.cn

Go:   // 手写循环累加
来源：http://mvr.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://suy.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://kow.zhijiandao.cn

[D17] 最大值与最小值
来源：http://fon.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://ltj.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://qvs.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jsu.vehdjk.com

TS:   Math.max(...arr);
来源：http://hii.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iyr.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nsz.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://nex.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://qbo.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://cth.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://exs.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://otz.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvf.ppjwa.cn

TS:   nested.flat();
来源：http://vje.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lzs.c1oappe.top

Go:   // 手写双层循环
来源：http://pkh.zycfv.cn

Ruby: nested.flatten
来源：http://gzg.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nxx.fktsv.cn

[D19] 按字段分组
来源：http://mxv.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://snw.chenjidiqi.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dsx.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://txr.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zja.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ohl.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://vzo.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hzt.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umj.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://fsh.wangdashe.top

Py:   Counter(arr)
来源：http://gnl.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://rim.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yck.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvh.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pps.jianghu66.top

Go:   // 手写 map[T]int
来源：http://out.zhongyouzk.top

Ruby: arr.tally
来源：http://ftg.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xny.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://qkx.zdbjq.cn

Py:   x in arr
来源：http://xwx.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://ydu.aizwys.cn

JS:   arr.includes(x)
来源：http://nrd.ybcxt.top

TS:   arr.includes(x)
来源：http://vzf.nanxinkj.top

Java: list.contains(x)
来源：http://chq.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://pyr.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://toi.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://ghc.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://ihn.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ehw.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hzx.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ezu.yj20258.top

TS:   [...arr];
来源：http://zmx.xuanzx.com

Java: new ArrayList<>(list);
来源：http://jvf.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://wok.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://yry.shuidangran.top

C#:   new List<int>(list);
来源：http://xkn.fktsv.cn

[D23] reduce 累积计算
来源：http://bab.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vma.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ias.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jsb.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eze.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqk.jinqigfzy.top

Go:   // 手写循环
来源：http://wfn.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pas.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://flu.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://sam.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ola.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rqp.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jln.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mwg.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mxb.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zlv.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cvy.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://foi.hammf.cn

[D25] Set 集合去重与交并差
来源：http://ain.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zjc.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tzd.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fas.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://glj.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ufl.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bld.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iam.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zzh.meibo888.top

[D26] 数组转字符串
来源：http://uvk.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://lhi.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://gni.havefunace.top

JS:   arr.join(", ")
来源：http://ozv.yuxming.cn

TS:   arr.join(", ")
来源：http://xul.hysaishi.cn

Java: String.join(", ", list)
来源：http://hmw.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://ija.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://ejh.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://yic.epnwcf.com

================================================================================
来源：http://wrm.jinqigfzy.top

E. 字符串处理
来源：http://kfw.sjlbkw.cn

================================================================================
来源：http://qts.fengsongda.top

[E01] 拼接字符串
来源：http://cej.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwn.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zld.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qzg.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yun.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xzm.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vcn.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xpl.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://klg.zhijiandao.cn

[E02] 重复字符串
来源：http://kbz.vehdjk.com

Py:   "ab" * 3
来源：http://vlf.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://dmc.nwbrower.top

JS:   "ab".repeat(3)
来源：http://rra.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://udx.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://gue.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://tmv.cqqwz.cn

Ruby: "ab" * 3
来源：http://lha.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rdf.ybcxt.top

[E03] 截取子串
来源：http://gix.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://awy.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owi.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ckl.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://wkz.chenzaomai.com

Java: s.substring(1, 4)
来源：http://pzm.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xzl.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://rgr.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://iau.zdqjudy.top

[E04] 查找子串位置
来源：http://jus.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://qne.jianghu66.top

PHP:  strpos($s, "x");
来源：http://coq.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cdm.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://ijv.meibo888.top

Java: s.indexOf("x")
来源：http://tqp.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://ebu.cheryme.top

Ruby: s.index("x")
来源：http://jse.nwbrower.top

C#:   s.IndexOf("x")
来源：http://oli.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://rzw.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hfd.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lgl.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fep.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ulf.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfy.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wyd.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fbk.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mxg.bbcook.cn

[E06] 替换子串
来源：http://ngt.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gsq.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://oed.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yfv.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://xmj.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlu.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dzr.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xsr.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://jab.c1oappe.top

[E07] 按分隔符拆分
来源：http://jtp.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uof.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oiw.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aqm.yj20258888.top

TS:   s.split(",")
来源：http://vcu.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://qhk.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qem.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://zoq.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gzv.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://izk.shzxlz.cn

Py:   ",".join(items)
来源：http://wys.zdqjudy.top

PHP:  implode(",", $items);
来源：http://mwm.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://wqt.yangfankeji.com

TS:   items.join(",")
来源：http://bpg.jiagoushi.top

Java: String.join(",", items)
来源：http://twx.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://cct.ydjk.org.cn

Ruby: items.join(",")
来源：http://xwm.yangfankeji.com

C#:   string.Join(",", items)
来源：http://zte.aizwys.cn

[E09] 去除所有空白字符
来源：http://pqx.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfu.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfh.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wgw.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://hmy.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://dui.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://srn.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hfm.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wbu.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://lak.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ogf.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cos.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://svk.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://hpy.cucudq.cn

Java: String.format("%03d", 7)
来源：http://nqi.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iow.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://riq.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sey.jinghuilouyu.cn

[E11] 反转字符串
来源：http://ksu.sufxvd.cn

Py:   s[::-1]
来源：http://sje.uphjek.com

PHP:  strrev($s);
来源：http://tzn.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://cqr.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://dlx.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vfk.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://myv.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://bfy.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qqk.sysykeji.top

[E12] 统计某字符出现次数
来源：http://prl.daxiang520.top

Py:   s.count("a")
来源：http://rft.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://yun.52xcode.cn

JS:   s.split("a").length - 1
来源：http://aei.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://rxz.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nel.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://gin.redwolf501.top

Ruby: s.count("a")
来源：http://bpg.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://yeb.zdqjudy.top

[E13] 逐字符遍历
来源：http://bgs.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://urf.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tji.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rbe.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bbk.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwb.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ezb.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dfu.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tgr.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://dqw.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cwp.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qvd.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://erc.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jbz.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uog.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://usz.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ojk.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cyk.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://xxi.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://itv.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kkp.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ksv.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eco.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://byn.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gps.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://frm.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hma.xziqi.cn

[E16] 数字千分位
来源：http://lcq.yfazqb.com

Py:   f"{1234567:,}"
来源：http://stp.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://wyg.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qzm.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://omp.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mwq.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xae.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://omc.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://vob.jinqigfzy.top

[E17] 首字母大写
来源：http://nxn.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iuz.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hyh.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mms.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dwl.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zik.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uwj.svipenyu.cn

Ruby: s.capitalize
来源：http://lgs.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aer.haohaochexian.top

[E18] 模板占位符替换
来源：http://vps.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ujq.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jnu.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ghi.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oud.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nzt.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://khx.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qpc.fehbvm.com


<!-- 参考信息 -->