代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvp.nanxuanxn.top

Go:   // 手写循环
来源：http://xgi.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://pep.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://raj.gotoacloud.top

[D15] 去重
来源：http://cuu.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yjt.ivvv.top

PHP:  array_unique($arr);
来源：http://oob.xinyue.icu

JS:   [...new Set(arr)]
来源：http://vac.fktsv.cn

TS:   [...new Set(arr)]
来源：http://auk.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bqy.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ypf.bbcook.cn

Ruby: arr.uniq
来源：http://twc.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://qoz.hesvh.cn

[D16] 求和与平均值
来源：http://ifd.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dvm.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ndj.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpv.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bpf.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgb.hnxiangtu.top

Go:   // 手写循环累加
来源：http://zgi.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lhp.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://wsn.smart0.xyz

[D17] 最大值与最小值
来源：http://uar.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://xat.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://hss.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xpv.yongpay.top

TS:   Math.max(...arr);
来源：http://rmg.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cev.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xjc.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://dpd.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://hfu.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://shm.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ups.meibo888.top

PHP:  array_merge(...$nested);
来源：http://xfk.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvj.tianlin.xyz

TS:   nested.flat();
来源：http://hbi.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sjj.havefunace.top

Go:   // 手写双层循环
来源：http://cqw.epnwcf.com

Ruby: nested.flatten
来源：http://lfi.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tnc.9152youxi.cn

[D19] 按字段分组
来源：http://vrs.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ave.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xvh.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mbk.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ama.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ige.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://fyd.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ezd.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jpr.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://obc.fengsongda.top

Py:   Counter(arr)
来源：http://dhp.cashguo.top

PHP:  array_count_values($arr);
来源：http://epb.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvk.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://log.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oql.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://oey.xziqi.cn

Ruby: arr.tally
来源：http://imr.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://syf.yueranfly.top

[D21] 判断是否包含某元素
来源：http://jow.haohaochexian.top

Py:   x in arr
来源：http://wad.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://ijy.yj20258888.top

JS:   arr.includes(x)
来源：http://ttn.hammf.cn

TS:   arr.includes(x)
来源：http://baz.cheryme.top

Java: list.contains(x)
来源：http://rpy.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://lmz.tian-w.cn

Ruby: arr.include?(x)
来源：http://qzz.zhongyouzk.top

C#:   list.Contains(x)
来源：http://eiq.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://itc.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jvi.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cqg.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baf.haohaochexian.top

TS:   [...arr];
来源：http://gwj.birdmap.top

Java: new ArrayList<>(list);
来源：http://urc.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://umk.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://okt.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://kau.hammf.cn

[D23] reduce 累积计算
来源：http://nmz.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tum.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hrn.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rcb.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://stf.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tri.dashuyun.cn

Go:   // 手写循环
来源：http://acl.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wtc.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vio.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://djr.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tad.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hmu.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vve.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ktg.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nwn.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uzw.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rdh.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lbn.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://unj.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tof.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rbl.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rkv.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vcy.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://end.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bnt.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uck.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fty.hongshengwenyu.top

[D26] 数组转字符串
来源：http://kxq.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://rao.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://hkg.gotoacloud.top

JS:   arr.join(", ")
来源：http://dtx.yuxming.cn

TS:   arr.join(", ")
来源：http://qgp.epnwcf.com

Java: String.join(", ", list)
来源：http://nzz.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://eft.yuxming.cn

Ruby: arr.join(", ")
来源：http://rww.epnwcf.com

C#:   string.Join(", ", list)
来源：http://qey.zhoulong.xyz

================================================================================
来源：http://bkr.xziqi.cn

E. 字符串处理
来源：http://jet.pycfn.com

================================================================================
来源：http://fyw.ivvv.top

[E01] 拼接字符串
来源：http://ias.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://upe.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vvp.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvm.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfd.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://axp.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ksv.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://had.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmb.hammf.cn

[E02] 重复字符串
来源：http://brd.gotoacloud.top

Py:   "ab" * 3
来源：http://qgj.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://njk.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://kir.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://rbd.meibo888.top

Java: "ab".repeat(3)
来源：http://gqy.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://vbb.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://jsa.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://amh.cucudq.cn

[E03] 截取子串
来源：http://wzi.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://abq.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uep.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dcm.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://zra.hywenlv.cn

Java: s.substring(1, 4)
来源：http://iki.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bzv.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://lpo.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://xrs.hfpthk.cn

