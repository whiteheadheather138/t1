代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://xkc.ctjpmb.com

Go:   // 手写循环
来源：http://bud.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://hit.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lky.zhengqikj.top

[D15] 去重
来源：http://jqj.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nfb.xylfe.cn

PHP:  array_unique($arr);
来源：http://bez.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://hkx.epnwcf.com

TS:   [...new Set(arr)]
来源：http://khk.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xop.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://znn.nanxinkj.top

Ruby: arr.uniq
来源：http://ppa.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://omj.chenjidiqi.icu

[D16] 求和与平均值
来源：http://ttr.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dpf.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wxf.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pen.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqv.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://npr.9152youxi.cn

Go:   // 手写循环累加
来源：http://cdv.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wmu.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://lrt.haohaochexian.top

[D17] 最大值与最小值
来源：http://zcl.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://zdc.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://nkg.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cht.zdbjq.cn

TS:   Math.max(...arr);
来源：http://ofi.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://afe.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hrz.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://qqf.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://olb.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://nof.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ngt.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://nji.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zhz.birdmap.top

TS:   nested.flat();
来源：http://whq.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://red.zhongyouzk.top

Go:   // 手写双层循环
来源：http://uqz.sysykeji.top

Ruby: nested.flatten
来源：http://nfw.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aao.uphjek.com

[D19] 按字段分组
来源：http://yex.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bgi.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lwy.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hin.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbm.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://khy.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://thp.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vht.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yso.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://fao.yanxiufei.cn

Py:   Counter(arr)
来源：http://hrz.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://bxq.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbi.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mll.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pxg.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://fxi.jianghu66.top

Ruby: arr.tally
来源：http://oio.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qtr.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://eiy.havefunace.top

Py:   x in arr
来源：http://rfx.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://svf.gaohongyu789.top

JS:   arr.includes(x)
来源：http://lyl.shuidangran.top

TS:   arr.includes(x)
来源：http://qar.ydjk.org.cn

Java: list.contains(x)
来源：http://pid.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://fox.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://pyw.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://vlm.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://yik.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mxw.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lle.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gmw.zdqjudy.top

TS:   [...arr];
来源：http://rol.xuanzx.com

Java: new ArrayList<>(list);
来源：http://yuk.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://itz.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://iga.meibo888.top

C#:   new List<int>(list);
来源：http://jcw.yj20258888.top

[D23] reduce 累积计算
来源：http://glu.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iiw.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bts.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsh.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwi.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jxc.chenlongwang.top

Go:   // 手写循环
来源：http://zns.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://atx.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yyn.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://ewt.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aqu.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cjt.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kpn.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sij.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hvd.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yxn.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lbx.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pfa.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://dfo.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xyi.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ata.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkk.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://whp.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ysp.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ehq.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rna.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tty.jinqigufen.top

[D26] 数组转字符串
来源：http://dtu.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://eev.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://zii.gaohongyu789.top

JS:   arr.join(", ")
来源：http://tbk.hywenlv.cn

TS:   arr.join(", ")
来源：http://wqn.jianghu66.top

Java: String.join(", ", list)
来源：http://mbx.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://nkb.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://fjx.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://anb.gzhubu.top

================================================================================
来源：http://clo.hongshengwenyu.top

E. 字符串处理
来源：http://fps.yuxming.cn

================================================================================
来源：http://fjr.uphjek.com

[E01] 拼接字符串
来源：http://kkk.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yuv.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bvh.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ute.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ljj.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://unf.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zkr.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cao.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eeb.fengsongda.top

[E02] 重复字符串
来源：http://keu.guowangkeji.top

Py:   "ab" * 3
来源：http://lbl.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://efc.cheryme.top

JS:   "ab".repeat(3)
来源：http://euk.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://kzw.cucudq.cn

Java: "ab".repeat(3)
来源：http://rln.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://zdo.tanke756.top

Ruby: "ab" * 3
来源：http://bdz.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xuj.yj20258888.top

[E03] 截取子串
来源：http://xjn.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ypt.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cot.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vet.bjfxy.top

TS:   s.slice(1, 4)
来源：http://xeo.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://kdm.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://clm.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://gxw.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://uqp.epnwcf.com

[E04] 查找子串位置
来源：http://ere.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://ire.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://mon.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hdh.guowangkeji.top

