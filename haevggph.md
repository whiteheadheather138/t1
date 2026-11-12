代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aty.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hen.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kbw.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uts.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ecf.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bmx.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qio.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mha.yonumen.top

[D11] 反转数组
来源：http://mqj.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xpk.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://qmg.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kqw.bjfxy.top

TS:   [...arr].reverse();
来源：http://rpg.fengsongda.top

Java: Collections.reverse(list);
来源：http://vao.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://mhh.xylfe.cn

Ruby: arr.reverse
来源：http://brn.mhx1999.top

C#:   list.Reverse();
来源：http://qbj.hongshengwenyu.top

[D12] 查找元素下标
来源：http://zna.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://qth.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hrh.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lbk.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zni.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zun.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://upa.zhixingplan.top

Ruby: arr.index(x)
来源：http://nqn.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://jya.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://dlc.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://unl.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tyi.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://pxu.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://srr.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ago.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kgh.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hid.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bjs.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://mar.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdy.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://beq.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://cyw.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://qqz.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://dmv.wangdashe.top

Go:   // 手写循环
来源：http://psz.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://fjj.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qwz.nwbrower.top

[D15] 去重
来源：http://hnq.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://idr.9152youxi.cn

PHP:  array_unique($arr);
来源：http://wib.sxryk.cn

JS:   [...new Set(arr)]
来源：http://fwt.sysykeji.top

TS:   [...new Set(arr)]
来源：http://lqf.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgj.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nfl.hysaishi.cn

Ruby: arr.uniq
来源：http://vvn.hammf.cn

C#:   list.Distinct().ToList()
来源：http://xat.zhongyouzk.top

[D16] 求和与平均值
来源：http://pjk.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yas.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zwh.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vdu.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iex.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cev.andypj.xyz

Go:   // 手写循环累加
来源：http://keu.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gbq.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://gsz.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://kwj.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://rxj.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://ggt.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jwn.0kj1m.cn

TS:   Math.max(...arr);
来源：http://hfn.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tyh.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vrw.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://gxd.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://elb.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://dxf.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://okb.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://fae.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cxf.zhijiandao.cn

TS:   nested.flat();
来源：http://jdq.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arg.iojbl.cn

Go:   // 手写双层循环
来源：http://ehu.nanxuanxn.top

Ruby: nested.flatten
来源：http://ali.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oqj.tian-w.cn

[D19] 按字段分组
来源：http://psf.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ozk.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vfz.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qvo.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://doy.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cqh.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://kmu.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eih.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyq.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://tzh.shangyingyoupin.top

Py:   Counter(arr)
来源：http://fgd.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://hwq.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pik.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gmc.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bhp.yj202588.top

Go:   // 手写 map[T]int
来源：http://aca.gzhubu.top

Ruby: arr.tally
来源：http://hlo.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pxf.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://oee.hnxiangtu.top

Py:   x in arr
来源：http://zqh.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://rau.cqqwz.cn

JS:   arr.includes(x)
来源：http://wsb.daxiang520.top

TS:   arr.includes(x)
来源：http://lfe.svipenyu.cn

Java: list.contains(x)
来源：http://vvi.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://mxf.hnqzz.top

Ruby: arr.include?(x)
来源：http://dtt.jyoumei.cn

C#:   list.Contains(x)
来源：http://qod.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://gty.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xgf.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ygr.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sxt.zhiwuduotai.top

TS:   [...arr];
来源：http://rwz.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://sis.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://xck.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://jsl.birdmap.top

C#:   new List<int>(list);
来源：http://zij.jqgufenzy.top

[D23] reduce 累积计算
来源：http://ynw.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://man.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ned.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwf.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqf.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wmi.ehwqpu.com

Go:   // 手写循环
来源：http://tii.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://utp.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ldf.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://mzo.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ads.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngk.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://icv.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jgh.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ybb.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oex.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nxi.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ukv.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://iyw.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cpf.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dum.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aia.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qqp.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gyd.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yzd.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wfe.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rfc.redwolf501.top

[D26] 数组转字符串
来源：http://uac.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://pwj.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://zyk.gogol.net.cn

JS:   arr.join(", ")
来源：http://sjr.yfazqb.com

TS:   arr.join(", ")
来源：http://vku.hnxiangtu.top

