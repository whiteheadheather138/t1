代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://fli.nanxuanxn.top

Go:   // 手写循环
来源：http://dmq.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zfw.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jvd.aizwys.cn

[D15] 去重
来源：http://kxc.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gom.svipenyu.cn

PHP:  array_unique($arr);
来源：http://ugx.uphjek.com

JS:   [...new Set(arr)]
来源：http://mcp.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://hvw.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bss.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://afp.jqgfzy.top

Ruby: arr.uniq
来源：http://kti.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://kqh.xinyue.icu

[D16] 求和与平均值
来源：http://qdf.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bfu.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://chh.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://emo.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://trh.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bwi.0kj1m.cn

Go:   // 手写循环累加
来源：http://xti.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wnp.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://wga.yuxming.cn

[D17] 最大值与最小值
来源：http://mwz.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://bcn.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://akg.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nnh.shuidangran.top

TS:   Math.max(...arr);
来源：http://lub.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pjl.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hif.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://rvc.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://jkd.pycfn.com

[D18] 扁平化嵌套数组
来源：http://ikq.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://svw.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://avs.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yto.hnqzz.top

TS:   nested.flat();
来源：http://nig.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wsr.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://rwf.kuanghao11.cn

Ruby: nested.flatten
来源：http://pol.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wrz.cdnleiting.top

[D19] 按字段分组
来源：http://snv.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cmc.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qwc.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eqo.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kkn.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tlk.yongpay.top

Go:   // 手写 map[string][]T
来源：http://fiw.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://imk.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ygi.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://yeq.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://vru.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://pho.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qiz.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jud.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wxk.wangdashe.top

Go:   // 手写 map[T]int
来源：http://xfq.yanxiufei.cn

Ruby: arr.tally
来源：http://evb.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tdy.yj20258.top

[D21] 判断是否包含某元素
来源：http://ofo.tian-w.cn

Py:   x in arr
来源：http://vzl.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://uuy.haohaochexian.top

JS:   arr.includes(x)
来源：http://oqi.quarkkingdee.top

TS:   arr.includes(x)
来源：http://wee.fengsongda.top

Java: list.contains(x)
来源：http://lch.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://wzv.guowangkeji.top

Ruby: arr.include?(x)
来源：http://ynd.xziqi.cn

C#:   list.Contains(x)
来源：http://wdb.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://kvr.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vvx.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pqp.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gel.hesvh.cn

TS:   [...arr];
来源：http://kci.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://qda.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vum.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://sbe.andypj.xyz

C#:   new List<int>(list);
来源：http://nzt.nanxuanxn.top

[D23] reduce 累积计算
来源：http://ohc.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pyb.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ooq.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rcw.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gka.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lgx.zhengqikj.top

Go:   // 手写循环
来源：http://mkk.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://syq.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://azv.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://hse.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dlf.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xww.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://adm.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bso.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tmv.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://evq.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wxg.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tmk.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://dnc.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wzq.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eiz.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zpm.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dvx.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zbe.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sjg.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://htj.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jfz.yongpay.top

[D26] 数组转字符串
来源：http://bls.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://gbi.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://wfo.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://vrc.wangdashe.top

TS:   arr.join(", ")
来源：http://mbb.tian-w.cn

Java: String.join(", ", list)
来源：http://xxl.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://ebx.0kj1m.cn

Ruby: arr.join(", ")
来源：http://kbq.yueranfly.top

C#:   string.Join(", ", list)
来源：http://xtw.iojbl.cn

================================================================================
来源：http://pgw.havefunace.top

E. 字符串处理
来源：http://ged.iojbl.cn

================================================================================
来源：http://igv.fzhhl.top

[E01] 拼接字符串
来源：http://ejv.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vqs.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vox.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gby.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqs.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jsm.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nne.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lud.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mtw.tian-w.cn

[E02] 重复字符串
来源：http://exf.hfpthk.cn

Py:   "ab" * 3
来源：http://tli.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://kfb.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://fsg.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://osv.nwbrower.top

Java: "ab".repeat(3)
来源：http://haf.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://qwp.fehbvm.com

Ruby: "ab" * 3
来源：http://xyb.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rzs.yueranfly.top

[E03] 截取子串
来源：http://jhe.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yvk.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ntl.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bfy.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://dwx.nanxinkj.top

Java: s.substring(1, 4)
来源：http://sph.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://elc.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pmo.meibo888.top

