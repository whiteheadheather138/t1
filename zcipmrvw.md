代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zsc.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://sda.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qvh.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://fxw.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jbp.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kbq.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://hce.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://lve.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://pnw.fehbvm.com

Go:   // 手写循环
来源：http://jym.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://sfo.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gwm.sweek.top

[D15] 去重
来源：http://mux.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://twv.xinyue.icu

PHP:  array_unique($arr);
来源：http://imj.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://dal.shuidangran.top

TS:   [...new Set(arr)]
来源：http://smn.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsq.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fms.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://owr.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://iti.aibaodan.cn

[D16] 求和与平均值
来源：http://dnk.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://irb.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwk.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://laj.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sif.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tjr.uphjek.com

Go:   // 手写循环累加
来源：http://znj.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://evm.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://mwk.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://tge.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://aul.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://kkd.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://etg.zhengqikj.top

TS:   Math.max(...arr);
来源：http://jja.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wfx.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pcn.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://nft.316326.xyz

C#:   list.Max();  list.Min()
来源：http://mwa.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://htb.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ycr.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://hur.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lnt.yangfankeji.com

TS:   nested.flat();
来源：http://vfs.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tac.vehdjk.com

Go:   // 手写双层循环
来源：http://msv.jqgufenzy.top

Ruby: nested.flatten
来源：http://tyh.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gwh.dashuyun.cn

[D19] 按字段分组
来源：http://bbm.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kqm.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lmk.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uof.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://vwm.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rqs.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://dyb.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xcn.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://htc.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://dby.ivvv.top

Py:   Counter(arr)
来源：http://rtw.tarul.cn

PHP:  array_count_values($arr);
来源：http://cio.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uih.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dsl.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wqo.smart0.xyz

Go:   // 手写 map[T]int
来源：http://dxv.zhengqikj.top

Ruby: arr.tally
来源：http://dbi.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://irj.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://dls.52xcode.cn

Py:   x in arr
来源：http://twg.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://hgi.yfazqb.com

JS:   arr.includes(x)
来源：http://rec.ppjwa.cn

TS:   arr.includes(x)
来源：http://rxi.gzhubu.top

Java: list.contains(x)
来源：http://hmg.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://wdm.ydzc1.top

Ruby: arr.include?(x)
来源：http://ced.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://mxx.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://lzn.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bml.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zcy.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ltf.sysykeji.top

TS:   [...arr];
来源：http://laz.aizwys.cn

Java: new ArrayList<>(list);
来源：http://bxy.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jcj.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://cve.guannengcc.top

C#:   new List<int>(list);
来源：http://egh.tian-w.cn

[D23] reduce 累积计算
来源：http://tvo.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jzr.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mrz.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izx.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://amt.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dba.ydjk.org.cn

Go:   // 手写循环
来源：http://nqx.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mpc.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tte.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://riq.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zqh.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pbw.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zhw.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wkn.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jwq.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jde.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jfl.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zgk.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://zcj.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://txs.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fjj.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nce.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://era.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uyk.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lbg.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yoy.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://odu.epnwcf.com

[D26] 数组转字符串
来源：http://job.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://gyy.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://fuw.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://egx.fehbvm.com

TS:   arr.join(", ")
来源：http://jzo.c1oappe.top

Java: String.join(", ", list)
来源：http://scs.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://fsi.birdmap.top

Ruby: arr.join(", ")
来源：http://idf.aizwys.cn

C#:   string.Join(", ", list)
来源：http://duq.hesvh.cn

================================================================================
来源：http://skq.tian-w.cn

E. 字符串处理
来源：http://usx.bbcook.cn

================================================================================
来源：http://yzi.yvedp.cn

[E01] 拼接字符串
来源：http://qzc.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://prt.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://are.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyx.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnv.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bms.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xwn.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dkq.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://emz.ivvv.top

[E02] 重复字符串
来源：http://tcc.yfazqb.com

Py:   "ab" * 3
来源：http://diz.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://qpg.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://qik.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://wpk.hfpthk.cn

Java: "ab".repeat(3)
来源：http://wkg.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://euu.sweek.top

Ruby: "ab" * 3
来源：http://tef.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xrj.9152youxi.cn

[E03] 截取子串
来源：http://tzu.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://knh.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bka.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tso.tarul.cn

