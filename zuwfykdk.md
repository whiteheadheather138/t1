代发 wailian999

Ruby: arr.index(x)
来源：http://hkk.ivvv.top

C#:   list.IndexOf(x);
来源：http://nlm.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://kua.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqt.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hxh.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://nhg.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://rtb.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://srs.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fiv.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://wol.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aon.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://vrb.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mpe.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uzi.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://jnc.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://clb.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bks.gogol.net.cn

Go:   // 手写循环
来源：http://xdg.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qhn.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xdl.fehbvm.com

[D15] 去重
来源：http://ybk.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dsg.tian-w.cn

PHP:  array_unique($arr);
来源：http://hkv.iojbl.cn

JS:   [...new Set(arr)]
来源：http://gln.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://lpl.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vnu.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lka.ydzc1.top

Ruby: arr.uniq
来源：http://zvk.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://dxl.zdbjq.cn

[D16] 求和与平均值
来源：http://eeq.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mmx.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tvt.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ztk.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgy.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://khe.jinqigfzy.top

Go:   // 手写循环累加
来源：http://tfl.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dki.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://pwi.jqgfzy.top

[D17] 最大值与最小值
来源：http://mfx.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://xxu.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://cii.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tpj.9152youxi.cn

TS:   Math.max(...arr);
来源：http://yxb.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gdc.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gmz.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://jxy.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://uxi.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://qxw.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://slz.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://gdq.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yyt.yongpay.top

TS:   nested.flat();
来源：http://tka.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nrc.zycfv.cn

Go:   // 手写双层循环
来源：http://etp.ppjwa.cn

Ruby: nested.flatten
来源：http://kgt.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dmt.nanxuanxn.top

[D19] 按字段分组
来源：http://ege.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://afb.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xmi.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gpk.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://knr.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hid.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://axl.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ntn.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kai.tanke756.top

[D20] 统计每个元素出现次数
来源：http://eox.epnwcf.com

Py:   Counter(arr)
来源：http://wou.guannengcc.top

PHP:  array_count_values($arr);
来源：http://uwq.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyz.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wyg.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kei.zycfv.cn

Go:   // 手写 map[T]int
来源：http://vph.daria6918.cn

Ruby: arr.tally
来源：http://kla.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aia.fengsongda.top

[D21] 判断是否包含某元素
来源：http://bxx.meibo888.top

Py:   x in arr
来源：http://ubl.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://hvu.yj202588.top

JS:   arr.includes(x)
来源：http://vpe.yj20258888.top

TS:   arr.includes(x)
来源：http://dci.ydzc1.top

Java: list.contains(x)
来源：http://nrl.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://qty.zdbjq.cn

Ruby: arr.include?(x)
来源：http://cxn.hfpthk.cn

C#:   list.Contains(x)
来源：http://fyj.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://bkz.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oju.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jyh.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pyw.ydjk.org.cn

TS:   [...arr];
来源：http://rob.yj20258.top

Java: new ArrayList<>(list);
来源：http://xrz.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://tqh.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://mms.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://efj.daria6918.cn

[D23] reduce 累积计算
来源：http://bzh.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kfi.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zlt.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfq.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vym.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gqq.xuanzx.com

Go:   // 手写循环
来源：http://lwf.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oaz.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uxl.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://cjg.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ktx.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zbt.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://esg.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xdk.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://psm.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://awu.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pgd.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vwp.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://tdb.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iji.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqj.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://obf.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xux.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ugq.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qmy.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ghc.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://owe.fktsv.cn

[D26] 数组转字符串
来源：http://vfl.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://vxq.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://umo.52xcode.cn

JS:   arr.join(", ")
来源：http://fzg.hywenlv.cn

TS:   arr.join(", ")
来源：http://tbu.shzxlz.cn

Java: String.join(", ", list)
来源：http://gru.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://nbc.aibaodan.cn

Ruby: arr.join(", ")
来源：http://gqs.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://mss.daria6918.cn

================================================================================
来源：http://czw.fanxiaobao.xyz

E. 字符串处理
来源：http://ogv.jinqigufen.top

================================================================================
来源：http://oqm.cdnleiting.top

[E01] 拼接字符串
来源：http://nzz.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gex.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sku.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://snc.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bhu.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ohn.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qnx.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zdl.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cqp.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://suw.sysykeji.top

