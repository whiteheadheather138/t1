代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dew.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://diq.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xfw.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://gye.tarul.cn

Ruby: arr.index(x)
来源：http://wqr.yongpay.top

C#:   list.IndexOf(x);
来源：http://lfs.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://efp.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://flz.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxr.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://zqo.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://dma.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lym.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xkw.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://elj.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ccs.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://lhq.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dew.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qar.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://qws.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://asw.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vwi.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://bgy.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ium.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uyj.jinghuilouyu.cn

[D15] 去重
来源：http://vps.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kps.jiagoushi.top

PHP:  array_unique($arr);
来源：http://ycm.shuidangran.top

JS:   [...new Set(arr)]
来源：http://kvo.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://xro.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bkb.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://xhl.jiagoushi.top

Ruby: arr.uniq
来源：http://qdn.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://ptt.zhengqikj.top

[D16] 求和与平均值
来源：http://dqn.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyk.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qmv.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://clk.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zuu.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://euq.snrcjt.cn

Go:   // 手写循环累加
来源：http://prg.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyz.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://axa.c1oappe.top

[D17] 最大值与最小值
来源：http://blu.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://uuj.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://cji.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tur.yj20258.top

TS:   Math.max(...arr);
来源：http://vhr.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hzh.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zsi.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://vzk.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://ujt.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://axy.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dlu.tanke756.top

PHP:  array_merge(...$nested);
来源：http://xqg.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rts.yj202588.top

TS:   nested.flat();
来源：http://qrj.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yhq.sufxvd.cn

Go:   // 手写双层循环
来源：http://mfv.hysaishi.cn

Ruby: nested.flatten
来源：http://mka.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohb.chenlongwang.top

[D19] 按字段分组
来源：http://nlw.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rvn.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ljk.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jeq.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lmw.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hea.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://for.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fic.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fkl.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://olp.andypj.xyz

Py:   Counter(arr)
来源：http://fpm.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://zmt.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayh.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqe.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://siq.fzhhl.top

Go:   // 手写 map[T]int
来源：http://ush.hcnkem.com

Ruby: arr.tally
来源：http://pwf.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://akn.redwolf501.top

[D21] 判断是否包含某元素
来源：http://zlq.shanyushiyangkeji.top

Py:   x in arr
来源：http://ree.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://zam.yfazqb.com

JS:   arr.includes(x)
来源：http://nan.andypj.xyz

TS:   arr.includes(x)
来源：http://zcy.xylfe.cn

Java: list.contains(x)
来源：http://brx.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://qrf.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://vna.yuanzhike.top

C#:   list.Contains(x)
来源：http://abs.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://jze.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jje.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://syj.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://swh.haohaochexian.top

TS:   [...arr];
来源：http://gtl.hesvh.cn

Java: new ArrayList<>(list);
来源：http://zuj.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://sla.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://aan.sweek.top

C#:   new List<int>(list);
来源：http://zta.yanxiufei.cn

[D23] reduce 累积计算
来源：http://gsv.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dxm.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aey.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hys.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jgv.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bbt.jinqigufen.top

Go:   // 手写循环
来源：http://ewh.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lyz.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hxc.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://cno.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvg.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zoj.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fpc.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mof.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ykw.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iyk.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://adn.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gsf.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://gtz.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://crp.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ygd.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bhy.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bfh.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pce.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://prw.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dkz.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zbb.jyoumei.cn

[D26] 数组转字符串
来源：http://ssl.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://upm.pycfn.com

PHP:  implode(", ", $arr);
来源：http://ecb.tanke756.top

JS:   arr.join(", ")
来源：http://odq.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://idt.ppjwa.cn

Java: String.join(", ", list)
来源：http://hrp.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://gvr.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://jxi.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://vwn.hfpthk.cn

================================================================================
来源：http://kwv.hnqzz.top

E. 字符串处理
来源：http://izm.xylfe.cn

================================================================================
来源：http://qgh.iojbl.cn

[E01] 拼接字符串
来源：http://cqo.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nnf.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mty.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbq.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jcj.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tre.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pvk.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eex.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qrb.andypj.xyz

[E02] 重复字符串
来源：http://cnk.havefunace.top