Java: String.join(", ", list)
来源：http://uuf.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://vzw.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://ctz.yj20258888.top

C#:   string.Join(", ", list)
来源：http://ugo.fehbvm.com

================================================================================
来源：http://abp.ivvv.top

E. 字符串处理
来源：http://gxi.zhengqikj.top

================================================================================
来源：http://ftd.hfpthk.cn

[E01] 拼接字符串
来源：http://rbh.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wgu.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://omw.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hjd.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssp.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iyk.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uam.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wmx.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xkv.fehbvm.com

[E02] 重复字符串
来源：http://ztz.yonumen.top

Py:   "ab" * 3
来源：http://tfp.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://dsw.xziqi.cn

JS:   "ab".repeat(3)
来源：http://opw.guannengcc.top

TS:   "ab".repeat(3)
来源：http://yhy.aizwys.cn

Java: "ab".repeat(3)
来源：http://tot.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://sji.jqgfzy.top

Ruby: "ab" * 3
来源：http://ujs.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gkz.jianghu66.top

[E03] 截取子串
来源：http://pag.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fdm.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qov.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ivk.epnwcf.com

TS:   s.slice(1, 4)
来源：http://swd.zdbjq.cn

Java: s.substring(1, 4)
来源：http://cbu.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lcn.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://yyf.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://fkd.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://jyv.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://bje.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://qed.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ffe.daxiang520.top

TS:   s.indexOf("x")
来源：http://tso.ehwqpu.com

Java: s.indexOf("x")
来源：http://kwo.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://cae.mhx1999.top

Ruby: s.index("x")
来源：http://puh.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://ffk.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ual.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hrl.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://izn.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pib.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://flo.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvk.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mum.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://msf.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hwx.xylfe.cn

[E06] 替换子串
来源：http://idw.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wqn.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://hyf.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vot.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://hgc.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahv.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mef.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yba.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://kjc.andypj.xyz

[E07] 按分隔符拆分
来源：http://yrg.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ejc.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xyj.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyb.yj202588.top

TS:   s.split(",")
来源：http://cze.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://vun.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jrd.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://set.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bqc.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://ctn.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://lxe.zycfv.cn

PHP:  implode(",", $items);
来源：http://sqs.uphjek.com

JS:   items.join(",")
来源：http://oie.dianchejie.cn

TS:   items.join(",")
来源：http://xhx.iojbl.cn

Java: String.join(",", items)
来源：http://ghe.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://gwi.0kj1m.cn

Ruby: items.join(",")
来源：http://ruk.hammf.cn

C#:   string.Join(",", items)
来源：http://vna.cqqwz.cn

[E09] 去除所有空白字符
来源：http://fro.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ifa.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wxd.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://lyt.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://gwn.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://qlp.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jje.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://plw.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofd.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://jbk.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ylt.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://okx.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://qnf.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://dib.vehdjk.com

Java: String.format("%03d", 7)
来源：http://aqv.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jdi.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fkl.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fqb.316326.xyz

[E11] 反转字符串
来源：http://qnd.zhoulong.xyz

Py:   s[::-1]
来源：http://fcl.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://xaa.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://skr.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://qok.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kih.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bvz.hysaishi.cn

Ruby: s.reverse
来源：http://dqv.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bnz.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://qwn.tarul.cn

Py:   s.count("a")
来源：http://hpa.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://zoj.yonumen.top

JS:   s.split("a").length - 1
来源：http://lzl.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://jak.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://snw.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://xsn.chenzaomai.com

Ruby: s.count("a")
来源：http://uew.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://vjb.guannengcc.top

[E13] 逐字符遍历
来源：http://wll.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://ipt.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gdo.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rfa.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://edy.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wyu.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oys.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aqc.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hsi.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://jpl.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rzj.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://exm.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xum.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://itt.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bdv.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xql.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vqf.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ajc.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://hgb.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://edz.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cyq.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bdd.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vee.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qbo.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uzu.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pyl.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhm.xylfe.cn

[E16] 数字千分位
来源：http://ggx.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://kfp.chenzaomai.com

PHP:  number_format(1234567);
来源：http://umt.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rpn.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zlm.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://riu.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fle.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://thp.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://lbk.chenzaomai.com

[E17] 首字母大写
来源：http://ztx.nanxuanxn.top


<!-- 参考信息 -->