Py:   "ab" * 3
来源：http://tkg.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://kpd.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://ivx.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://qaf.sweek.top

Java: "ab".repeat(3)
来源：http://iyi.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://brb.zhijiandao.cn

Ruby: "ab" * 3
来源：http://zwi.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qko.daxiang520.top

[E03] 截取子串
来源：http://kfj.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sjh.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rqd.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vfg.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://ypy.smart0.xyz

Java: s.substring(1, 4)
来源：http://tbu.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mwo.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://wbx.uphjek.com

C#:   s.Substring(1, 3)
来源：http://prm.vqdsnc.cn

[E04] 查找子串位置
来源：http://tpx.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://fer.ybcxt.top

PHP:  strpos($s, "x");
来源：http://wdn.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbf.wangdashe.top

TS:   s.indexOf("x")
来源：http://hid.9152youxi.cn

Java: s.indexOf("x")
来源：http://rtk.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://itv.hongshengwenyu.top

Ruby: s.index("x")
来源：http://qcc.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://dgb.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hhj.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mey.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kwp.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bof.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tdb.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bke.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jnf.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bex.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bli.zdbjq.cn

[E06] 替换子串
来源：http://rvj.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xgz.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://ivp.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdz.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://bmj.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpk.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pmv.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dlo.316326.xyz

C#:   s.Replace("a", "b")
来源：http://sso.52xcode.cn

[E07] 按分隔符拆分
来源：http://bku.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gfx.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wff.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://jkp.chenjidiqi.icu

TS:   s.split(",")
来源：http://mia.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://vwk.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://icn.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://nlt.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esl.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://cvh.ivvv.top

Py:   ",".join(items)
来源：http://rdu.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://tbn.hammf.cn

JS:   items.join(",")
来源：http://ltw.tian-w.cn

TS:   items.join(",")
来源：http://pcl.chenlongwang.top

Java: String.join(",", items)
来源：http://wqf.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://wvr.yuanzhike.top

Ruby: items.join(",")
来源：http://zai.ivvv.top

C#:   string.Join(",", items)
来源：http://ecm.haohaochexian.top

[E09] 去除所有空白字符
来源：http://bwg.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rqk.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uaf.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://tqv.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://izp.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://prw.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bih.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://ltj.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yru.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://mwg.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wtf.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qkg.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://ceh.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://ztn.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://jaj.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://alp.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bma.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bwt.cashguo.top

[E11] 反转字符串
来源：http://otx.yj20258.top

Py:   s[::-1]
来源：http://frq.guannengcc.top

PHP:  strrev($s);
来源：http://iss.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://vap.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://dlc.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dyc.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zfh.zhiwuduotai.top

Ruby: s.reverse
来源：http://mfe.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://drl.guannengcc.top

[E12] 统计某字符出现次数
来源：http://ccs.dashuyun.cn

Py:   s.count("a")
来源：http://lrq.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://kiu.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://vyd.iojbl.cn

TS:   s.split("a").length - 1
来源：http://vyp.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nes.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://gnx.meibo888.top

Ruby: s.count("a")
来源：http://eus.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://qdt.jianghu66.top

[E13] 逐字符遍历
来源：http://wmz.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://bre.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eve.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://umk.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fdh.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xye.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ucw.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://unx.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aux.c1oappe.top

[E14] URL 编码与 Base64
来源：http://ltc.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jng.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qyo.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tcl.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cta.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gjq.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gww.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwg.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rpt.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://flz.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bqr.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dtv.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://slv.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ylz.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pee.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pge.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tnr.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://glj.jqgfzy.top

[E16] 数字千分位
来源：http://dbw.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://ouk.meibo888.top

PHP:  number_format(1234567);
来源：http://ysv.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gdk.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gfn.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jge.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pdg.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vfc.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://uxs.gaohongyu789.top

[E17] 首字母大写
来源：http://clp.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cpk.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fcl.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jtj.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcx.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qdt.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://veo.iojbl.cn

Ruby: s.capitalize
来源：http://zat.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vtk.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://pjj.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ywh.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gkz.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://quj.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pdo.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dat.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cje.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yaz.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ayg.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://rpm.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://spo.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ihr.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://vit.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://xse.xuetiantiany.cn

Java: s.lines().toList()
来源：http://qsc.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://cfs.zhoulong.xyz


<!-- 参考信息 -->