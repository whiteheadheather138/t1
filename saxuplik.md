代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oqh.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://knx.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://unn.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://zin.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://zxb.sxryk.cn

Go:   // 手写循环
来源：http://mej.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wmm.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sbf.zhongyouzk.top

[D15] 去重
来源：http://zar.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pqc.gzhubu.top

PHP:  array_unique($arr);
来源：http://zfc.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://hgh.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://pfw.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oim.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://vre.gaohongyu789.top

Ruby: arr.uniq
来源：http://nar.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://wmi.jqgfzy.top

[D16] 求和与平均值
来源：http://zur.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yid.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sbm.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mbl.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bcs.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hsm.xziqi.cn

Go:   // 手写循环累加
来源：http://kcs.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tfi.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://yya.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://byv.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://hel.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://wdu.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://btd.hcnkem.com

TS:   Math.max(...arr);
来源：http://gpj.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dgr.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftn.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://ula.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://pex.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://ehc.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vnw.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://poc.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lqf.cdnleiting.top

TS:   nested.flat();
来源：http://daw.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://esr.aibaodan.cn

Go:   // 手写双层循环
来源：http://aam.zdbjq.cn

Ruby: nested.flatten
来源：http://tnm.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tbg.cdnleiting.top

[D19] 按字段分组
来源：http://ice.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vhj.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sik.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gma.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hzh.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufw.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://vwm.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sum.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nxk.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://owg.zhongyouzk.top

Py:   Counter(arr)
来源：http://lju.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://diq.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxn.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hkn.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dus.yj20258888.top

Go:   // 手写 map[T]int
来源：http://wxx.zhongyouzk.top

Ruby: arr.tally
来源：http://ijn.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qto.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://gsu.redwolf501.top

Py:   x in arr
来源：http://erj.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://hut.zhijiandao.cn

JS:   arr.includes(x)
来源：http://jbt.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://djs.ivvv.top

Java: list.contains(x)
来源：http://qyc.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://rfm.cqqwz.cn

Ruby: arr.include?(x)
来源：http://tma.yonumen.top

C#:   list.Contains(x)
来源：http://hik.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://zqw.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ikj.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mwr.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fdk.ivvv.top

TS:   [...arr];
来源：http://nqw.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://kbi.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://snd.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://zei.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://dbs.jlsjyb.cn

[D23] reduce 累积计算
来源：http://htf.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gor.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uzd.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lls.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://whb.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jwk.zdbjq.cn

Go:   // 手写循环
来源：http://gpb.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://guc.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zua.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://sey.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bbv.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ese.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mbx.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tij.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gza.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldj.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kvx.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jgw.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://tqe.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xkl.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vgo.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngm.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cyq.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gvw.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bqv.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lhh.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uqh.zhijiandao.cn

[D26] 数组转字符串
来源：http://ctq.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://zoi.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://lzf.andypj.xyz

JS:   arr.join(", ")
来源：http://cgh.ydjk.org.cn

TS:   arr.join(", ")
来源：http://xsc.pycfn.com

Java: String.join(", ", list)
来源：http://vkb.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://wnw.yuxming.cn

Ruby: arr.join(", ")
来源：http://uee.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://mnu.uphjek.com

================================================================================
来源：http://feo.xylfe.cn

E. 字符串处理
来源：http://ooa.52xcode.cn

================================================================================
来源：http://rku.dashuyun.cn

[E01] 拼接字符串
来源：http://hti.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pgx.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ght.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzx.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bge.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dye.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zum.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sva.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bjg.aibaodan.cn

[E02] 重复字符串
来源：http://lyf.yuanzhike.top

Py:   "ab" * 3
来源：http://ola.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://mbl.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://gqc.316326.xyz

TS:   "ab".repeat(3)
来源：http://jac.yueranfly.top

Java: "ab".repeat(3)
来源：http://dfc.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://lps.hnxiangtu.top

Ruby: "ab" * 3
来源：http://whs.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yii.sjlbkw.cn

[E03] 截取子串
来源：http://nix.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://klw.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://avg.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pns.hesvh.cn

TS:   s.slice(1, 4)
来源：http://luz.ctjpmb.com

Java: s.substring(1, 4)
来源：http://jhz.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vlb.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://knc.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://oua.daria6918.cn

