代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ipz.zdbjq.cn

Go:   // 手写循环
来源：http://atc.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wmv.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iom.ydjk.org.cn

[D15] 去重
来源：http://ceb.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://awk.iojbl.cn

PHP:  array_unique($arr);
来源：http://aov.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://vdk.hammf.cn

TS:   [...new Set(arr)]
来源：http://seq.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ejw.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://kyh.mhx1999.top

Ruby: arr.uniq
来源：http://dsr.yj20258.top

C#:   list.Distinct().ToList()
来源：http://zft.zhiwuduotai.top

[D16] 求和与平均值
来源：http://fdg.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://srp.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://llg.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mui.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://noq.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zvp.yanxiufei.cn

Go:   // 手写循环累加
来源：http://fze.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kjl.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://fge.nanxinkj.top

[D17] 最大值与最小值
来源：http://obu.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://hqi.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://qdb.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fum.zdbjq.cn

TS:   Math.max(...arr);
来源：http://fob.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://lkm.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iwj.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://wda.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://yfm.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://lrx.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dec.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://fbj.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zmy.gzhubu.top

TS:   nested.flat();
来源：http://qup.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pcf.aizwys.cn

Go:   // 手写双层循环
来源：http://gyv.yangfankeji.com

Ruby: nested.flatten
来源：http://lvg.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yty.aibaodan.cn

[D19] 按字段分组
来源：http://ibg.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nrh.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wti.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bpy.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bhf.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vua.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://pxg.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wwt.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jtr.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://jex.hnxiangtu.top

Py:   Counter(arr)
来源：http://xor.c1oappe.top

PHP:  array_count_values($arr);
来源：http://pvo.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tfx.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dmg.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ahx.daria6918.cn

Go:   // 手写 map[T]int
来源：http://qnm.zhongyouzk.top

Ruby: arr.tally
来源：http://eez.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cmr.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://zlj.fehbvm.com

Py:   x in arr
来源：http://tnr.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://ljy.quarkkingdee.top

JS:   arr.includes(x)
来源：http://hnj.birdmap.top

TS:   arr.includes(x)
来源：http://umf.jlsjyb.cn

Java: list.contains(x)
来源：http://lga.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://byc.zdbjq.cn

Ruby: arr.include?(x)
来源：http://thw.yongpay.top

C#:   list.Contains(x)
来源：http://ene.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://sqq.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bby.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hzs.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://etq.bbcook.cn

TS:   [...arr];
来源：http://ogs.xinyue.icu

Java: new ArrayList<>(list);
来源：http://skw.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://bpy.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://nyk.ivvv.top

C#:   new List<int>(list);
来源：http://vru.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://rwy.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lly.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmp.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bzi.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vec.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gxq.tanke756.top

Go:   // 手写循环
来源：http://ldy.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qmj.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ztt.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://nyj.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rgv.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qup.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rwq.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nob.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ver.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wws.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ipi.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkx.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://nkf.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cwd.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://phq.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fwz.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ndp.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lur.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mmo.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gpk.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nyn.epnwcf.com

[D26] 数组转字符串
来源：http://ulx.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://cua.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://oom.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://ter.sufxvd.cn

TS:   arr.join(", ")
来源：http://ksw.xinyue.icu

Java: String.join(", ", list)
来源：http://gcd.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://uci.fzhhl.top

Ruby: arr.join(", ")
来源：http://wks.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://ydw.shangyingyoupin.top

================================================================================
来源：http://ktr.cqqwz.cn

E. 字符串处理
来源：http://xdh.snrcjt.cn

================================================================================
来源：http://iyg.tianlin.xyz

[E01] 拼接字符串
来源：http://gcf.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wxk.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tkv.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lox.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrf.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zed.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://knp.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pvd.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlm.cucudq.cn

[E02] 重复字符串
来源：http://qpp.nanxinkj.top

Py:   "ab" * 3
来源：http://udj.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://xqr.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://nzj.ydzc1.top

TS:   "ab".repeat(3)
来源：http://ski.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://hav.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://viu.gogol.net.cn

Ruby: "ab" * 3
来源：http://xhr.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qbl.ivvv.top

[E03] 截取子串
来源：http://htd.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yqv.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jdl.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jca.gzhubu.top

TS:   s.slice(1, 4)
来源：http://fym.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://hgb.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eep.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nun.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://qmf.sysykeji.top