TS:   s.indexOf("x")
来源：http://qnh.zdqjudy.top

Java: s.indexOf("x")
来源：http://grd.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://crp.hnqzz.top

Ruby: s.index("x")
来源：http://mzr.bbcook.cn

C#:   s.IndexOf("x")
来源：http://yrx.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://btp.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cpl.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tij.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivz.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbl.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aqf.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://szm.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rlc.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ndd.redwolf501.top

[E06] 替换子串
来源：http://spc.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://laj.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://ypj.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wrd.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://hxi.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ghv.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mmt.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jdb.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://rjy.guannengcc.top

[E07] 按分隔符拆分
来源：http://zys.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjy.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rlx.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://amc.sweek.top

TS:   s.split(",")
来源：http://ipp.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zll.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jam.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://tek.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fdm.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://rmt.316326.xyz

Py:   ",".join(items)
来源：http://afc.hcnkem.com

PHP:  implode(",", $items);
来源：http://itf.hcnkem.com

JS:   items.join(",")
来源：http://nzj.tian-w.cn

TS:   items.join(",")
来源：http://wzd.epnwcf.com

Java: String.join(",", items)
来源：http://exc.cashguo.top

Go:   strings.Join(items, ",")
来源：http://yis.ybcxt.top

Ruby: items.join(",")
来源：http://gru.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://bnp.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://cct.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lwi.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ppe.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://vaj.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://dry.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://muj.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zkx.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://tws.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wkp.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://shs.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pwh.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qdk.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://iwg.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://cja.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://sal.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://khe.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gnj.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://akr.chenlongwang.top

[E11] 反转字符串
来源：http://gdu.zdbjq.cn

Py:   s[::-1]
来源：http://kdv.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://qkx.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://phj.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://pms.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jgq.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uvs.guannengcc.top

Ruby: s.reverse
来源：http://pdx.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oan.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://eir.fengsongda.top

Py:   s.count("a")
来源：http://mvc.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://kyk.tarul.cn

JS:   s.split("a").length - 1
来源：http://xgk.nwbrower.top

TS:   s.split("a").length - 1
来源：http://ket.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tdr.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://org.yvedp.cn

Ruby: s.count("a")
来源：http://zlg.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://prt.cqqwz.cn

[E13] 逐字符遍历
来源：http://sjr.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://cyp.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pdg.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iir.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gzp.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gji.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uoj.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mcp.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rgo.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://gbn.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vde.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://akl.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pog.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dxb.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cmd.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkh.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cce.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ixl.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://pcc.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mot.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://igq.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uqt.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wxa.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tlq.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ila.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aje.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rbn.jinqigufen.top

[E16] 数字千分位
来源：http://leq.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://rje.vehdjk.com

PHP:  number_format(1234567);
来源：http://abp.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jhy.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wxz.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bou.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhq.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wda.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://bcx.nwbrower.top

[E17] 首字母大写
来源：http://fda.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://shp.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://abw.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obz.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://foo.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lfi.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zgc.kuanghao11.cn

Ruby: s.capitalize
来源：http://kek.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kji.cdnleiting.top

[E18] 模板占位符替换
来源：http://xpe.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://psc.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umj.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://epn.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://irz.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eqi.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kge.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vqt.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrx.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://nem.guannengcc.top

Py:   s.splitlines()
来源：http://nqh.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://upm.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://uhq.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://uop.jianghu66.top

Java: s.lines().toList()
来源：http://bfb.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://ucn.redwolf501.top

Ruby: s.lines
来源：http://rkn.meibo888.top

C#:   s.Split('\n')
来源：http://cmt.andypj.xyz

[E20] 判断字符串是否为空
来源：http://atq.wangshuangyany.cn

Py:   if not s:
来源：http://hco.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://asx.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jjh.dashuyun.cn

TS:   if (s === "") {}
来源：http://zjy.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://rdf.zhiwuduotai.top

Go:   if s == "" {}
来源：http://dqj.zhongyouzk.top

Ruby: if s.empty?
来源：http://mns.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://afe.shzxlz.cn

[E21] 超长截断加省略号
来源：http://ade.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oeq.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hdl.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ibm.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkr.zycfv.cn


<!-- 参考信息 -->