[E04] 查找子串位置
来源：http://rhb.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://cze.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://gqj.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yis.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://jhr.hysaishi.cn

Java: s.indexOf("x")
来源：http://jsi.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://wmb.havefunace.top

Ruby: s.index("x")
来源：http://chi.yj20258888.top

C#:   s.IndexOf("x")
来源：http://hrx.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xhe.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dhm.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tpb.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ouf.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dic.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rrw.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kct.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uoe.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jmc.jqgufenzy.top

[E06] 替换子串
来源：http://wbz.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rxn.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ume.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://emv.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://now.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ung.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xfr.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sml.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://jtg.aibaodan.cn

[E07] 按分隔符拆分
来源：http://mhn.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wwr.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ana.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://res.cheryme.top

TS:   s.split(",")
来源：http://nie.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://ntm.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fjp.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://lsu.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kuv.xziqi.cn

[E08] 数组按分隔符合并
来源：http://nku.zhijiandao.cn

Py:   ",".join(items)
来源：http://aat.birdmap.top

PHP:  implode(",", $items);
来源：http://dfk.sweek.top

JS:   items.join(",")
来源：http://ews.smart0.xyz

TS:   items.join(",")
来源：http://fvd.ehwqpu.com

Java: String.join(",", items)
来源：http://kpb.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://vww.316326.xyz

Ruby: items.join(",")
来源：http://sdl.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://fkr.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://kma.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xsh.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jok.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://xzh.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://lhg.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://jzk.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jdd.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lkz.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mjc.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://qmp.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rpu.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mjl.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://bgj.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://sjv.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://vqh.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kwr.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xqq.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://frd.chenlongwang.top

[E11] 反转字符串
来源：http://ncg.fktsv.cn

Py:   s[::-1]
来源：http://elc.yuxming.cn

PHP:  strrev($s);
来源：http://stu.yj20258.top

JS:   [...s].reverse().join("")
来源：http://bzh.tanke756.top

TS:   [...s].reverse().join("")
来源：http://itr.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cvv.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kyq.hfpthk.cn

Ruby: s.reverse
来源：http://geb.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://yug.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://cwg.cucudq.cn

Py:   s.count("a")
来源：http://gxc.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://rgd.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://pox.nwbrower.top

TS:   s.split("a").length - 1
来源：http://cgj.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tna.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://cyo.yanxiufei.cn

Ruby: s.count("a")
来源：http://rzp.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://nuv.quarkkingdee.top

[E13] 逐字符遍历
来源：http://eua.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://zbg.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qmu.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kla.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://paf.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nec.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://itv.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xlx.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://omt.epnwcf.com

[E14] URL 编码与 Base64
来源：http://ogt.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ezr.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hpw.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gch.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baf.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qsn.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kxh.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bmv.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbc.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://ovq.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rks.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oya.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oqw.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nqv.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bzs.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ubp.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kbt.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://syc.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://aja.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://zuw.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://yep.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cnd.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kym.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://efr.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://air.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wes.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://hha.0kj1m.cn

[E17] 首字母大写
来源：http://lig.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zhq.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bvh.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfx.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mlg.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yge.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hoa.guowangkeji.top

Ruby: s.capitalize
来源：http://qxo.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rlr.cdnleiting.top

[E18] 模板占位符替换
来源：http://pak.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ruy.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ylm.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fbz.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qth.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xbw.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qex.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gvj.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ipw.fktsv.cn

[E19] 多行文本按行拆分
来源：http://jje.smart0.xyz

Py:   s.splitlines()
来源：http://sek.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ijw.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://ltg.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://oua.jlsjyb.cn

Java: s.lines().toList()
来源：http://kqi.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://rww.fktsv.cn

Ruby: s.lines
来源：http://gzl.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://mmv.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://ghg.kuanghao11.cn

Py:   if not s:
来源：http://uxa.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://byv.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vkt.316326.xyz

TS:   if (s === "") {}
来源：http://mdb.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://gcb.tianlin.xyz

Go:   if s == "" {}
来源：http://prl.hammf.cn

Ruby: if s.empty?
来源：http://uld.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://arg.sweek.top

[E21] 超长截断加省略号
来源：http://jjv.meibo888.top


<!-- 参考信息 -->