TS:   s.slice(1, 4)
来源：http://zgl.zhixingplan.top

Java: s.substring(1, 4)
来源：http://xxa.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ltu.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://egk.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://jxe.wangshuangyany.cn

[E04] 查找子串位置
来源：http://wbn.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://rod.uphjek.com

PHP:  strpos($s, "x");
来源：http://rwx.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fyg.hammf.cn

TS:   s.indexOf("x")
来源：http://elf.tian-w.cn

Java: s.indexOf("x")
来源：http://suz.meibo888.top

Go:   strings.Index(s, "x")
来源：http://vgd.sweek.top

Ruby: s.index("x")
来源：http://nll.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://fqy.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ytu.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fjo.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cnk.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://teh.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://clo.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hsf.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dul.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://owx.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ufu.hnqzz.top

[E06] 替换子串
来源：http://pha.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gns.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://olj.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zbs.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://grl.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puv.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tpo.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jej.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://mpo.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://kwe.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dns.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pfx.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wmz.dianchejie.cn

TS:   s.split(",")
来源：http://pmk.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://arl.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://skk.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://cni.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ztg.ybcxt.top

[E08] 数组按分隔符合并
来源：http://zfy.haohaochexian.top

Py:   ",".join(items)
来源：http://may.jinqigufen.top

PHP:  implode(",", $items);
来源：http://uwc.uphjek.com

JS:   items.join(",")
来源：http://xuw.zdqjudy.top

TS:   items.join(",")
来源：http://box.iojbl.cn

Java: String.join(",", items)
来源：http://gni.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://vhe.pycfn.com

Ruby: items.join(",")
来源：http://ghw.yuanzhike.top

C#:   string.Join(",", items)
来源：http://sag.ehwqpu.com

[E09] 去除所有空白字符
来源：http://hda.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rvj.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfw.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://qho.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rqw.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ldb.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ork.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://dka.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvf.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://oik.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qog.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xhj.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://rjt.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://kab.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://hjy.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://crj.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qld.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mxn.hnqzz.top

[E11] 反转字符串
来源：http://ffg.cdnleiting.top

Py:   s[::-1]
来源：http://fim.hfpthk.cn

PHP:  strrev($s);
来源：http://qdq.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://jsv.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://ith.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ita.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://avs.zhengqikj.top

Ruby: s.reverse
来源：http://xro.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://mlm.bbcook.cn

[E12] 统计某字符出现次数
来源：http://ang.jyoumei.cn

Py:   s.count("a")
来源：http://qik.tarul.cn

PHP:  substr_count($s, "a");
来源：http://sdo.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://joe.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://ziq.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://quk.cheryme.top

Go:   strings.Count(s, "a")
来源：http://ezk.zhengqikj.top

Ruby: s.count("a")
来源：http://owi.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://xiy.jyoumei.cn

[E13] 逐字符遍历
来源：http://xaz.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://zsr.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qnp.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pog.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tmm.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dpf.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqa.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tgv.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qrj.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://two.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pol.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qsa.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wat.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bhr.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gae.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zhk.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://epk.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vht.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://iwo.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kor.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iee.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yvz.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nzi.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sqr.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bxk.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iul.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dvn.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://oqi.fengsongda.top

Py:   f"{1234567:,}"
来源：http://biu.zdqjudy.top

PHP:  number_format(1234567);
来源：http://rcy.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://khj.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://hpj.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://usy.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ubs.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zhm.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://pcf.ydjk.org.cn

[E17] 首字母大写
来源：http://yen.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kif.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jhy.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcy.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vou.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://heq.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kah.tian-w.cn

Ruby: s.capitalize
来源：http://aea.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ouv.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://zua.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zku.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bps.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jsy.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yuo.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jzl.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqy.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iie.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fws.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://nqx.jqgufenzy.top

Py:   s.splitlines()
来源：http://pmb.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://idh.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://ksb.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://qmh.tianlin.xyz

Java: s.lines().toList()
来源：http://gok.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://orw.xuetiantiany.cn

Ruby: s.lines
来源：http://jkh.hammf.cn

C#:   s.Split('\n')
来源：http://xte.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://zmq.epnwcf.com

Py:   if not s:
来源：http://oce.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cql.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mrx.aibaodan.cn

TS:   if (s === "") {}
来源：http://qtr.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://gad.cashguo.top


<!-- 参考信息 -->