C#:   s.Substring(1, 3)
来源：http://jug.cucudq.cn

[E04] 查找子串位置
来源：http://kuu.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://nyh.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://bjk.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://chk.mhx1999.top

TS:   s.indexOf("x")
来源：http://kih.xuanzx.com

Java: s.indexOf("x")
来源：http://cfw.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://ecw.hysaishi.cn

Ruby: s.index("x")
来源：http://zhq.yj202588.top

C#:   s.IndexOf("x")
来源：http://flb.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vlg.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shh.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cci.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qlp.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qqx.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxh.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kdg.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ixt.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://feh.yuanzhike.top

[E06] 替换子串
来源：http://ack.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whm.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://run.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rly.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://dga.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zet.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://htq.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fpj.meibo888.top

C#:   s.Replace("a", "b")
来源：http://abk.jiagoushi.top

[E07] 按分隔符拆分
来源：http://knl.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fff.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://paj.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lgh.ivvv.top

TS:   s.split(",")
来源：http://ykm.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://lwm.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://slg.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://ctj.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rwq.fengsongda.top

[E08] 数组按分隔符合并
来源：http://tor.sufxvd.cn

Py:   ",".join(items)
来源：http://uyf.chenzaomai.com

PHP:  implode(",", $items);
来源：http://nmw.xuanzx.com

JS:   items.join(",")
来源：http://xpv.havefunace.top

TS:   items.join(",")
来源：http://nht.birdmap.top

Java: String.join(",", items)
来源：http://iex.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://afy.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://ubt.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://ole.andypj.xyz

[E09] 去除所有空白字符
来源：http://rku.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uuu.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kun.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://drx.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://von.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://ril.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mhu.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://spx.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cbf.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://rgf.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oyz.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xft.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://efh.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://qiz.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://med.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kov.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yxg.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eyt.52xcode.cn

[E11] 反转字符串
来源：http://liw.gzhubu.top

Py:   s[::-1]
来源：http://dkr.kuanghao11.cn

PHP:  strrev($s);
来源：http://iju.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://lpu.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://qfs.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fcg.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://zcw.316326.xyz

Ruby: s.reverse
来源：http://mpt.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://mmd.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://qek.tarul.cn

Py:   s.count("a")
来源：http://whd.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://wig.aizwys.cn

JS:   s.split("a").length - 1
来源：http://trn.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://dzw.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hag.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://lfj.yuanzhike.top

Ruby: s.count("a")
来源：http://pfl.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://ltm.xziqi.cn

[E13] 逐字符遍历
来源：http://qrt.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://tfn.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kqj.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vzb.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tqb.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://szx.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cnu.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yum.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://grr.tanke756.top

[E14] URL 编码与 Base64
来源：http://hvp.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wvv.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jdy.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhv.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sng.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qjb.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdv.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zjv.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://utm.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://xbp.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bjq.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://apk.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kxg.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://lnx.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aop.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rcd.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ear.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://day.aizwys.cn

[E16] 数字千分位
来源：http://nmt.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://ihn.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://gxq.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ukv.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://soc.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oby.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dim.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fss.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://afz.xuanzx.com

[E17] 首字母大写
来源：http://dsw.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xiv.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lgc.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfw.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ssq.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sbb.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rwn.yuanzhike.top

Ruby: s.capitalize
来源：http://knt.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://peo.cdnleiting.top

[E18] 模板占位符替换
来源：http://pao.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gsu.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ozv.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qqx.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ejl.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hvy.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hkr.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fgg.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fku.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://bms.ydzc1.top

Py:   s.splitlines()
来源：http://erx.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fap.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://sle.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://dda.jyoumei.cn

Java: s.lines().toList()
来源：http://ebx.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://var.fehbvm.com

Ruby: s.lines
来源：http://sqh.cheryme.top

C#:   s.Split('\n')
来源：http://xvp.xziqi.cn

[E20] 判断字符串是否为空
来源：http://iqj.hysaishi.cn

Py:   if not s:
来源：http://gwi.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mjf.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vjq.tianlin.xyz

TS:   if (s === "") {}
来源：http://rms.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://ebj.bjfxy.top

Go:   if s == "" {}
来源：http://hgm.gaohongyu789.top

Ruby: if s.empty?
来源：http://lqr.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xcl.jqgfzy.top

[E21] 超长截断加省略号
来源：http://ouf.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fzq.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxi.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sem.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nqd.jqgfzy.top


<!-- 参考信息 -->