[E04] 查找子串位置
来源：http://lck.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://gvt.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://pko.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nyz.zdbjq.cn

TS:   s.indexOf("x")
来源：http://vov.tanke756.top

Java: s.indexOf("x")
来源：http://zhs.tanke756.top

Go:   strings.Index(s, "x")
来源：http://pym.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://gyb.xuanzx.com

C#:   s.IndexOf("x")
来源：http://gzv.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wjt.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pes.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ask.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cgl.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://avj.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://elp.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://maa.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bol.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ucd.tian-w.cn

[E06] 替换子串
来源：http://hmq.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://euj.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://tqs.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcn.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://blf.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umg.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hbd.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gfn.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://nhf.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://ukh.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qso.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ktm.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bqi.feifeiyinyue.top

TS:   s.split(",")
来源：http://jtb.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://ftd.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hhv.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://vkc.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pdv.fengsongda.top

[E08] 数组按分隔符合并
来源：http://fxq.epnwcf.com

Py:   ",".join(items)
来源：http://jvw.cdnleiting.top

PHP:  implode(",", $items);
来源：http://tse.chenzaomai.com

JS:   items.join(",")
来源：http://jwa.jinqigufen.top

TS:   items.join(",")
来源：http://fyz.sweek.top

Java: String.join(",", items)
来源：http://piu.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://otg.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://vnf.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://eza.yueranfly.top

[E09] 去除所有空白字符
来源：http://fgf.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bhs.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nqj.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://xtw.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://knj.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://ntx.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zqx.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://pvu.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ceg.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://vna.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qcg.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rlg.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://cwx.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://urh.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://khs.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bme.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pyz.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://feu.hongshengwenyu.top

[E11] 反转字符串
来源：http://bjt.hesvh.cn

Py:   s[::-1]
来源：http://iql.9152youxi.cn

PHP:  strrev($s);
来源：http://diz.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://rmd.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://bos.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hzb.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kua.gotoacloud.top

Ruby: s.reverse
来源：http://lai.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://mqc.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://ofw.hysaishi.cn

Py:   s.count("a")
来源：http://snx.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://bpc.yj20258888.top

JS:   s.split("a").length - 1
来源：http://dud.iojbl.cn

TS:   s.split("a").length - 1
来源：http://yyu.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://acw.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://dmn.hnqzz.top

Ruby: s.count("a")
来源：http://hyt.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://hvj.zdbjq.cn

[E13] 逐字符遍历
来源：http://uku.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://rul.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wac.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgd.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mba.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ugf.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ehs.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ftu.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rpf.yonumen.top

[E14] URL 编码与 Base64
来源：http://upk.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qsv.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ily.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uvs.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rga.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wpd.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mql.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbt.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bwg.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://zno.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://jgk.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yca.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qjd.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ggj.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfn.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ufu.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://idq.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dwi.shuidangran.top

[E16] 数字千分位
来源：http://oyi.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://ugj.cheryme.top

PHP:  number_format(1234567);
来源：http://vxr.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://mhh.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://duz.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azj.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dbq.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zdv.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://ukp.snrcjt.cn

[E17] 首字母大写
来源：http://xru.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jjw.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kli.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbz.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjm.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ans.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cpp.nanxinkj.top

Ruby: s.capitalize
来源：http://mrq.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwg.chenzaomai.com

[E18] 模板占位符替换
来源：http://enm.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dca.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zno.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fym.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zlr.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wsd.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pvs.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://efo.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rby.smart0.xyz

[E19] 多行文本按行拆分
来源：http://zst.uphjek.com

Py:   s.splitlines()
来源：http://rys.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://geo.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://yrf.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://ozx.yj20258.top

Java: s.lines().toList()
来源：http://ypc.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://qtk.ivvv.top

Ruby: s.lines
来源：http://uxp.zdbjq.cn

C#:   s.Split('\n')
来源：http://kqi.yvedp.cn

[E20] 判断字符串是否为空
来源：http://fry.cucudq.cn

Py:   if not s:
来源：http://rae.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fec.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ofv.hywenlv.cn

TS:   if (s === "") {}
来源：http://fnh.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://ixe.nwbrower.top

Go:   if s == "" {}
来源：http://fyb.c1oappe.top

Ruby: if s.empty?
来源：http://pyj.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oab.sufxvd.cn

[E21] 超长截断加省略号
来源：http://ivq.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uil.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uwy.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rkv.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezk.fanxiaobao.xyz


<!-- 参考信息 -->