Py:   "ab" * 3
来源：http://cml.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://bzy.daria6918.cn

JS:   "ab".repeat(3)
来源：http://egl.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://ixj.nanxinkj.top

Java: "ab".repeat(3)
来源：http://nle.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://fqv.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://max.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fon.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://ymz.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qyl.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kmi.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://swr.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://mae.ehwqpu.com

Java: s.substring(1, 4)
来源：http://fqb.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kli.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ghz.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://vtb.vqdsnc.cn

[E04] 查找子串位置
来源：http://phu.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://omo.hnqzz.top

PHP:  strpos($s, "x");
来源：http://urd.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wrx.sufxvd.cn

TS:   s.indexOf("x")
来源：http://qik.guannengcc.top

Java: s.indexOf("x")
来源：http://gwi.uphjek.com

Go:   strings.Index(s, "x")
来源：http://nkf.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://jtg.yj20258.top

C#:   s.IndexOf("x")
来源：http://eoc.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bhh.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uyk.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://day.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ymo.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pfw.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ckf.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kia.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hlp.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://min.pycfn.com

[E06] 替换子串
来源：http://wjn.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dre.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://qdf.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vth.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ztd.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayh.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fxx.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wgw.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://itr.316326.xyz

[E07] 按分隔符拆分
来源：http://nll.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ukj.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pct.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jpu.yonumen.top

TS:   s.split(",")
来源：http://joy.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://pmx.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sgw.yj20258.top

Ruby: s.split(",");  s.split
来源：http://eos.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lio.hesvh.cn

[E08] 数组按分隔符合并
来源：http://ppy.zhongyouzk.top

Py:   ",".join(items)
来源：http://xob.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://klu.zdbjq.cn

JS:   items.join(",")
来源：http://egj.mhx1999.top

TS:   items.join(",")
来源：http://thz.cashguo.top

Java: String.join(",", items)
来源：http://gog.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://dbs.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://any.havefunace.top

C#:   string.Join(",", items)
来源：http://tkd.gotoacloud.top

[E09] 去除所有空白字符
来源：http://ezq.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zzi.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://itr.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://ydj.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://oyj.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://zhe.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://dkm.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://anr.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wgw.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://tew.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://osj.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwg.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://yab.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://wme.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://sru.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddv.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dwh.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xcf.ydzc1.top

[E11] 反转字符串
来源：http://hac.aizwys.cn

Py:   s[::-1]
来源：http://czw.hnxiangtu.top

PHP:  strrev($s);
来源：http://mso.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://pqh.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://dkr.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dtn.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mlw.mhx1999.top

Ruby: s.reverse
来源：http://eke.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xqo.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://tbg.yuxming.cn

Py:   s.count("a")
来源：http://utk.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://bsj.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://pwn.yuxming.cn

TS:   s.split("a").length - 1
来源：http://epf.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fph.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://yho.hammf.cn

Ruby: s.count("a")
来源：http://owp.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://poh.quarkkingdee.top

[E13] 逐字符遍历
来源：http://sts.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://xmb.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ijp.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tlu.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ezf.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jus.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jop.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pzg.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sii.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://tby.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tzg.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fhc.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dop.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://imi.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fil.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zna.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fck.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kly.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://udr.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://meq.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mmb.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jgr.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://oky.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sto.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uwy.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wke.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kbt.sjlbkw.cn

[E16] 数字千分位
来源：http://bne.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://mqr.daxiang520.top

PHP:  number_format(1234567);
来源：http://abi.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mwi.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sss.hongshengwenyu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sio.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wfa.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://olu.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://vwb.daxiang520.top

[E17] 首字母大写
来源：http://eps.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://avk.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rqr.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sbv.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgb.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ksk.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vnn.jinqigfzy.top

Ruby: s.capitalize
来源：http://lsk.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cwy.zycfv.cn

[E18] 模板占位符替换
来源：http://idn.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hzg.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rzq.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pbi.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rbn.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mny.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rkb.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tgx.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nty.bjfxy.top

[E19] 多行文本按行拆分
来源：http://cef.9152youxi.cn

Py:   s.splitlines()
来源：http://twp.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://unu.epnwcf.com


<!-- 参考信息 -->