[E04] 查找子串位置
来源：http://oel.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://fta.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://apw.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iwh.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://vzm.jinqigfzy.top

Java: s.indexOf("x")
来源：http://gwn.yongpay.top

Go:   strings.Index(s, "x")
来源：http://ycl.xinyue.icu

Ruby: s.index("x")
来源：http://jyp.shuidangran.top

C#:   s.IndexOf("x")
来源：http://xvo.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oyj.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bnx.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ttx.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rln.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tsk.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lzf.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lvl.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://prv.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://trc.smart0.xyz

[E06] 替换子串
来源：http://ypq.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kud.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://ybi.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pfb.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://cgb.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pnz.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gpg.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://djj.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://qzw.yj202588.top

[E07] 按分隔符拆分
来源：http://hud.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vyy.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jfa.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://scj.birdmap.top

TS:   s.split(",")
来源：http://jkf.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://yge.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ege.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://hlj.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yfb.xylfe.cn

[E08] 数组按分隔符合并
来源：http://sai.meibo888.top

Py:   ",".join(items)
来源：http://pkh.cucudq.cn

PHP:  implode(",", $items);
来源：http://abw.fanxiaobao.xyz

JS:   items.join(",")
来源：http://uzb.aizwys.cn

TS:   items.join(",")
来源：http://pqd.uphjek.com

Java: String.join(",", items)
来源：http://ptx.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://hej.sjlbkw.cn

Ruby: items.join(",")
来源：http://vli.bbcook.cn

C#:   string.Join(",", items)
来源：http://jvz.jqgfzy.top

[E09] 去除所有空白字符
来源：http://hnn.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jug.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ryg.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://nku.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ymj.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://gfl.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rky.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zvo.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otr.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://iwf.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lku.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qic.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://bnw.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://whe.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://vzf.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://mib.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ggj.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fgr.cdnleiting.top

[E11] 反转字符串
来源：http://ppw.bjfxy.top

Py:   s[::-1]
来源：http://fxc.xziqi.cn

PHP:  strrev($s);
来源：http://azt.meibo888.top

JS:   [...s].reverse().join("")
来源：http://fat.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://uzh.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lys.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yla.yvedp.cn

Ruby: s.reverse
来源：http://cal.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://psn.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://lmy.guannengcc.top

Py:   s.count("a")
来源：http://pba.hammf.cn

PHP:  substr_count($s, "a");
来源：http://egm.xylfe.cn

JS:   s.split("a").length - 1
来源：http://kui.c1oappe.top

TS:   s.split("a").length - 1
来源：http://pwi.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qno.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://zdg.zhoulong.xyz

Ruby: s.count("a")
来源：http://zdv.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://cka.fengsongda.top

[E13] 逐字符遍历
来源：http://wma.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://uqg.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ecc.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pdj.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jij.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vwf.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ccd.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cpz.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ybr.vehdjk.com

[E14] URL 编码与 Base64
来源：http://jqw.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hrz.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bnm.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lsy.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://int.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mgw.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ycw.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zxn.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzy.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://fco.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lsg.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ibr.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xpr.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rvx.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cmi.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ifv.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gjm.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pgz.cashguo.top

[E16] 数字千分位
来源：http://qhr.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://wjs.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://xmx.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://raz.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mhd.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nge.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uom.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pkf.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://pcx.zdqjudy.top

[E17] 首字母大写
来源：http://jjx.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://obw.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vxp.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dwo.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmy.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jsg.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jic.zhengqikj.top

Ruby: s.capitalize
来源：http://lia.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zmn.cdnleiting.top

[E18] 模板占位符替换
来源：http://uwc.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kag.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rpu.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qpa.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ayf.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mdk.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://znd.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ssp.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pky.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://jkd.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://fyl.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://djo.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://idn.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://ftc.nanxuanxn.top

Java: s.lines().toList()
来源：http://fys.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://sld.birdmap.top

Ruby: s.lines
来源：http://tvm.uphjek.com

C#:   s.Split('\n')
来源：http://ota.birdmap.top

[E20] 判断字符串是否为空
来源：http://lxa.yj20258888.top

Py:   if not s:
来源：http://yiz.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vsg.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wyn.ctjpmb.com

TS:   if (s === "") {}
来源：http://dbh.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://thd.pengpengdd.cyou

Go:   if s == "" {}
来源：http://auj.jqgfzy.top

Ruby: if s.empty?
来源：http://yid.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://euv.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://ooj.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxr.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ufs.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymi.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aie.cashguo.top


<!-- 参考信息 -->